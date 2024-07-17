**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat   
Download: [zipped raw stdout](plumed.order.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az695-456:71758] *** Process received signal ***
[fv-az695-456:71758] Signal: Aborted (6)
[fv-az695-456:71758] Signal code:  (-6)
[fv-az695-456:71758] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7eff6c442520]
[fv-az695-456:71758] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7eff6c4969fc]
[fv-az695-456:71758] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7eff6c442476]
[fv-az695-456:71758] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7eff6c4287f3]
[fv-az695-456:71758] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7eff6c8a2b9e]
[fv-az695-456:71758] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7eff6c8ae20c]
[fv-az695-456:71758] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7eff6c8ae277]
[fv-az695-456:71758] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7eff6c8ae52b]
[fv-az695-456:71758] [ 8] plumed(+0x12f48)[0x55ddcc6aff48]
[fv-az695-456:71758] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7eff6c429d90]
[fv-az695-456:71758] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7eff6c429e40]
[fv-az695-456:71758] [11] plumed(+0x131e5)[0x55ddcc6b01e5]
[fv-az695-456:71758] *** End of error message ***
</pre>
{% endraw %}
