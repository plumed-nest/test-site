**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1148-6:08994] *** Process received signal ***
[fv-az1148-6:08994] Signal: Aborted (6)
[fv-az1148-6:08994] Signal code:  (-6)
[fv-az1148-6:08994] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5cd9e42520]
[fv-az1148-6:08994] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5cd9e969fc]
[fv-az1148-6:08994] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5cd9e42476]
[fv-az1148-6:08994] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5cd9e287f3]
[fv-az1148-6:08994] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f5cda2a4f26]
[fv-az1148-6:08994] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f5cda2b6d9c]
[fv-az1148-6:08994] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f5cda2b6e07]
[fv-az1148-6:08994] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5cda2b70bb]
[fv-az1148-6:08994] [ 8] plumed_master(+0x12ebf)[0x56403534bebf]
[fv-az1148-6:08994] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5cd9e29d90]
[fv-az1148-6:08994] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5cd9e29e40]
[fv-az1148-6:08994] [11] plumed_master(+0x13155)[0x56403534c155]
[fv-az1148-6:08994] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1148-6:08993] *** Process received signal ***
[fv-az1148-6:08993] Signal: Aborted (6)
[fv-az1148-6:08993] Signal code:  (-6)
[fv-az1148-6:08993] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fec1ba42520]
[fv-az1148-6:08993] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fec1ba969fc]
[fv-az1148-6:08993] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fec1ba42476]
[fv-az1148-6:08993] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fec1ba287f3]
[fv-az1148-6:08993] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fec1bea4f26]
[fv-az1148-6:08993] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fec1beb6d9c]
[fv-az1148-6:08993] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fec1beb6e07]
[fv-az1148-6:08993] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fec1beb70bb]
[fv-az1148-6:08993] [ 8] plumed_master(+0x12ebf)[0x55d8027e6ebf]
[fv-az1148-6:08993] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fec1ba29d90]
[fv-az1148-6:08993] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fec1ba29e40]
[fv-az1148-6:08993] [11] plumed_master(+0x13155)[0x55d8027e7155]
[fv-az1148-6:08993] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1148-6 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
