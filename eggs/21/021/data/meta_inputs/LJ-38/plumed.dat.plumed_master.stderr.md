**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  meta_inputs/LJ-38/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az979-741:06976] *** Process received signal ***
[fv-az979-741:06976] Signal: Aborted (6)
[fv-az979-741:06976] Signal code:  (-6)
[fv-az979-741:06976] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f32a1242520]
[fv-az979-741:06976] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f32a12969fc]
[fv-az979-741:06976] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f32a1242476]
[fv-az979-741:06976] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f32a12287f3]
[fv-az979-741:06976] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f32a16a4f26]
[fv-az979-741:06976] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f32a16b6d9c]
[fv-az979-741:06976] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f32a16b6e07]
[fv-az979-741:06976] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f32a16b70bb]
[fv-az979-741:06976] [ 8] plumed_master(+0x12ebf)[0x5606c67e8ebf]
[fv-az979-741:06976] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f32a1229d90]
[fv-az979-741:06976] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f32a1229e40]
[fv-az979-741:06976] [11] plumed_master(+0x13155)[0x5606c67e9155]
[fv-az979-741:06976] *** End of error message ***
</pre>
{% endraw %}
