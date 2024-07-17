**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[fv-az695-456:71797] *** Process received signal ***
[fv-az695-456:71797] Signal: Aborted (6)
[fv-az695-456:71797] Signal code:  (-6)
[fv-az695-456:71797] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f82d3a42520]
[fv-az695-456:71797] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f82d3a969fc]
[fv-az695-456:71797] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f82d3a42476]
[fv-az695-456:71797] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f82d3a287f3]
[fv-az695-456:71797] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f82d3ea2b9e]
[fv-az695-456:71797] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f82d3eae20c]
[fv-az695-456:71797] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f82d3eae277]
[fv-az695-456:71797] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f82d3eae52b]
[fv-az695-456:71797] [ 8] plumed_master(+0x14274)[0x5636f49c3274]
[fv-az695-456:71797] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f82d3a29d90]
[fv-az695-456:71797] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f82d3a29e40]
[fv-az695-456:71797] [11] plumed_master(+0x14ed5)[0x5636f49c3ed5]
[fv-az695-456:71797] *** End of error message ***
</pre>
{% endraw %}
