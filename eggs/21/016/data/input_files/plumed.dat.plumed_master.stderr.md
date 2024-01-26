**Project ID:** [plumID:21.016]({{ '/' | absolute_url }}eggs/21/016/)  
Stderr for source:  input_files/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=1
[fv-az979-741:05923] *** Process received signal ***
[fv-az979-741:05923] Signal: Aborted (6)
[fv-az979-741:05923] Signal code:  (-6)
[fv-az979-741:05923] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f22ce842520]
[fv-az979-741:05923] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f22ce8969fc]
[fv-az979-741:05923] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f22ce842476]
[fv-az979-741:05923] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f22ce8287f3]
[fv-az979-741:05923] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f22ceca4f26]
[fv-az979-741:05923] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f22cecb6d9c]
[fv-az979-741:05923] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f22cecb6e07]
[fv-az979-741:05923] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f22cecb70bb]
[fv-az979-741:05923] [ 8] plumed_master(+0x12ebf)[0x55805570eebf]
[fv-az979-741:05923] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f22ce829d90]
[fv-az979-741:05923] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f22ce829e40]
[fv-az979-741:05923] [11] plumed_master(+0x13155)[0x55805570f155]
[fv-az979-741:05923] *** End of error message ***
</pre>
{% endraw %}
