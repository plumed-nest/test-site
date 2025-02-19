**Project ID:** [plumID:25.006]({{ '/' | absolute_url }}eggs/25/006/)  
Stderr for source:  PROTACs_PBMetaD_PLUMED-NEST/Input_Files/plumed_lastbias.dat   
Download: [zipped raw stdout](plumed_lastbias.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_lastbias.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label d_tbut_ph_brd4 : could not find file named ../colvar_distances.data
[fv-az1770-999:05276] *** Process received signal ***
[fv-az1770-999:05276] Signal: Aborted (6)
[fv-az1770-999:05276] Signal code:  (-6)
[fv-az1770-999:05276] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f85e1a45330]
[fv-az1770-999:05276] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f85e1a9eb2c]
[fv-az1770-999:05276] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f85e1a4527e]
[fv-az1770-999:05276] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f85e1a288ff]
[fv-az1770-999:05276] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f85e1ea5ff5]
[fv-az1770-999:05276] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f85e1ebb0da]
[fv-az1770-999:05276] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f85e1ea5a55]
[fv-az1770-999:05276] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f85e1ea5a6f]
[fv-az1770-999:05276] [ 8] plumed(+0x146dd)[0x55f188dab6dd]
[fv-az1770-999:05276] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f85e1a2a1ca]
[fv-az1770-999:05276] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f85e1a2a28b]
[fv-az1770-999:05276] [11] plumed(+0x15365)[0x55f188dac365]
[fv-az1770-999:05276] *** End of error message ***
</pre>
{% endraw %}
