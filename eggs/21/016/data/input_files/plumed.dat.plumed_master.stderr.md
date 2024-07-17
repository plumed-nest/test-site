**Project ID:** [plumID:21.016]({{ '/' | absolute_url }}eggs/21/016/)  
Stderr for source:  input_files/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=1
[fv-az659-178:71130] *** Process received signal ***
[fv-az659-178:71130] Signal: Aborted (6)
[fv-az659-178:71130] Signal code:  (-6)
[fv-az659-178:71130] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f392d842520]
[fv-az659-178:71130] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f392d8969fc]
[fv-az659-178:71130] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f392d842476]
[fv-az659-178:71130] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f392d8287f3]
[fv-az659-178:71130] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f392dca2b9e]
[fv-az659-178:71130] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f392dcae20c]
[fv-az659-178:71130] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f392dcae277]
[fv-az659-178:71130] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f392dcae52b]
[fv-az659-178:71130] [ 8] plumed_master(+0x14274)[0x55eb7d1a7274]
[fv-az659-178:71130] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f392d829d90]
[fv-az659-178:71130] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f392d829e40]
[fv-az659-178:71130] [11] plumed_master(+0x14ed5)[0x55eb7d1a7ed5]
[fv-az659-178:71130] *** End of error message ***
</pre>
{% endraw %}
