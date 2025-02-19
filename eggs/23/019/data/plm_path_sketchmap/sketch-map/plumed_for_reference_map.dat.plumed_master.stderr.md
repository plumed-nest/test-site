**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_for_reference_map.dat   
Download: [zipped raw stdout](plumed_for_reference_map.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_for_reference_map.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action VSTACK with label mat : keyword ARG is compulsory for this action
[fv-az1718-879:06360] *** Process received signal ***
[fv-az1718-879:06360] Signal: Aborted (6)
[fv-az1718-879:06360] Signal code:  (-6)
[fv-az1718-879:06360] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efc73a45330]
[fv-az1718-879:06360] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efc73a9eb2c]
[fv-az1718-879:06360] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efc73a4527e]
[fv-az1718-879:06360] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efc73a288ff]
[fv-az1718-879:06360] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efc73ea5ff5]
[fv-az1718-879:06360] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efc73ebb0da]
[fv-az1718-879:06360] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efc73ea5a55]
[fv-az1718-879:06360] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efc73ea5a6f]
[fv-az1718-879:06360] [ 8] plumed_master(+0x146dd)[0x55e86475b6dd]
[fv-az1718-879:06360] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efc73a2a1ca]
[fv-az1718-879:06360] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efc73a2a28b]
[fv-az1718-879:06360] [11] plumed_master(+0x15365)[0x55e86475c365]
[fv-az1718-879:06360] *** End of error message ***
</pre>
{% endraw %}
