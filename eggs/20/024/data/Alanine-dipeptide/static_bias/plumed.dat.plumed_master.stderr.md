**Project ID:** [plumID:20.024]({{ '/' | absolute_url }}eggs/20/024/)  
Stderr for source:  Alanine-dipeptide/static_bias/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Keywords.cpp:385) void PLMD::Keywords::use(std::string_view)
+++ assertion failed: reserved(k)
the ARG keyword is not reserved
[fv-az1672-644:08522] *** Process received signal ***
[fv-az1672-644:08522] Signal: Aborted (6)
[fv-az1672-644:08522] Signal code:  (-6)
[fv-az1672-644:08522] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5d7a445330]
[fv-az1672-644:08522] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5d7a49eb2c]
[fv-az1672-644:08522] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5d7a44527e]
[fv-az1672-644:08522] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5d7a4288ff]
[fv-az1672-644:08522] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5d7a8a5ff5]
[fv-az1672-644:08522] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5d7a8bb0da]
[fv-az1672-644:08522] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5d7a8a5a55]
[fv-az1672-644:08522] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5d7a8a5a6f]
[fv-az1672-644:08522] [ 8] plumed_master(+0x146dd)[0x55c37acdf6dd]
[fv-az1672-644:08522] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5d7a42a1ca]
[fv-az1672-644:08522] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5d7a42a28b]
[fv-az1672-644:08522] [11] plumed_master(+0x15365)[0x55c37ace0365]
[fv-az1672-644:08522] *** End of error message ***
</pre>
{% endraw %}
