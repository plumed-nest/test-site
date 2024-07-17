**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az695-456:71697] *** Process received signal ***
[fv-az695-456:71697] Signal: Aborted (6)
[fv-az695-456:71697] Signal code:  (-6)
[fv-az695-456:71697] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3788e42520]
[fv-az695-456:71697] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3788e969fc]
[fv-az695-456:71697] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3788e42476]
[fv-az695-456:71697] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3788e287f3]
[fv-az695-456:71697] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f37892a2b9e]
[fv-az695-456:71697] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f37892ae20c]
[fv-az695-456:71697] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f37892ae277]
[fv-az695-456:71697] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f37892ae52b]
[fv-az695-456:71697] [ 8] plumed(+0x12f48)[0x56152e1f4f48]
[fv-az695-456:71697] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3788e29d90]
[fv-az695-456:71697] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3788e29e40]
[fv-az695-456:71697] [11] plumed(+0x131e5)[0x56152e1f51e5]
[fv-az695-456:71697] *** End of error message ***
</pre>
{% endraw %}
