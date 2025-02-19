**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
Stderr for source:  PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_read.dat   
Download: [zipped raw stdout](plumed_read.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_read.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label d_tbut_ph_brd4 : could not find file named ../colvar_distances.data
[fv-az1770-999:05400] *** Process received signal ***
[fv-az1770-999:05400] Signal: Aborted (6)
[fv-az1770-999:05400] Signal code:  (-6)
[fv-az1770-999:05400] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb267a45330]
[fv-az1770-999:05400] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb267a9eb2c]
[fv-az1770-999:05400] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb267a4527e]
[fv-az1770-999:05400] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb267a288ff]
[fv-az1770-999:05400] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb267ea5ff5]
[fv-az1770-999:05400] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb267ebb0da]
[fv-az1770-999:05400] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb267ea5a55]
[fv-az1770-999:05400] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb267ea5a6f]
[fv-az1770-999:05400] [ 8] plumed_master(+0x146dd)[0x55931224e6dd]
[fv-az1770-999:05400] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb267a2a1ca]
[fv-az1770-999:05400] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb267a2a28b]
[fv-az1770-999:05400] [11] plumed_master(+0x15365)[0x55931224f365]
[fv-az1770-999:05400] *** End of error message ***
</pre>
{% endraw %}
