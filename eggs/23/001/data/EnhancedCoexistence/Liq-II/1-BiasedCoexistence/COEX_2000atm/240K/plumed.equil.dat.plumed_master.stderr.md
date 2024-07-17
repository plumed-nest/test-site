**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.equil.dat   
Download: [zipped raw stdout](plumed.equil.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.equil.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : missing input file ice.pdb
[fv-az695-456:71735] *** Process received signal ***
[fv-az695-456:71735] Signal: Aborted (6)
[fv-az695-456:71735] Signal code:  (-6)
[fv-az695-456:71735] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f065de42520]
[fv-az695-456:71735] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f065de969fc]
[fv-az695-456:71735] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f065de42476]
[fv-az695-456:71735] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f065de287f3]
[fv-az695-456:71735] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f065e2a2b9e]
[fv-az695-456:71735] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f065e2ae20c]
[fv-az695-456:71735] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f065e2ae277]
[fv-az695-456:71735] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f065e2ae52b]
[fv-az695-456:71735] [ 8] plumed_master(+0x14274)[0x556e48f63274]
[fv-az695-456:71735] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f065de29d90]
[fv-az695-456:71735] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f065de29e40]
[fv-az695-456:71735] [11] plumed_master(+0x14ed5)[0x556e48f63ed5]
[fv-az695-456:71735] *** End of error message ***
</pre>
{% endraw %}
