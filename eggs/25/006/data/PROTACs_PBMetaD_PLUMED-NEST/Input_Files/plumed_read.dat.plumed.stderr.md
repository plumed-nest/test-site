**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
Stderr for source:  PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_read.dat   
Download: [zipped raw stdout](plumed_read.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_read.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label d_tbut_ph_brd4 : could not find file named ../colvar_distances.data
[fv-az1770-999:05384] *** Process received signal ***
[fv-az1770-999:05384] Signal: Aborted (6)
[fv-az1770-999:05384] Signal code:  (-6)
[fv-az1770-999:05384] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2457245330]
[fv-az1770-999:05384] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f245729eb2c]
[fv-az1770-999:05384] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f245724527e]
[fv-az1770-999:05384] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f24572288ff]
[fv-az1770-999:05384] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f24576a5ff5]
[fv-az1770-999:05384] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f24576bb0da]
[fv-az1770-999:05384] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f24576a5a55]
[fv-az1770-999:05384] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f24576a5a6f]
[fv-az1770-999:05384] [ 8] plumed(+0x146dd)[0x555ed75a56dd]
[fv-az1770-999:05384] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f245722a1ca]
[fv-az1770-999:05384] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f245722a28b]
[fv-az1770-999:05384] [11] plumed(+0x15365)[0x555ed75a6365]
[fv-az1770-999:05384] *** End of error message ***
</pre>
{% endraw %}
