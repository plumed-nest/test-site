**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1436-30:10553] *** Process received signal ***
[fv-az1436-30:10553] Signal: Aborted (6)
[fv-az1436-30:10553] Signal code:  (-6)
[fv-az1436-30:10553] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efcc5e45330]
[fv-az1436-30:10553] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efcc5e9eb2c]
[fv-az1436-30:10553] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efcc5e4527e]
[fv-az1436-30:10553] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efcc5e288ff]
[fv-az1436-30:10553] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efcc62a5ff5]
[fv-az1436-30:10553] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efcc62bb0da]
[fv-az1436-30:10553] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efcc62a5a55]
[fv-az1436-30:10553] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efcc62a5a6f]
[fv-az1436-30:10553] [ 8] plumed(+0x146dd)[0x558d513716dd]
[fv-az1436-30:10553] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efcc5e2a1ca]
[fv-az1436-30:10553] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efcc5e2a28b]
[fv-az1436-30:10553] [11] plumed(+0x15365)[0x558d51372365]
[fv-az1436-30:10553] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1436-30:10554] *** Process received signal ***
[fv-az1436-30:10554] Signal: Aborted (6)
[fv-az1436-30:10554] Signal code:  (-6)
[fv-az1436-30:10554] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f684a845330]
[fv-az1436-30:10554] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f684a89eb2c]
[fv-az1436-30:10554] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f684a84527e]
[fv-az1436-30:10554] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f684a8288ff]
[fv-az1436-30:10554] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f684aca5ff5]
[fv-az1436-30:10554] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f684acbb0da]
[fv-az1436-30:10554] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f684aca5a55]
[fv-az1436-30:10554] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f684aca5a6f]
[fv-az1436-30:10554] [ 8] plumed(+0x146dd)[0x5594f040a6dd]
[fv-az1436-30:10554] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f684a82a1ca]
[fv-az1436-30:10554] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f684a82a28b]
[fv-az1436-30:10554] [11] plumed(+0x15365)[0x5594f040b365]
[fv-az1436-30:10554] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1436-30 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
