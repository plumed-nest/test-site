**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  oncogenic/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:137) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  483  97.1
[fv-az2031-223:44123] *** Process received signal ***
[fv-az2031-223:44123] Signal: Aborted (6)
[fv-az2031-223:44123] Signal code:  (-6)
[fv-az2031-223:44123] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7faa96642520]
[fv-az2031-223:44123] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7faa966969fc]
[fv-az2031-223:44123] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7faa96642476]
[fv-az2031-223:44123] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7faa966287f3]
[fv-az2031-223:44123] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7faa96aa2b9e]
[fv-az2031-223:44123] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7faa96aae20c]
[fv-az2031-223:44123] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7faa96aae277]
[fv-az2031-223:44123] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7faa96aae52b]
[fv-az2031-223:44123] [ 8] plumed(+0x12f48)[0x56298c362f48]
[fv-az2031-223:44123] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7faa96629d90]
[fv-az2031-223:44123] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7faa96629e40]
[fv-az2031-223:44123] [11] plumed(+0x131e5)[0x56298c3631e5]
[fv-az2031-223:44123] *** End of error message ***
</pre>
{% endraw %}
