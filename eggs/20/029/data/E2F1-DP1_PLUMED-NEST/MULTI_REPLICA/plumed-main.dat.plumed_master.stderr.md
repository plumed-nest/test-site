**Project ID:** [plumID:20.029]({{ '/' | absolute_url }}eggs/20/029/)  
Stderr for source:  E2F1-DP1_PLUMED-NEST/MULTI_REPLICA/plumed-main.dat   
Download: [zipped raw stdout](plumed-main.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-main.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsCG : cannot understand the following words from the input line : SCALEINT=107.069000
[fv-az1542-52:07895] *** Process received signal ***
[fv-az1542-52:07895] Signal: Aborted (6)
[fv-az1542-52:07895] Signal code:  (-6)
[fv-az1542-52:07895] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb437842520]
[fv-az1542-52:07895] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb4378969fc]
[fv-az1542-52:07895] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb437842476]
[fv-az1542-52:07895] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb4378287f3]
[fv-az1542-52:07895] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb437ca4f26]
[fv-az1542-52:07895] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb437cb6d9c]
[fv-az1542-52:07895] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb437cb6e07]
[fv-az1542-52:07895] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb437cb70bb]
[fv-az1542-52:07895] [ 8] plumed_master(+0x12ebf)[0x55bb5bedfebf]
[fv-az1542-52:07895] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb437829d90]
[fv-az1542-52:07895] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb437829e40]
[fv-az1542-52:07895] [11] plumed_master(+0x13155)[0x55bb5bee0155]
[fv-az1542-52:07895] *** End of error message ***
</pre>
{% endraw %}
