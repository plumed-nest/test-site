**Project ID:** [plumID:21.016]({{ '/' | absolute_url }}eggs/21/016/)  
Stderr for source:  input_files/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=1
[fv-az659-178:71122] *** Process received signal ***
[fv-az659-178:71122] Signal: Aborted (6)
[fv-az659-178:71122] Signal code:  (-6)
[fv-az659-178:71122] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdcc4642520]
[fv-az659-178:71122] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdcc46969fc]
[fv-az659-178:71122] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdcc4642476]
[fv-az659-178:71122] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdcc46287f3]
[fv-az659-178:71122] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdcc4aa2b9e]
[fv-az659-178:71122] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdcc4aae20c]
[fv-az659-178:71122] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdcc4aae277]
[fv-az659-178:71122] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdcc4aae52b]
[fv-az659-178:71122] [ 8] plumed(+0x12f48)[0x558c228a9f48]
[fv-az659-178:71122] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdcc4629d90]
[fv-az659-178:71122] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdcc4629e40]
[fv-az659-178:71122] [11] plumed(+0x131e5)[0x558c228aa1e5]
[fv-az659-178:71122] *** End of error message ***
</pre>
{% endraw %}
