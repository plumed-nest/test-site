**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat   
Download: [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[fv-az1113-981:41245] *** Process received signal ***
[fv-az1113-981:41245] Signal: Aborted (6)
[fv-az1113-981:41245] Signal code:  (-6)
[fv-az1113-981:41245] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd29fe42520]
[fv-az1113-981:41245] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd29fe969fc]
[fv-az1113-981:41245] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd29fe42476]
[fv-az1113-981:41245] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd29fe287f3]
[fv-az1113-981:41245] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd2a02a2b9e]
[fv-az1113-981:41245] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd2a02ae20c]
[fv-az1113-981:41245] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd2a02ae277]
[fv-az1113-981:41245] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd2a02ae52b]
[fv-az1113-981:41245] [ 8] plumed_master(+0x14274)[0x5557dc32e274]
[fv-az1113-981:41245] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd29fe29d90]
[fv-az1113-981:41245] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd29fe29e40]
[fv-az1113-981:41245] [11] plumed_master(+0x14ed5)[0x5557dc32eed5]
[fv-az1113-981:41245] *** End of error message ***
</pre>
{% endraw %}
