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
[fv-az1109-238:40861] *** Process received signal ***
[fv-az1109-238:40861] Signal: Aborted (6)
[fv-az1109-238:40861] Signal code:  (-6)
[fv-az1109-238:40861] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd57c442520]
[fv-az1109-238:40861] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd57c4969fc]
[fv-az1109-238:40861] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd57c442476]
[fv-az1109-238:40861] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd57c4287f3]
[fv-az1109-238:40861] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd57c8a2b9e]
[fv-az1109-238:40861] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd57c8ae20c]
[fv-az1109-238:40861] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd57c8ae277]
[fv-az1109-238:40861] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd57c8ae52b]
[fv-az1109-238:40861] [ 8] plumed(+0x12f48)[0x556c19623f48]
[fv-az1109-238:40861] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd57c429d90]
[fv-az1109-238:40861] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd57c429e40]
[fv-az1109-238:40861] [11] plumed(+0x131e5)[0x556c196241e5]
[fv-az1109-238:40861] *** End of error message ***
</pre>
{% endraw %}
