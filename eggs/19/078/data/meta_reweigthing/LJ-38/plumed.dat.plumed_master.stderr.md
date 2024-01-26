**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az532-512:10607] *** Process received signal ***
[fv-az532-512:10607] Signal: Aborted (6)
[fv-az532-512:10607] Signal code:  (-6)
[fv-az532-512:10607] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0690642520]
[fv-az532-512:10607] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f06906969fc]
[fv-az532-512:10607] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0690642476]
[fv-az532-512:10607] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f06906287f3]
[fv-az532-512:10607] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f0690aa4f26]
[fv-az532-512:10607] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f0690ab6d9c]
[fv-az532-512:10607] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f0690ab6e07]
[fv-az532-512:10607] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0690ab70bb]
[fv-az532-512:10607] [ 8] plumed_master(+0x12ebf)[0x564e9c765ebf]
[fv-az532-512:10607] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0690629d90]
[fv-az532-512:10607] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0690629e40]
[fv-az532-512:10607] [11] plumed_master(+0x13155)[0x564e9c766155]
[fv-az532-512:10607] *** End of error message ***
</pre>
{% endraw %}
