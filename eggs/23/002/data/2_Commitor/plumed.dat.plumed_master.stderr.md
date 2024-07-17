**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  2_Commitor/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[fv-az774-16:70491] *** Process received signal ***
[fv-az774-16:70491] Signal: Aborted (6)
[fv-az774-16:70491] Signal code:  (-6)
[fv-az774-16:70491] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd08f042520]
[fv-az774-16:70491] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd08f0969fc]
[fv-az774-16:70491] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd08f042476]
[fv-az774-16:70491] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd08f0287f3]
[fv-az774-16:70491] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd08f4a2b9e]
[fv-az774-16:70491] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd08f4ae20c]
[fv-az774-16:70491] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd08f4ae277]
[fv-az774-16:70491] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd08f4ae52b]
[fv-az774-16:70491] [ 8] plumed_master(+0x14274)[0x5557eebf1274]
[fv-az774-16:70491] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd08f029d90]
[fv-az774-16:70491] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd08f029e40]
[fv-az774-16:70491] [11] plumed_master(+0x14ed5)[0x5557eebf1ed5]
[fv-az774-16:70491] *** End of error message ***
</pre>
{% endraw %}
