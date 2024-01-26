**Project ID:** [plumID:21.004]({{ '/' | absolute_url }}eggs/21/004/)  
Stderr for source:  GSK/3/plumed_path.dat   
Download: [zipped raw stdout](plumed_path.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_path.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1542-52:07803] *** Process received signal ***
[fv-az1542-52:07803] Signal: Aborted (6)
[fv-az1542-52:07803] Signal code:  (-6)
[fv-az1542-52:07803] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffa30642520]
[fv-az1542-52:07803] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffa306969fc]
[fv-az1542-52:07803] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffa30642476]
[fv-az1542-52:07803] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffa306287f3]
[fv-az1542-52:07803] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ffa30aa4f26]
[fv-az1542-52:07803] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ffa30ab6d9c]
[fv-az1542-52:07803] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ffa30ab6e07]
[fv-az1542-52:07803] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffa30ab70bb]
[fv-az1542-52:07803] [ 8] plumed(+0x12f48)[0x561ba70a4f48]
[fv-az1542-52:07803] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffa30629d90]
[fv-az1542-52:07803] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffa30629e40]
[fv-az1542-52:07803] [11] plumed(+0x131e5)[0x561ba70a51e5]
[fv-az1542-52:07803] *** End of error message ***
</pre>
{% endraw %}
