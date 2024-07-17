**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat   
Download: [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[fv-az695-456:71766] *** Process received signal ***
[fv-az695-456:71766] Signal: Aborted (6)
[fv-az695-456:71766] Signal code:  (-6)
[fv-az695-456:71766] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd9af242520]
[fv-az695-456:71766] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd9af2969fc]
[fv-az695-456:71766] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd9af242476]
[fv-az695-456:71766] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd9af2287f3]
[fv-az695-456:71766] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd9af6a2b9e]
[fv-az695-456:71766] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd9af6ae20c]
[fv-az695-456:71766] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd9af6ae277]
[fv-az695-456:71766] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd9af6ae52b]
[fv-az695-456:71766] [ 8] plumed_master(+0x14274)[0x55cba0a35274]
[fv-az695-456:71766] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd9af229d90]
[fv-az695-456:71766] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd9af229e40]
[fv-az695-456:71766] [11] plumed_master(+0x14ed5)[0x55cba0a35ed5]
[fv-az695-456:71766] *** End of error message ***
</pre>
{% endraw %}
