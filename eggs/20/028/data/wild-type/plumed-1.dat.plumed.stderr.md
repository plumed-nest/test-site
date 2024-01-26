**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  wild-type/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:137) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  461  97.1
[fv-az1148-6:09023] *** Process received signal ***
[fv-az1148-6:09023] Signal: Aborted (6)
[fv-az1148-6:09023] Signal code:  (-6)
[fv-az1148-6:09023] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8556c42520]
[fv-az1148-6:09023] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8556c969fc]
[fv-az1148-6:09023] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8556c42476]
[fv-az1148-6:09023] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8556c287f3]
[fv-az1148-6:09023] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f85570a4f26]
[fv-az1148-6:09023] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f85570b6d9c]
[fv-az1148-6:09023] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f85570b6e07]
[fv-az1148-6:09023] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f85570b70bb]
[fv-az1148-6:09023] [ 8] plumed(+0x12f48)[0x55a28437df48]
[fv-az1148-6:09023] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8556c29d90]
[fv-az1148-6:09023] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8556c29e40]
[fv-az1148-6:09023] [11] plumed(+0x131e5)[0x55a28437e1e5]
[fv-az1148-6:09023] *** End of error message ***
</pre>
{% endraw %}
