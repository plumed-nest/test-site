**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PDB2CONSTANT with label @s95 : argument O1O_lessthan was not set in pdb input
[fv-az2027-338:11093] *** Process received signal ***
[fv-az2027-338:11093] Signal: Aborted (6)
[fv-az2027-338:11093] Signal code:  (-6)
[fv-az2027-338:11093] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa304045330]
[fv-az2027-338:11093] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa30409eb2c]
[fv-az2027-338:11093] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa30404527e]
[fv-az2027-338:11093] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa3040288ff]
[fv-az2027-338:11093] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa3044a5ff5]
[fv-az2027-338:11093] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa3044bb0da]
[fv-az2027-338:11093] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa3044a5a55]
[fv-az2027-338:11093] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa3044a5a6f]
[fv-az2027-338:11093] [ 8] plumed(+0x146dd)[0x559f9bac96dd]
[fv-az2027-338:11093] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa30402a1ca]
[fv-az2027-338:11093] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa30402a28b]
[fv-az2027-338:11093] [11] plumed(+0x15365)[0x559f9baca365]
[fv-az2027-338:11093] *** End of error message ***
</pre>
{% endraw %}
