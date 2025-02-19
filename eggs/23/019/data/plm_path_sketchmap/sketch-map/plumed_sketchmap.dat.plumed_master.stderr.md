**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_sketchmap.dat   
Download: [zipped raw stdout](plumed_sketchmap.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sketchmap.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action VSTACK with label mat : keyword ARG is compulsory for this action
[fv-az1718-879:06439] *** Process received signal ***
[fv-az1718-879:06439] Signal: Aborted (6)
[fv-az1718-879:06439] Signal code:  (-6)
[fv-az1718-879:06439] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f948cc45330]
[fv-az1718-879:06439] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f948cc9eb2c]
[fv-az1718-879:06439] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f948cc4527e]
[fv-az1718-879:06439] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f948cc288ff]
[fv-az1718-879:06439] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f948d0a5ff5]
[fv-az1718-879:06439] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f948d0bb0da]
[fv-az1718-879:06439] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f948d0a5a55]
[fv-az1718-879:06439] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f948d0a5a6f]
[fv-az1718-879:06439] [ 8] plumed_master(+0x146dd)[0x55caf06106dd]
[fv-az1718-879:06439] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f948cc2a1ca]
[fv-az1718-879:06439] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f948cc2a28b]
[fv-az1718-879:06439] [11] plumed_master(+0x15365)[0x55caf0611365]
[fv-az1718-879:06439] *** End of error message ***
</pre>
{% endraw %}
