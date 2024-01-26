**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
Stderr for source:  PLUMED-NEST_chignolin/Part2_MM/plumed_PB4_MM.dat   
Download: [zipped raw stdout](plumed_PB4_MM.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_PB4_MM.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
[fv-az1542-52:07759] *** Process received signal ***
[fv-az1542-52:07759] Signal: Aborted (6)
[fv-az1542-52:07759] Signal code:  (-6)
[fv-az1542-52:07759] [ 0] terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
/lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc2f4042520]
[fv-az1542-52:07759]   what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
[ 1] [fv-az1542-52:07760] *** Process received signal ***
[fv-az1542-52:07760] Signal: Aborted (6)
[fv-az1542-52:07760] Signal code:  (-6)
[fv-az1542-52:07760] [ 0] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc2f40969fc]
[fv-az1542-52:07759] [ 2] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbad0e42520]
[fv-az1542-52:07760] [ 1] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc2f4042476]
[fv-az1542-52:07759] [ 3] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbad0e969fc]
[fv-az1542-52:07760] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc2f40287f3]
[fv-az1542-52:07759] [ 4] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbad0e42476]
[fv-az1542-52:07760] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbad0e287f3]
[fv-az1542-52:07760] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fc2f44a4f26]
[fv-az1542-52:07759] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fbad12a4f26]
[fv-az1542-52:07760] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fbad12b6d9c]
[fv-az1542-52:07760] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fc2f44b6d9c]
[fv-az1542-52:07759] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fbad12b6e07]
[fv-az1542-52:07760] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fc2f44b6e07]
[fv-az1542-52:07759] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbad12b70bb]
[fv-az1542-52:07760] [ 8] plumed(+0x12f48)[0x563da4803f48]
[fv-az1542-52:07760] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbad0e29d90]
[fv-az1542-52:07760] [10] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc2f44b70bb]
[fv-az1542-52:07759] [ 8] plumed(+0x12f48)[0x556d3b74ff48]
[fv-az1542-52:07759] [ 9] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbad0e29e40]
[fv-az1542-52:07760] [11] plumed(+0x131e5)[0x563da48041e5]
[fv-az1542-52:07760] *** End of error message ***
/lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc2f4029d90]
[fv-az1542-52:07759] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc2f4029e40]
[fv-az1542-52:07759] [11] plumed(+0x131e5)[0x556d3b7501e5]
[fv-az1542-52:07759] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1542-52 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
