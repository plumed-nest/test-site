**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  meta_inputs/LJ-38/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az1543-369:41648] *** Process received signal ***
[fv-az1543-369:41648] Signal: Aborted (6)
[fv-az1543-369:41648] Signal code:  (-6)
[fv-az1543-369:41648] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffb40a42520]
[fv-az1543-369:41648] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffb40a969fc]
[fv-az1543-369:41648] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffb40a42476]
[fv-az1543-369:41648] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffb40a287f3]
[fv-az1543-369:41648] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ffb40ea2b9e]
[fv-az1543-369:41648] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ffb40eae20c]
[fv-az1543-369:41648] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ffb40eae277]
[fv-az1543-369:41648] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffb40eae52b]
[fv-az1543-369:41648] [ 8] plumed(+0x12f48)[0x562107a52f48]
[fv-az1543-369:41648] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffb40a29d90]
[fv-az1543-369:41648] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffb40a29e40]
[fv-az1543-369:41648] [11] plumed(+0x131e5)[0x562107a531e5]
[fv-az1543-369:41648] *** End of error message ***
</pre>
{% endraw %}
