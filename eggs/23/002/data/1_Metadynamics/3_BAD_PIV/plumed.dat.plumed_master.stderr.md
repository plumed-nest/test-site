**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/3_BAD_PIV/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[fv-az774-16:70429] *** Process received signal ***
[fv-az774-16:70429] Signal: Aborted (6)
[fv-az774-16:70429] Signal code:  (-6)
[fv-az774-16:70429] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb9e4a42520]
[fv-az774-16:70429] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb9e4a969fc]
[fv-az774-16:70429] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb9e4a42476]
[fv-az774-16:70429] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb9e4a287f3]
[fv-az774-16:70429] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb9e4ea2b9e]
[fv-az774-16:70429] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb9e4eae20c]
[fv-az774-16:70429] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb9e4eae277]
[fv-az774-16:70429] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb9e4eae52b]
[fv-az774-16:70429] [ 8] plumed_master(+0x14274)[0x55a08d8a2274]
[fv-az774-16:70429] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb9e4a29d90]
[fv-az774-16:70429] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb9e4a29e40]
[fv-az774-16:70429] [11] plumed_master(+0x14ed5)[0x55a08d8a2ed5]
[fv-az774-16:70429] *** End of error message ***
</pre>
{% endraw %}
