**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_GeTe.dat   
Download: [zipped raw stdout](plumed_GeTe.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_GeTe.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label cc_cmat : it was not possible to interpret atom name flq6
[fv-az774-16:73962] *** Process received signal ***
[fv-az774-16:73962] Signal: Aborted (6)
[fv-az774-16:73962] Signal code:  (-6)
[fv-az774-16:73962] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6609842520]
[fv-az774-16:73962] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f66098969fc]
[fv-az774-16:73962] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6609842476]
[fv-az774-16:73962] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f66098287f3]
[fv-az774-16:73962] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6609ca2b9e]
[fv-az774-16:73962] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6609cae20c]
[fv-az774-16:73962] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6609cae277]
[fv-az774-16:73962] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6609cae52b]
[fv-az774-16:73962] [ 8] plumed_master(+0x14274)[0x55e963b6a274]
[fv-az774-16:73962] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6609829d90]
[fv-az774-16:73962] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6609829e40]
[fv-az774-16:73962] [11] plumed_master(+0x14ed5)[0x55e963b6aed5]
[fv-az774-16:73962] *** End of error message ***
</pre>
{% endraw %}
