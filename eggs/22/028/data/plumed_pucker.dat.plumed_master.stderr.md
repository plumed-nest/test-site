**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az1372-996:08538] *** Process received signal ***
[fv-az1372-996:08538] Signal: Aborted (6)
[fv-az1372-996:08538] Signal code:  (-6)
[fv-az1372-996:08538] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2b0fe45330]
[fv-az1372-996:08538] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2b0fe9eb2c]
[fv-az1372-996:08538] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2b0fe4527e]
[fv-az1372-996:08538] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2b0fe288ff]
[fv-az1372-996:08538] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2b102a5ff5]
[fv-az1372-996:08538] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2b102bb0da]
[fv-az1372-996:08538] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2b102a5a55]
[fv-az1372-996:08538] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2b102a5a6f]
[fv-az1372-996:08538] [ 8] plumed_master(+0x146dd)[0x5634b28706dd]
[fv-az1372-996:08538] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2b0fe2a1ca]
[fv-az1372-996:08538] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2b0fe2a28b]
[fv-az1372-996:08538] [11] plumed_master(+0x15365)[0x5634b2871365]
[fv-az1372-996:08538] *** End of error message ***
</pre>
{% endraw %}
