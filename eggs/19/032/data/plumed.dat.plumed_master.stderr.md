**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action PDB2CONSTANT with label @s1259 : argument O1O_lessthan was not set in pdb input
[fv-az1445-962:75438] *** Process received signal ***
[fv-az1445-962:75438] Signal: Aborted (6)
[fv-az1445-962:75438] Signal code:  (-6)
[fv-az1445-962:75438] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6a16642520]
[fv-az1445-962:75438] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6a166969fc]
[fv-az1445-962:75438] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6a16642476]
[fv-az1445-962:75438] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6a166287f3]
[fv-az1445-962:75438] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6a16aa2b9e]
[fv-az1445-962:75438] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6a16aae20c]
[fv-az1445-962:75438] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6a16aae277]
[fv-az1445-962:75438] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6a16aae52b]
[fv-az1445-962:75438] [ 8] plumed_master(+0x14274)[0x555621ffa274]
[fv-az1445-962:75438] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6a16629d90]
[fv-az1445-962:75438] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6a16629e40]
[fv-az1445-962:75438] [11] plumed_master(+0x14ed5)[0x555621ffaed5]
[fv-az1445-962:75438] *** End of error message ***
</pre>
{% endraw %}
