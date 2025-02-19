**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_for_reference_map.dat   
Download: [zipped raw stdout](plumed_for_reference_map.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_for_reference_map.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[fv-az1718-879:06343] *** Process received signal ***
[fv-az1718-879:06343] Signal: Aborted (6)
[fv-az1718-879:06343] Signal code:  (-6)
[fv-az1718-879:06343] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdeb8645330]
[fv-az1718-879:06343] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdeb869eb2c]
[fv-az1718-879:06343] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdeb864527e]
[fv-az1718-879:06343] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdeb86288ff]
[fv-az1718-879:06343] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdeb8aa5ff5]
[fv-az1718-879:06343] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdeb8abb0da]
[fv-az1718-879:06343] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdeb8aa5a55]
[fv-az1718-879:06343] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdeb8aa5a6f]
[fv-az1718-879:06343] [ 8] plumed(+0x146dd)[0x55e813e016dd]
[fv-az1718-879:06343] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdeb862a1ca]
[fv-az1718-879:06343] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdeb862a28b]
[fv-az1718-879:06343] [11] plumed(+0x15365)[0x55e813e02365]
[fv-az1718-879:06343] *** End of error message ***
</pre>
{% endraw %}
