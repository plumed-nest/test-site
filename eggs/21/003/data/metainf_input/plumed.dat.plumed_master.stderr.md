**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1445-962:74309] *** Process received signal ***
[fv-az1445-962:74309] Signal: Aborted (6)
[fv-az1445-962:74309] Signal code:  (-6)
[fv-az1445-962:74309] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f97c3c42520]
[fv-az1445-962:74309] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f97c3c969fc]
[fv-az1445-962:74309] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f97c3c42476]
[fv-az1445-962:74309] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f97c3c287f3]
[fv-az1445-962:74309] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f97c40a2b9e]
[fv-az1445-962:74309] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f97c40ae20c]
[fv-az1445-962:74309] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f97c40ae277]
[fv-az1445-962:74309] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f97c40ae52b]
[fv-az1445-962:74309] [ 8] plumed_master(+0x14274)[0x55f492fee274]
[fv-az1445-962:74309] [ 9] terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
/lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f97c3c29d90]
[fv-az1445-962:74309] [10] [fv-az1445-962:74310] *** Process received signal ***
[fv-az1445-962:74310] Signal: Aborted (6)
[fv-az1445-962:74310] Signal code:  (-6)
[fv-az1445-962:74310] [ 0] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f97c3c29e40]
[fv-az1445-962:74309] [11] plumed_master(+0x14ed5)[0x55f492feeed5]
[fv-az1445-962:74309] *** End of error message ***
/lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe897842520]
[fv-az1445-962:74310] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe8978969fc]
[fv-az1445-962:74310] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe897842476]
[fv-az1445-962:74310] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe8978287f3]
[fv-az1445-962:74310] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe897ca2b9e]
[fv-az1445-962:74310] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe897cae20c]
[fv-az1445-962:74310] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe897cae277]
[fv-az1445-962:74310] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe897cae52b]
[fv-az1445-962:74310] [ 8] plumed_master(+0x14274)[0x55bcc9d5a274]
[fv-az1445-962:74310] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe897829d90]
[fv-az1445-962:74310] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe897829e40]
[fv-az1445-962:74310] [11] plumed_master(+0x14ed5)[0x55bcc9d5aed5]
[fv-az1445-962:74310] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az1445-962 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
