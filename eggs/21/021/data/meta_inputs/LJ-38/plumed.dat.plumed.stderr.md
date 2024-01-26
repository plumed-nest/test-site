**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  meta_inputs/LJ-38/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az979-741:06968] *** Process received signal ***
[fv-az979-741:06968] Signal: Aborted (6)
[fv-az979-741:06968] Signal code:  (-6)
[fv-az979-741:06968] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5888a42520]
[fv-az979-741:06968] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5888a969fc]
[fv-az979-741:06968] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5888a42476]
[fv-az979-741:06968] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5888a287f3]
[fv-az979-741:06968] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f5888ea4f26]
[fv-az979-741:06968] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f5888eb6d9c]
[fv-az979-741:06968] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f5888eb6e07]
[fv-az979-741:06968] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5888eb70bb]
[fv-az979-741:06968] [ 8] plumed(+0x12f48)[0x55dc874f6f48]
[fv-az979-741:06968] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5888a29d90]
[fv-az979-741:06968] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5888a29e40]
[fv-az979-741:06968] [11] plumed(+0x131e5)[0x55dc874f71e5]
[fv-az979-741:06968] *** End of error message ***
</pre>
{% endraw %}
