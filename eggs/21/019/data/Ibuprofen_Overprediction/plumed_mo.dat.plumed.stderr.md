**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_mo.dat   
Download: [zipped raw stdout](plumed_mo.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label @0 : Number of specified atoms should be 2
[fv-az695-456:74636] *** Process received signal ***
[fv-az695-456:74636] Signal: Aborted (6)
[fv-az695-456:74636] Signal code:  (-6)
[fv-az695-456:74636] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9c12e42520]
[fv-az695-456:74636] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9c12e969fc]
[fv-az695-456:74636] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9c12e42476]
[fv-az695-456:74636] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9c12e287f3]
[fv-az695-456:74636] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f9c132a2b9e]
[fv-az695-456:74636] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f9c132ae20c]
[fv-az695-456:74636] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f9c132ae277]
[fv-az695-456:74636] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9c132ae52b]
[fv-az695-456:74636] [ 8] plumed(+0x12f48)[0x55a0888a8f48]
[fv-az695-456:74636] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9c12e29d90]
[fv-az695-456:74636] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9c12e29e40]
[fv-az695-456:74636] [11] plumed(+0x131e5)[0x55a0888a91e5]
[fv-az695-456:74636] *** End of error message ***
</pre>
{% endraw %}
