**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_forward.dat   
Download: [zipped raw stdout](plumed_Argon_forward.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[fv-az1372-996:05847] *** Process received signal ***
[fv-az1372-996:05847] Signal: Aborted (6)
[fv-az1372-996:05847] Signal code:  (-6)
[fv-az1372-996:05847] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7faf9e645330]
[fv-az1372-996:05847] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7faf9e69eb2c]
[fv-az1372-996:05847] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7faf9e64527e]
[fv-az1372-996:05847] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7faf9e6288ff]
[fv-az1372-996:05847] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7faf9eaa5ff5]
[fv-az1372-996:05847] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7faf9eabb0da]
[fv-az1372-996:05847] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7faf9eaa5a55]
[fv-az1372-996:05847] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7faf9eaa5a6f]
[fv-az1372-996:05847] [ 8] plumed_master(+0x146dd)[0x5605418296dd]
[fv-az1372-996:05847] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7faf9e62a1ca]
[fv-az1372-996:05847] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7faf9e62a28b]
[fv-az1372-996:05847] [11] plumed_master(+0x15365)[0x56054182a365]
[fv-az1372-996:05847] *** End of error message ***
</pre>
{% endraw %}
