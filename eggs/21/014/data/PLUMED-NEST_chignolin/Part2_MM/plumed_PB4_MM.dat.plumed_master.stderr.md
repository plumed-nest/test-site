**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
Stderr for source:  PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat   
Download: [zipped raw stdout](plumed_PB4_MM.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_PB4_MM.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
[fv-az1542-52:07774] *** Process received signal ***
[fv-az1542-52:07774] Signal: Aborted (6)
[fv-az1542-52:07774] Signal code:  (-6)
[fv-az1542-52:07774] [ 0]   what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
[fv-az1542-52:07773] *** Process received signal ***
[fv-az1542-52:07773] Signal: Aborted (6)
[fv-az1542-52:07773] Signal code:  (-6)
[fv-az1542-52:07773] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4d56442520]
[fv-az1542-52:07774] [ 1] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe53e842520]
[fv-az1542-52:07773] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4d564969fc]
[fv-az1542-52:07774] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4d56442476]
[fv-az1542-52:07774] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4d564287f3]
[fv-az1542-52:07774] [ 4] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe53e8969fc]
[fv-az1542-52:07773] [ 2] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f4d568a4f26]
[fv-az1542-52:07774] [ 5] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe53e842476]
[fv-az1542-52:07773] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe53e8287f3]
[fv-az1542-52:07773] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f4d568b6d9c]
[fv-az1542-52:07774] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f4d568b6e07]
[fv-az1542-52:07774] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe53eca4f26]
[fv-az1542-52:07773] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4d568b70bb]
[fv-az1542-52:07774] [ 8] plumed_master(+0x12ebf)[0x5643d7445ebf]
[fv-az1542-52:07774] [ 9] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe53ecb6d9c]
[fv-az1542-52:07773] [ 6] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4d56429d90]
[fv-az1542-52:07774] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4d56429e40]
[fv-az1542-52:07774] [11] plumed_master(+0x13155)[0x5643d7446155]
[fv-az1542-52:07774] *** End of error message ***
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe53ecb6e07]
[fv-az1542-52:07773] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe53ecb70bb]
[fv-az1542-52:07773] [ 8] plumed_master(+0x12ebf)[0x55a917640ebf]
[fv-az1542-52:07773] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe53e829d90]
[fv-az1542-52:07773] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe53e829e40]
[fv-az1542-52:07773] [11] plumed_master(+0x13155)[0x55a917641155]
[fv-az1542-52:07773] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1542-52 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
