**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COLLECT with label cc_ns : missing TYPE keyword.  TYPE should specify whether data is to be stored as a vector or a matrix
[fv-az1372-996:11461] *** Process received signal ***
[fv-az1372-996:11461] Signal: Aborted (6)
[fv-az1372-996:11461] Signal code:  (-6)
[fv-az1372-996:11461] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f095c245330]
[fv-az1372-996:11461] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f095c29eb2c]
[fv-az1372-996:11461] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f095c24527e]
[fv-az1372-996:11461] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f095c2288ff]
[fv-az1372-996:11461] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f095c6a5ff5]
[fv-az1372-996:11461] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f095c6bb0da]
[fv-az1372-996:11461] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f095c6a5a55]
[fv-az1372-996:11461] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f095c6a5a6f]
[fv-az1372-996:11461] [ 8] plumed_master(+0x146dd)[0x55f4a7e996dd]
[fv-az1372-996:11461] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f095c22a1ca]
[fv-az1372-996:11461] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f095c22a28b]
[fv-az1372-996:11461] [11] plumed_master(+0x15365)[0x55f4a7e9a365]
[fv-az1372-996:11461] *** End of error message ***
</pre>
{% endraw %}
