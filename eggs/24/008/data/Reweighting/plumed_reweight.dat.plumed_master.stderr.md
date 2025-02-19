**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1945-156:06798] *** Process received signal ***
[fv-az1945-156:06798] Signal: Aborted (6)
[fv-az1945-156:06798] Signal code:  (-6)
[fv-az1945-156:06798] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f082b445330]
[fv-az1945-156:06798] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f082b49eb2c]
[fv-az1945-156:06798] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f082b44527e]
[fv-az1945-156:06798] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f082b4288ff]
[fv-az1945-156:06798] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f082b8a5ff5]
[fv-az1945-156:06798] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f082b8bb0da]
[fv-az1945-156:06798] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f082b8a5a55]
[fv-az1945-156:06798] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f082b8a5a6f]
[fv-az1945-156:06798] [ 8] plumed_master(+0x146dd)[0x55ab19d356dd]
[fv-az1945-156:06798] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f082b42a1ca]
[fv-az1945-156:06798] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f082b42a28b]
[fv-az1945-156:06798] [11] plumed_master(+0x15365)[0x55ab19d36365]
[fv-az1945-156:06798] *** End of error message ***
</pre>
{% endraw %}
