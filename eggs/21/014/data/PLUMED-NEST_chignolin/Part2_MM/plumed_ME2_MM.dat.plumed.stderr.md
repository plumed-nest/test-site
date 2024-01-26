**Project ID:** [plumID:21.014]({{ '/' | absolute_url }}eggs/21/014/)  
Stderr for source:  PLUMED-NEST_chignolin/Part2_MM/plumed_ME2_MM.dat   
Download: [zipped raw stdout](plumed_ME2_MM.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ME2_MM.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():  terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100

(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=100
[fv-az1542-52:07719] *** Process received signal ***
[fv-az1542-52:07719] Signal: Aborted (6)
[fv-az1542-52:07719] Signal code:  (-6)
[fv-az1542-52:07718] *** Process received signal ***
[fv-az1542-52:07718] Signal: Aborted (6)
[fv-az1542-52:07718] Signal code:  (-6)
[fv-az1542-52:07718] [ 0] [fv-az1542-52:07719] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7b4c242520]
[fv-az1542-52:07718] [ 1] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f13a1642520]
[fv-az1542-52:07719] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7b4c2969fc]
[fv-az1542-52:07718] [ 2] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f13a16969fc]
[fv-az1542-52:07719] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7b4c242476]
[fv-az1542-52:07718] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7b4c2287f3]
[fv-az1542-52:07718] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f13a1642476]
[fv-az1542-52:07719] [ 3] [ 4] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f13a16287f3]
[fv-az1542-52:07719] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7b4c6a4f26]
[fv-az1542-52:07718] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f13a1aa4f26]
[fv-az1542-52:07719] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7b4c6b6d9c]
[fv-az1542-52:07718] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7b4c6b6e07]
[fv-az1542-52:07718] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7b4c6b70bb]
[fv-az1542-52:07718] [ 8] plumed(+0x12f48)[0x555bfdea9f48]
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f13a1ab6d9c]
[fv-az1542-52:07719] [ 6] [fv-az1542-52:07718] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7b4c229d90]
[fv-az1542-52:07718] [10] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f13a1ab6e07]
[fv-az1542-52:07719] [ 7] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7b4c229e40]
[fv-az1542-52:07718] [11] plumed(+0x131e5)[0x555bfdeaa1e5]
[fv-az1542-52:07718] *** End of error message ***
/lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f13a1ab70bb]
[fv-az1542-52:07719] [ 8] plumed(+0x12f48)[0x55a0573ccf48]
[fv-az1542-52:07719] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f13a1629d90]
[fv-az1542-52:07719] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f13a1629e40]
[fv-az1542-52:07719] [11] plumed(+0x131e5)[0x55a0573cd1e5]
[fv-az1542-52:07719] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1542-52 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
