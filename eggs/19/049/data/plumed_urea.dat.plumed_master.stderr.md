**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_urea.dat   
Download: [zipped raw stdout](plumed_urea.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_urea.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label @s41 : missing SWITCH11 keyword
[fv-az774-16:74023] *** Process received signal ***
[fv-az774-16:74023] Signal: Aborted (6)
[fv-az774-16:74023] Signal code:  (-6)
[fv-az774-16:74023] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb4f2242520]
[fv-az774-16:74023] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb4f22969fc]
[fv-az774-16:74023] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb4f2242476]
[fv-az774-16:74023] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb4f22287f3]
[fv-az774-16:74023] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb4f26a2b9e]
[fv-az774-16:74023] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb4f26ae20c]
[fv-az774-16:74023] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb4f26ae277]
[fv-az774-16:74023] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb4f26ae52b]
[fv-az774-16:74023] [ 8] plumed_master(+0x14274)[0x557bda6f9274]
[fv-az774-16:74023] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb4f2229d90]
[fv-az774-16:74023] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb4f2229e40]
[fv-az774-16:74023] [11] plumed_master(+0x14ed5)[0x557bda6f9ed5]
[fv-az774-16:74023] *** End of error message ***
</pre>
{% endraw %}
