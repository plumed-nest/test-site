**Project ID:** [plumID:24.033]({{ '/' | absolute_url }}eggs/24/033/)  
Stderr for source:  Plumed-nest/7q4m/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action EMMI with label gmm : REWEIGHT can only be used in parallel with 2 or more replicas
[fv-az1945-156:05525] *** Process received signal ***
[fv-az1945-156:05525] Signal: Aborted (6)
[fv-az1945-156:05525] Signal code:  (-6)
[fv-az1945-156:05525] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f20acc45330]
[fv-az1945-156:05525] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f20acc9eb2c]
[fv-az1945-156:05525] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f20acc4527e]
[fv-az1945-156:05525] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f20acc288ff]
[fv-az1945-156:05525] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f20ad0a5ff5]
[fv-az1945-156:05525] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f20ad0bb0da]
[fv-az1945-156:05525] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f20ad0a5a55]
[fv-az1945-156:05525] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f20ad0a5a6f]
[fv-az1945-156:05525] [ 8] plumed(+0x146dd)[0x55deda2566dd]
[fv-az1945-156:05525] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f20acc2a1ca]
[fv-az1945-156:05525] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f20acc2a28b]
[fv-az1945-156:05525] [11] plumed(+0x15365)[0x55deda257365]
[fv-az1945-156:05525] *** End of error message ***
</pre>
{% endraw %}
