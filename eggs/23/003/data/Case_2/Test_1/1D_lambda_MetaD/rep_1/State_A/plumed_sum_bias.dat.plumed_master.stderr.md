**Project ID:** [plumID:23.003]({{ '/' | absolute_url }}eggs/23/003/)  
Stderr for source:  Case_2/Test_1/1D_lambda_MetaD/rep_1/State_A/plumed_sum_bias.dat   
Download: [zipped raw stdout](plumed_sum_bias.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_sum_bias.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS_1D_modified_fake not found
[fv-az979-741:05033] *** Process received signal ***
[fv-az979-741:05033] Signal: Aborted (6)
[fv-az979-741:05033] Signal code:  (-6)
[fv-az979-741:05033] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7049a42520]
[fv-az979-741:05033] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7049a969fc]
[fv-az979-741:05033] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7049a42476]
[fv-az979-741:05033] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7049a287f3]
[fv-az979-741:05033] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7049ea4f26]
[fv-az979-741:05033] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7049eb6d9c]
[fv-az979-741:05033] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7049eb6e07]
[fv-az979-741:05033] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7049eb70bb]
[fv-az979-741:05033] [ 8] plumed_master(+0x12ebf)[0x559a8da73ebf]
[fv-az979-741:05033] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7049a29d90]
[fv-az979-741:05033] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7049a29e40]
[fv-az979-741:05033] [11] plumed_master(+0x13155)[0x559a8da74155]
[fv-az979-741:05033] *** End of error message ***
</pre>
{% endraw %}
