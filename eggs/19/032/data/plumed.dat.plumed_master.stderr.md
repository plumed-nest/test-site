**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action PDB2CONSTANT with label @s1259 : argument O1O_lessthan was not set in pdb input
[fv-az2031-223:45207] *** Process received signal ***
[fv-az2031-223:45207] Signal: Aborted (6)
[fv-az2031-223:45207] Signal code:  (-6)
[fv-az2031-223:45207] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f090da42520]
[fv-az2031-223:45207] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f090da969fc]
[fv-az2031-223:45207] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f090da42476]
[fv-az2031-223:45207] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f090da287f3]
[fv-az2031-223:45207] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f090dea2b9e]
[fv-az2031-223:45207] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f090deae20c]
[fv-az2031-223:45207] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f090deae277]
[fv-az2031-223:45207] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f090deae52b]
[fv-az2031-223:45207] [ 8] plumed_master(+0x14274)[0x557506d4c274]
[fv-az2031-223:45207] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f090da29d90]
[fv-az2031-223:45207] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f090da29e40]
[fv-az2031-223:45207] [11] plumed_master(+0x14ed5)[0x557506d4ced5]
[fv-az2031-223:45207] *** End of error message ***
</pre>
{% endraw %}
