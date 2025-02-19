**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_Argon_forward.dat   
Download: [zipped raw stdout](plumed_Argon_forward.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_Argon_forward.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action COORDINATIONNUMBER with label @s11 : keyword MORE_THAN could not be read correctly
[fv-az1372-996:05831] *** Process received signal ***
[fv-az1372-996:05831] Signal: Aborted (6)
[fv-az1372-996:05831] Signal code:  (-6)
[fv-az1372-996:05831] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6510645330]
[fv-az1372-996:05831] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f651069eb2c]
[fv-az1372-996:05831] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f651064527e]
[fv-az1372-996:05831] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f65106288ff]
[fv-az1372-996:05831] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6510aa5ff5]
[fv-az1372-996:05831] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6510abb0da]
[fv-az1372-996:05831] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6510aa5a55]
[fv-az1372-996:05831] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6510aa5a6f]
[fv-az1372-996:05831] [ 8] plumed(+0x146dd)[0x55887ce766dd]
[fv-az1372-996:05831] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f651062a1ca]
[fv-az1372-996:05831] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f651062a28b]
[fv-az1372-996:05831] [11] plumed(+0x15365)[0x55887ce77365]
[fv-az1372-996:05831] *** End of error message ***
</pre>
{% endraw %}
