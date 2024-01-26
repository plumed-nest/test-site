**Project ID:** [plumID:19.057]({{ '/' | absolute_url }}eggs/19/057/)  
Stderr for source:  plumed-main.dat   
Download: [zipped raw stdout](plumed-main.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-main.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsdata : cannot understand the following words from the input line : SCALEINT=66
[fv-az1200-577:10018] *** Process received signal ***
[fv-az1200-577:10018] Signal: Aborted (6)
[fv-az1200-577:10018] Signal code:  (-6)
[fv-az1200-577:10018] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe7dd642520]
[fv-az1200-577:10018] [ 1] terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxsdata : cannot understand the following words from the input line : SCALEINT=66
/lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe7dd6969fc]
[fv-az1200-577:10018] [ 2] [fv-az1200-577:10019] *** Process received signal ***
[fv-az1200-577:10019] Signal: Aborted (6)
[fv-az1200-577:10019] Signal code:  (-6)
[fv-az1200-577:10019] [ 0] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe7dd642476]
[fv-az1200-577:10018] [ 3] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbe16642520]
[fv-az1200-577:10019] [ 1] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe7dd6287f3]
[fv-az1200-577:10018] [ 4] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbe166969fc]
[fv-az1200-577:10019] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbe16642476]
[fv-az1200-577:10019] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe7ddaa4f26]
[fv-az1200-577:10018] [ 5] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbe166287f3]
[fv-az1200-577:10019] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe7ddab6d9c]
[fv-az1200-577:10018] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fbe16aa4f26]
[fv-az1200-577:10019] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fbe16ab6d9c]
[fv-az1200-577:10019] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe7ddab6e07]
[fv-az1200-577:10018] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fbe16ab6e07]
[fv-az1200-577:10019] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe7ddab70bb]
[fv-az1200-577:10018] [ 8] plumed(+0x12f48)[0x56046b823f48]
[fv-az1200-577:10018] [ 9] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbe16ab70bb]
[fv-az1200-577:10019] [ 8] plumed(+0x12f48)[0x5607cdeadf48]
[fv-az1200-577:10019] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbe16629d90]
[fv-az1200-577:10019] [10] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe7dd629d90]
[fv-az1200-577:10018] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbe16629e40]
[fv-az1200-577:10019] [11] plumed(+0x131e5)[0x5607cdeae1e5]
[fv-az1200-577:10019] *** End of error message ***
/lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe7dd629e40]
[fv-az1200-577:10018] [11] plumed(+0x131e5)[0x56046b8241e5]
[fv-az1200-577:10018] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1200-577 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
