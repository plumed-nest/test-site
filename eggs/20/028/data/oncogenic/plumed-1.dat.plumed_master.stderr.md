**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  oncogenic/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:151) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  483  97.1
[fv-az2031-223:44131] *** Process received signal ***
[fv-az2031-223:44131] Signal: Aborted (6)
[fv-az2031-223:44131] Signal code:  (-6)
[fv-az2031-223:44131] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3ebca42520]
[fv-az2031-223:44131] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3ebca969fc]
[fv-az2031-223:44131] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3ebca42476]
[fv-az2031-223:44131] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3ebca287f3]
[fv-az2031-223:44131] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3ebcea2b9e]
[fv-az2031-223:44131] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3ebceae20c]
[fv-az2031-223:44131] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3ebceae277]
[fv-az2031-223:44131] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3ebceae52b]
[fv-az2031-223:44131] [ 8] plumed_master(+0x14274)[0x55b552e16274]
[fv-az2031-223:44131] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3ebca29d90]
[fv-az2031-223:44131] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3ebca29e40]
[fv-az2031-223:44131] [11] plumed_master(+0x14ed5)[0x55b552e16ed5]
[fv-az2031-223:44131] *** End of error message ***
</pre>
{% endraw %}
