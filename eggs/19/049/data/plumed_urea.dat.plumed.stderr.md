**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_urea.dat   
Download: [zipped raw stdout](plumed_urea.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_urea.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX with label @s41 : missing SWITCH11 keyword
[fv-az1947-39:14197] *** Process received signal ***
[fv-az1947-39:14197] Signal: Aborted (6)
[fv-az1947-39:14197] Signal code:  (-6)
[fv-az1947-39:14197] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f36d8445330]
[fv-az1947-39:14197] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f36d849eb2c]
[fv-az1947-39:14197] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f36d844527e]
[fv-az1947-39:14197] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f36d84288ff]
[fv-az1947-39:14197] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f36d88a5ff5]
[fv-az1947-39:14197] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f36d88bb0da]
[fv-az1947-39:14197] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f36d88a5a55]
[fv-az1947-39:14197] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f36d88a5a6f]
[fv-az1947-39:14197] [ 8] plumed(+0x146dd)[0x55f31c1d46dd]
[fv-az1947-39:14197] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f36d842a1ca]
[fv-az1947-39:14197] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f36d842a28b]
[fv-az1947-39:14197] [11] plumed(+0x15365)[0x55f31c1d5365]
[fv-az1947-39:14197] *** End of error message ***
</pre>
{% endraw %}
