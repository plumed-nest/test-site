**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  DIDE-water/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @47 : keyword ARG is compulsory for this action
[fv-az2027-338:05437] *** Process received signal ***
[fv-az2027-338:05437] Signal: Aborted (6)
[fv-az2027-338:05437] Signal code:  (-6)
[fv-az2027-338:05437] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1da5045330]
[fv-az2027-338:05437] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1da509eb2c]
[fv-az2027-338:05437] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1da504527e]
[fv-az2027-338:05437] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1da50288ff]
[fv-az2027-338:05437] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1da54a5ff5]
[fv-az2027-338:05437] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1da54bb0da]
[fv-az2027-338:05437] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1da54a5a55]
[fv-az2027-338:05437] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1da54a5a6f]
[fv-az2027-338:05437] [ 8] plumed_master(+0x146dd)[0x55f4aea046dd]
[fv-az2027-338:05437] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1da502a1ca]
[fv-az2027-338:05437] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1da502a28b]
[fv-az2027-338:05437] [11] plumed_master(+0x15365)[0x55f4aea05365]
[fv-az2027-338:05437] *** End of error message ***
</pre>
{% endraw %}
