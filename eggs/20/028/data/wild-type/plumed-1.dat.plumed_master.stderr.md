**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  wild-type/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:151) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  461  97.1
[fv-az1326-415:12438] *** Process received signal ***
[fv-az1326-415:12438] Signal: Aborted (6)
[fv-az1326-415:12438] Signal code:  (-6)
[fv-az1326-415:12438] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7774245330]
[fv-az1326-415:12438] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f777429eb2c]
[fv-az1326-415:12438] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f777424527e]
[fv-az1326-415:12438] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f77742288ff]
[fv-az1326-415:12438] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f77746a5ff5]
[fv-az1326-415:12438] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f77746bb0da]
[fv-az1326-415:12438] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f77746a5a55]
[fv-az1326-415:12438] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f77746a5a6f]
[fv-az1326-415:12438] [ 8] plumed_master(+0x146dd)[0x55b4543d86dd]
[fv-az1326-415:12438] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f777422a1ca]
[fv-az1326-415:12438] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f777422a28b]
[fv-az1326-415:12438] [11] plumed_master(+0x15365)[0x55b4543d9365]
[fv-az1326-415:12438] *** End of error message ***
</pre>
{% endraw %}
