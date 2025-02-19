**Project ID:** [plumID:24.033]({{ '/' | absolute_url }}eggs/24/033/)  
Stderr for source:  Plumed-nest/7q4b/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action EMMI with label gmm : REWEIGHT can only be used in parallel with 2 or more replicas
[fv-az1945-156:05369] *** Process received signal ***
[fv-az1945-156:05369] Signal: Aborted (6)
[fv-az1945-156:05369] Signal code:  (-6)
[fv-az1945-156:05369] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1402c45330]
[fv-az1945-156:05369] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1402c9eb2c]
[fv-az1945-156:05369] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1402c4527e]
[fv-az1945-156:05369] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1402c288ff]
[fv-az1945-156:05369] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f14030a5ff5]
[fv-az1945-156:05369] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f14030bb0da]
[fv-az1945-156:05369] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f14030a5a55]
[fv-az1945-156:05369] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f14030a5a6f]
[fv-az1945-156:05369] [ 8] plumed_master(+0x146dd)[0x5564bed806dd]
[fv-az1945-156:05369] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1402c2a1ca]
[fv-az1945-156:05369] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1402c2a28b]
[fv-az1945-156:05369] [11] plumed_master(+0x15365)[0x5564bed81365]
[fv-az1945-156:05369] *** End of error message ***
</pre>
{% endraw %}
