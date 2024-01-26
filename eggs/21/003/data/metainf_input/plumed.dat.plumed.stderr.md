**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1148-6:08981] *** Process received signal ***
[fv-az1148-6:08981] Signal: Aborted (6)
[fv-az1148-6:08981] Signal code:  (-6)
[fv-az1148-6:08981] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6953242520]
[fv-az1148-6:08981] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f69532969fc]
[fv-az1148-6:08981] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6953242476]
[fv-az1148-6:08981] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f69532287f3]
[fv-az1148-6:08981] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f69536a4f26]
[fv-az1148-6:08981] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f69536b6d9c]
[fv-az1148-6:08981] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f69536b6e07]
[fv-az1148-6:08981] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f69536b70bb]
[fv-az1148-6:08981] [ 8] plumed(+0x12f48)[0x558fbba35f48]
[fv-az1148-6:08981] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6953229d90]
[fv-az1148-6:08981] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6953229e40]
[fv-az1148-6:08981] [11] plumed(+0x131e5)[0x558fbba361e5]
[fv-az1148-6:08981] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[fv-az1148-6:08982] *** Process received signal ***
[fv-az1148-6:08982] Signal: Aborted (6)
[fv-az1148-6:08982] Signal code:  (-6)
[fv-az1148-6:08982] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb3ea442520]
[fv-az1148-6:08982] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb3ea4969fc]
[fv-az1148-6:08982] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb3ea442476]
[fv-az1148-6:08982] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb3ea4287f3]
[fv-az1148-6:08982] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fb3ea8a4f26]
[fv-az1148-6:08982] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fb3ea8b6d9c]
[fv-az1148-6:08982] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fb3ea8b6e07]
[fv-az1148-6:08982] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb3ea8b70bb]
[fv-az1148-6:08982] [ 8] plumed(+0x12f48)[0x55b74bed0f48]
[fv-az1148-6:08982] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb3ea429d90]
[fv-az1148-6:08982] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb3ea429e40]
[fv-az1148-6:08982] [11] plumed(+0x131e5)[0x55b74bed11e5]
[fv-az1148-6:08982] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1148-6 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
