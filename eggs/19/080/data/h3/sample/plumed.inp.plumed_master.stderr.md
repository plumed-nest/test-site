**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
Stderr for source:  h3/sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @33 : keyword ARG is compulsory for this action
[fv-az1436-30:11817] *** Process received signal ***
[fv-az1436-30:11817] Signal: Aborted (6)
[fv-az1436-30:11817] Signal code:  (-6)
[fv-az1436-30:11817] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa1b9045330]
[fv-az1436-30:11817] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa1b909eb2c]
[fv-az1436-30:11817] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa1b904527e]
[fv-az1436-30:11817] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa1b90288ff]
[fv-az1436-30:11817] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa1b94a5ff5]
[fv-az1436-30:11817] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa1b94bb0da]
[fv-az1436-30:11817] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa1b94a5a55]
[fv-az1436-30:11817] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa1b94a5a6f]
[fv-az1436-30:11817] [ 8] plumed_master(+0x146dd)[0x55b0a13a86dd]
[fv-az1436-30:11817] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa1b902a1ca]
[fv-az1436-30:11817] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa1b902a28b]
[fv-az1436-30:11817] [11] plumed_master(+0x15365)[0x55b0a13a9365]
[fv-az1436-30:11817] *** End of error message ***
</pre>
{% endraw %}
