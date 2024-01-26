**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
Stderr for source:  PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat   
Download: [zipped raw stdout](plumed_ME2_MM.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ME2_MM.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():  terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100

(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
[fv-az1542-52:07731] *** Process received signal ***
[fv-az1542-52:07731] Signal: Aborted (6)
[fv-az1542-52:07731] Signal code:  (-6)
[fv-az1542-52:07731] [ 0] [fv-az1542-52:07730] *** Process received signal ***
[fv-az1542-52:07730] Signal: Aborted (6)
[fv-az1542-52:07730] Signal code:  (-6)
[fv-az1542-52:07730] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f92b7242520]
[fv-az1542-52:07731] [ 1] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe7a3e42520]
[fv-az1542-52:07730] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f92b72969fc]
[fv-az1542-52:07731] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f92b7242476]
[fv-az1542-52:07731] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f92b72287f3]
/lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe7a3e969fc]
[fv-az1542-52:07730] [ 2] [fv-az1542-52:07731] [ 4] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe7a3e42476]
[fv-az1542-52:07730] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f92b76a4f26]
[fv-az1542-52:07731] [ 5] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe7a3e287f3]
[fv-az1542-52:07730] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f92b76b6d9c]
[fv-az1542-52:07731] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe7a42a4f26]
[fv-az1542-52:07730] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f92b76b6e07]
[fv-az1542-52:07731] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f92b76b70bb]
[fv-az1542-52:07731] [ 8] plumed_master(+0x12ebf)[0x5613668c9ebf]
[fv-az1542-52:07731] [ 9] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe7a42b6d9c]
[fv-az1542-52:07730] [ 6] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f92b7229d90]
[fv-az1542-52:07731] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f92b7229e40]
[fv-az1542-52:07731] [11] plumed_master(+0x13155)[0x5613668ca155]
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe7a42b6e07]
[fv-az1542-52:07730] [ 7] [fv-az1542-52:07731] *** End of error message ***
/lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe7a42b70bb]
[fv-az1542-52:07730] [ 8] plumed_master(+0x12ebf)[0x55912187eebf]
[fv-az1542-52:07730] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe7a3e29d90]
[fv-az1542-52:07730] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe7a3e29e40]
[fv-az1542-52:07730] [11] plumed_master(+0x13155)[0x55912187f155]
[fv-az1542-52:07730] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1542-52 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
