**Project ID:** [plumID:19.027]({{ '/' | absolute_url }}eggs/19/027/)  
Stderr for source:  MulticanonicalSimulations/Multicanonical/Analysis/SampledDistribution/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @28 : keyword ARG is compulsory for this action
[fv-az1718-879:12003] *** Process received signal ***
[fv-az1718-879:12003] Signal: Aborted (6)
[fv-az1718-879:12003] Signal code:  (-6)
[fv-az1718-879:12003] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4e67645330]
[fv-az1718-879:12003] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4e6769eb2c]
[fv-az1718-879:12003] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4e6764527e]
[fv-az1718-879:12003] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4e676288ff]
[fv-az1718-879:12003] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4e67aa5ff5]
[fv-az1718-879:12003] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4e67abb0da]
[fv-az1718-879:12003] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4e67aa5a55]
[fv-az1718-879:12003] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4e67aa5a6f]
[fv-az1718-879:12003] [ 8] plumed_master(+0x146dd)[0x561d005d06dd]
[fv-az1718-879:12003] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4e6762a1ca]
[fv-az1718-879:12003] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4e6762a28b]
[fv-az1718-879:12003] [11] plumed_master(+0x15365)[0x561d005d1365]
[fv-az1718-879:12003] *** End of error message ***
</pre>
{% endraw %}
