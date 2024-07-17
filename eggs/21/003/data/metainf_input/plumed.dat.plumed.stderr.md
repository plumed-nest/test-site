**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1445-962:74298] *** Process received signal ***
[fv-az1445-962:74298] Signal: Aborted (6)
[fv-az1445-962:74298] Signal code:  (-6)
[fv-az1445-962:74298] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fca55042520]
[fv-az1445-962:74298] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fca550969fc]
[fv-az1445-962:74298] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fca55042476]
[fv-az1445-962:74298] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fca550287f3]
[fv-az1445-962:74298] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fca554a2b9e]
[fv-az1445-962:74298] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fca554ae20c]
[fv-az1445-962:74298] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fca554ae277]
[fv-az1445-962:74298] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fca554ae52b]
[fv-az1445-962:74298] [ 8] plumed(+0x12f48)[0x55591355bf48]
[fv-az1445-962:74298] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fca55029d90]
[fv-az1445-962:74298] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fca55029e40]
[fv-az1445-962:74298] [11] plumed(+0x131e5)[0x55591355c1e5]
[fv-az1445-962:74298] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1445-962:74297] *** Process received signal ***
[fv-az1445-962:74297] Signal: Aborted (6)
[fv-az1445-962:74297] Signal code:  (-6)
[fv-az1445-962:74297] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8b74242520]
[fv-az1445-962:74297] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8b742969fc]
[fv-az1445-962:74297] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8b74242476]
[fv-az1445-962:74297] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8b742287f3]
[fv-az1445-962:74297] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8b746a2b9e]
[fv-az1445-962:74297] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8b746ae20c]
[fv-az1445-962:74297] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8b746ae277]
[fv-az1445-962:74297] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8b746ae52b]
[fv-az1445-962:74297] [ 8] plumed(+0x12f48)[0x55d57e21ff48]
[fv-az1445-962:74297] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8b74229d90]
[fv-az1445-962:74297] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8b74229e40]
[fv-az1445-962:74297] [11] plumed(+0x131e5)[0x55d57e2201e5]
[fv-az1445-962:74297] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1445-962 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
