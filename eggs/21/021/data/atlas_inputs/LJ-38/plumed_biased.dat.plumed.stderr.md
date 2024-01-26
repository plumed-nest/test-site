**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/LJ-38/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label n4 : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az979-741:06613] *** Process received signal ***
[fv-az979-741:06613] Signal: Aborted (6)
[fv-az979-741:06613] Signal code:  (-6)
[fv-az979-741:06613] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f168c642520]
[fv-az979-741:06613] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f168c6969fc]
[fv-az979-741:06613] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f168c642476]
[fv-az979-741:06613] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f168c6287f3]
[fv-az979-741:06613] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f168caa4f26]
[fv-az979-741:06613] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f168cab6d9c]
[fv-az979-741:06613] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f168cab6e07]
[fv-az979-741:06613] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f168cab70bb]
[fv-az979-741:06613] [ 8] plumed(+0x12f48)[0x55fbf46eef48]
[fv-az979-741:06613] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f168c629d90]
[fv-az979-741:06613] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f168c629e40]
[fv-az979-741:06613] [11] plumed(+0x131e5)[0x55fbf46ef1e5]
[fv-az979-741:06613] *** End of error message ***
</pre>
{% endraw %}
