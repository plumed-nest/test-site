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
[fv-az2031-223:44053] *** Process received signal ***
[fv-az2031-223:44053] Signal: Aborted (6)
[fv-az2031-223:44053] Signal code:  (-6)
[fv-az2031-223:44053] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f83fc442520]
[fv-az2031-223:44053] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f83fc4969fc]
[fv-az2031-223:44053] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f83fc442476]
[fv-az2031-223:44053] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f83fc4287f3]
[fv-az2031-223:44053] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f83fc8a2b9e]
[fv-az2031-223:44053] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f83fc8ae20c]
[fv-az2031-223:44053] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f83fc8ae277]
[fv-az2031-223:44053] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f83fc8ae52b]
[fv-az2031-223:44053] [ 8] plumed(+0x12f48)[0x55bf36e74f48]
[fv-az2031-223:44053] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f83fc429d90]
[fv-az2031-223:44053] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f83fc429e40]
[fv-az2031-223:44053] [11] plumed(+0x131e5)[0x55bf36e751e5]
[fv-az2031-223:44053] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az2031-223:44052] *** Process received signal ***
[fv-az2031-223:44052] Signal: Aborted (6)
[fv-az2031-223:44052] Signal code:  (-6)
[fv-az2031-223:44052] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0071e42520]
[fv-az2031-223:44052] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0071e969fc]
[fv-az2031-223:44052] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0071e42476]
[fv-az2031-223:44052] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0071e287f3]
[fv-az2031-223:44052] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f00722a2b9e]
[fv-az2031-223:44052] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f00722ae20c]
[fv-az2031-223:44052] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f00722ae277]
[fv-az2031-223:44052] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f00722ae52b]
[fv-az2031-223:44052] [ 8] plumed(+0x12f48)[0x559f760cff48]
[fv-az2031-223:44052] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0071e29d90]
[fv-az2031-223:44052] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0071e29e40]
[fv-az2031-223:44052] [11] plumed(+0x131e5)[0x559f760d01e5]
[fv-az2031-223:44052] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az2031-223 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
