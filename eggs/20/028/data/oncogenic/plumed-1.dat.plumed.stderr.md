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
[fv-az1148-6:09056] *** Process received signal ***
[fv-az1148-6:09056] Signal: Aborted (6)
[fv-az1148-6:09056] Signal code:  (-6)
[fv-az1148-6:09056] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f96a1042520]
[fv-az1148-6:09056] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f96a10969fc]
[fv-az1148-6:09056] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f96a1042476]
[fv-az1148-6:09056] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f96a10287f3]
[fv-az1148-6:09056] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f96a14a4f26]
[fv-az1148-6:09056] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f96a14b6d9c]
[fv-az1148-6:09056] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f96a14b6e07]
[fv-az1148-6:09056] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f96a14b70bb]
[fv-az1148-6:09056] [ 8] plumed(+0x12f48)[0x55566805ff48]
[fv-az1148-6:09056] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f96a1029d90]
[fv-az1148-6:09056] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f96a1029e40]
[fv-az1148-6:09056] [11] plumed(+0x131e5)[0x5556680601e5]
[fv-az1148-6:09056] *** End of error message ***
</pre>
{% endraw %}
