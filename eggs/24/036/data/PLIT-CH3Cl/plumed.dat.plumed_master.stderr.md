**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  PLIT-CH3Cl/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @45 : keyword ARG is compulsory for this action
[fv-az2027-338:05585] *** Process received signal ***
[fv-az2027-338:05585] Signal: Aborted (6)
[fv-az2027-338:05585] Signal code:  (-6)
[fv-az2027-338:05585] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff184645330]
[fv-az2027-338:05585] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff18469eb2c]
[fv-az2027-338:05585] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff18464527e]
[fv-az2027-338:05585] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff1846288ff]
[fv-az2027-338:05585] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff184aa5ff5]
[fv-az2027-338:05585] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff184abb0da]
[fv-az2027-338:05585] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff184aa5a55]
[fv-az2027-338:05585] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff184aa5a6f]
[fv-az2027-338:05585] [ 8] plumed_master(+0x146dd)[0x55c6b98d46dd]
[fv-az2027-338:05585] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff18462a1ca]
[fv-az2027-338:05585] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff18462a28b]
[fv-az2027-338:05585] [11] plumed_master(+0x15365)[0x55c6b98d5365]
[fv-az2027-338:05585] *** End of error message ***
</pre>
{% endraw %}
