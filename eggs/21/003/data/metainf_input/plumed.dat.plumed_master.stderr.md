**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az2031-223:44065] *** Process received signal ***
[fv-az2031-223:44065] Signal: Aborted (6)
[fv-az2031-223:44065] Signal code:  (-6)
[fv-az2031-223:44065] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7e3f642520]
[fv-az2031-223:44065] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7e3f6969fc]
[fv-az2031-223:44065] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7e3f642476]
[fv-az2031-223:44065] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7e3f6287f3]
[fv-az2031-223:44065] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7e3faa2b9e]
[fv-az2031-223:44065] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7e3faae20c]
[fv-az2031-223:44065] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7e3faae277]
[fv-az2031-223:44065] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7e3faae52b]
[fv-az2031-223:44065] [ 8] plumed_master(+0x14274)[0x55caa2523274]
[fv-az2031-223:44065] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7e3f629d90]
[fv-az2031-223:44065] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7e3f629e40]
[fv-az2031-223:44065] [11] plumed_master(+0x14ed5)[0x55caa2523ed5]
[fv-az2031-223:44065] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az2031-223:44064] *** Process received signal ***
[fv-az2031-223:44064] Signal: Aborted (6)
[fv-az2031-223:44064] Signal code:  (-6)
[fv-az2031-223:44064] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f65cae42520]
[fv-az2031-223:44064] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f65cae969fc]
[fv-az2031-223:44064] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f65cae42476]
[fv-az2031-223:44064] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f65cae287f3]
[fv-az2031-223:44064] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f65cb2a2b9e]
[fv-az2031-223:44064] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f65cb2ae20c]
[fv-az2031-223:44064] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f65cb2ae277]
[fv-az2031-223:44064] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f65cb2ae52b]
[fv-az2031-223:44064] [ 8] plumed_master(+0x14274)[0x564d54629274]
[fv-az2031-223:44064] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f65cae29d90]
[fv-az2031-223:44064] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f65cae29e40]
[fv-az2031-223:44064] [11] plumed_master(+0x14ed5)[0x564d54629ed5]
[fv-az2031-223:44064] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az2031-223 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
