**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_backward.dat   
Download: [zipped raw stdout](plumed_Argon_backward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_backward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[fv-az1372-996:05778] *** Process received signal ***
[fv-az1372-996:05778] Signal: Aborted (6)
[fv-az1372-996:05778] Signal code:  (-6)
[fv-az1372-996:05778] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5900e45330]
[fv-az1372-996:05778] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5900e9eb2c]
[fv-az1372-996:05778] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5900e4527e]
[fv-az1372-996:05778] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5900e288ff]
[fv-az1372-996:05778] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f59012a5ff5]
[fv-az1372-996:05778] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f59012bb0da]
[fv-az1372-996:05778] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f59012a5a55]
[fv-az1372-996:05778] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f59012a5a6f]
[fv-az1372-996:05778] [ 8] plumed(+0x146dd)[0x559d3b3d66dd]
[fv-az1372-996:05778] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5900e2a1ca]
[fv-az1372-996:05778] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5900e2a28b]
[fv-az1372-996:05778] [11] plumed(+0x15365)[0x559d3b3d7365]
[fv-az1372-996:05778] *** End of error message ***
</pre>
{% endraw %}
