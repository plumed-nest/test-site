**Project ID:** [plumID:22.028]({{ '/' | absolute_url }}eggs/22/028/)  
Stderr for source:  plumed_pucker.dat   
Download: [zipped raw stdout](plumed_pucker.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_pucker.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label puck1 : could not find file named COLVAR_theta.0
[fv-az1372-996:08522] *** Process received signal ***
[fv-az1372-996:08522] Signal: Aborted (6)
[fv-az1372-996:08522] Signal code:  (-6)
[fv-az1372-996:08522] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f068f845330]
[fv-az1372-996:08522] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f068f89eb2c]
[fv-az1372-996:08522] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f068f84527e]
[fv-az1372-996:08522] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f068f8288ff]
[fv-az1372-996:08522] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f068fca5ff5]
[fv-az1372-996:08522] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f068fcbb0da]
[fv-az1372-996:08522] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f068fca5a55]
[fv-az1372-996:08522] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f068fca5a6f]
[fv-az1372-996:08522] [ 8] plumed(+0x146dd)[0x55fa4360c6dd]
[fv-az1372-996:08522] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f068f82a1ca]
[fv-az1372-996:08522] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f068f82a28b]
[fv-az1372-996:08522] [11] plumed(+0x15365)[0x55fa4360d365]
[fv-az1372-996:08522] *** End of error message ***
</pre>
{% endraw %}
