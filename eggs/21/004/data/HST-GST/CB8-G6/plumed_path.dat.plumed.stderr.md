**Project ID:** [plumID:21.004]({{ '/' | absolute_url }}eggs/21/004/)  
Stderr for source:  HST-GST/CB8-G6/plumed_path.dat   
Download: [zipped raw stdout](plumed_path.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_path.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : restart file HILLS not found
[fv-az1542-52:07835] *** Process received signal ***
[fv-az1542-52:07835] Signal: Aborted (6)
[fv-az1542-52:07835] Signal code:  (-6)
[fv-az1542-52:07835] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f767fa42520]
[fv-az1542-52:07835] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f767fa969fc]
[fv-az1542-52:07835] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f767fa42476]
[fv-az1542-52:07835] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f767fa287f3]
[fv-az1542-52:07835] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f767fea4f26]
[fv-az1542-52:07835] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f767feb6d9c]
[fv-az1542-52:07835] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f767feb6e07]
[fv-az1542-52:07835] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f767feb70bb]
[fv-az1542-52:07835] [ 8] plumed(+0x12f48)[0x55fec4c3bf48]
[fv-az1542-52:07835] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f767fa29d90]
[fv-az1542-52:07835] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f767fa29e40]
[fv-az1542-52:07835] [11] plumed(+0x131e5)[0x55fec4c3c1e5]
[fv-az1542-52:07835] *** End of error message ***
</pre>
{% endraw %}
