**Project ID:** [plumID:22.044]({{ '/' | absolute_url }}eggs/22/044/)  
Stderr for source:  plumed-all-search.dat   
Download: [zipped raw stdout](plumed-all-search.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-all-search.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label laq4_mat : problem reading switching function description found the following rogue keywords in switching function input : RATIONAL
[fv-az1109-238:39895] *** Process received signal ***
[fv-az1109-238:39895] Signal: Aborted (6)
[fv-az1109-238:39895] Signal code:  (-6)
[fv-az1109-238:39895] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f09f3a42520]
[fv-az1109-238:39895] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f09f3a969fc]
[fv-az1109-238:39895] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f09f3a42476]
[fv-az1109-238:39895] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f09f3a287f3]
[fv-az1109-238:39895] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f09f3ea2b9e]
[fv-az1109-238:39895] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f09f3eae20c]
[fv-az1109-238:39895] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f09f3eae277]
[fv-az1109-238:39895] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f09f3eae52b]
[fv-az1109-238:39895] [ 8] plumed_master(+0x14274)[0x5639b4a7a274]
[fv-az1109-238:39895] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f09f3a29d90]
[fv-az1109-238:39895] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f09f3a29e40]
[fv-az1109-238:39895] [11] plumed_master(+0x14ed5)[0x5639b4a7aed5]
[fv-az1109-238:39895] *** End of error message ***
</pre>
{% endraw %}
