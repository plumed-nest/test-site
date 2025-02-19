**Project ID:** [plumID:22.006]({{ '/' | absolute_url }}eggs/22/006/)  
Stderr for source:  analysis/new_cvs.plumed   
Download: [zipped raw stdout](new_cvs.plumed.plumed_master.stdout.txt.zip) - [zipped raw stderr](new_cvs.plumed.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @94 : keyword ARG is compulsory for this action
[fv-az2027-338:06801] *** Process received signal ***
[fv-az2027-338:06801] Signal: Aborted (6)
[fv-az2027-338:06801] Signal code:  (-6)
[fv-az2027-338:06801] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0277245330]
[fv-az2027-338:06801] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f027729eb2c]
[fv-az2027-338:06801] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f027724527e]
[fv-az2027-338:06801] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f02772288ff]
[fv-az2027-338:06801] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f02776a5ff5]
[fv-az2027-338:06801] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f02776bb0da]
[fv-az2027-338:06801] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f02776a5a55]
[fv-az2027-338:06801] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f02776a5a6f]
[fv-az2027-338:06801] [ 8] plumed_master(+0x146dd)[0x5603b8a436dd]
[fv-az2027-338:06801] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f027722a1ca]
[fv-az2027-338:06801] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f027722a28b]
[fv-az2027-338:06801] [11] plumed_master(+0x15365)[0x5603b8a44365]
[fv-az2027-338:06801] *** End of error message ***
</pre>
{% endraw %}
