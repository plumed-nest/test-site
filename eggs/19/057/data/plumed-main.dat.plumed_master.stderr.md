**Project ID:** [plumID:19.057]({{ '/' | absolute_url }}eggs/19/057/)  
Stderr for source:  plumed-main.dat   
Download: [zipped raw stdout](plumed-main.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-main.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsdata : cannot understand the following words from the input line : SCALEINT=66
[fv-az1200-577:10031] *** Process received signal ***
[fv-az1200-577:10031] Signal: Aborted (6)
[fv-az1200-577:10031] Signal code:  (-6)
[fv-az1200-577:10031] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9db2c42520]
[fv-az1200-577:10031] [ 1] terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsdata : cannot understand the following words from the input line : SCALEINT=66
/lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9db2c969fc]
[fv-az1200-577:10031] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9db2c42476]
[fv-az1200-577:10031] [ 3] [fv-az1200-577:10032] *** Process received signal ***
[fv-az1200-577:10032] Signal: Aborted (6)
[fv-az1200-577:10032] Signal code:  (-6)
[fv-az1200-577:10032] [ 0] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9db2c287f3]
[fv-az1200-577:10031] [ 4] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdd60042520]
[fv-az1200-577:10032] [ 1] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9db30a4f26]
[fv-az1200-577:10031] [ 5] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdd600969fc]
[fv-az1200-577:10032] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdd60042476]
[fv-az1200-577:10032] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdd600287f3]
[fv-az1200-577:10032] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9db30b6d9c]
[fv-az1200-577:10031] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fdd604a4f26]
[fv-az1200-577:10032] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9db30b6e07]
[fv-az1200-577:10031] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fdd604b6d9c]
[fv-az1200-577:10032] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9db30b70bb]
[fv-az1200-577:10031] [ 8] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fdd604b6e07]
[fv-az1200-577:10032] [ 7] plumed_master(+0x12ebf)[0x55f1aac40ebf]
[fv-az1200-577:10031] [ 9] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdd604b70bb]
[fv-az1200-577:10032] [ 8] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9db2c29d90]
[fv-az1200-577:10031] [10] plumed_master(+0x12ebf)[0x55900c533ebf]
[fv-az1200-577:10032] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdd60029d90]
[fv-az1200-577:10032] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9db2c29e40]
[fv-az1200-577:10031] [11] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdd60029e40]
[fv-az1200-577:10032] [11] plumed_master(+0x13155)[0x55900c534155]
[fv-az1200-577:10032] *** End of error message ***
plumed_master(+0x13155)[0x55f1aac41155]
[fv-az1200-577:10031] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1200-577 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
