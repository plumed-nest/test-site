**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  wild-type/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:141) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  461  97.1
[fv-az1148-6:09033] *** Process received signal ***
[fv-az1148-6:09033] Signal: Aborted (6)
[fv-az1148-6:09033] Signal code:  (-6)
[fv-az1148-6:09033] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f86a9242520]
[fv-az1148-6:09033] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f86a92969fc]
[fv-az1148-6:09033] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f86a9242476]
[fv-az1148-6:09033] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f86a92287f3]
[fv-az1148-6:09033] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f86a96a4f26]
[fv-az1148-6:09033] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f86a96b6d9c]
[fv-az1148-6:09033] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f86a96b6e07]
[fv-az1148-6:09033] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f86a96b70bb]
[fv-az1148-6:09033] [ 8] plumed_master(+0x12ebf)[0x55c8f4275ebf]
[fv-az1148-6:09033] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f86a9229d90]
[fv-az1148-6:09033] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f86a9229e40]
[fv-az1148-6:09033] [11] plumed_master(+0x13155)[0x55c8f4276155]
[fv-az1148-6:09033] *** End of error message ***
</pre>
{% endraw %}
