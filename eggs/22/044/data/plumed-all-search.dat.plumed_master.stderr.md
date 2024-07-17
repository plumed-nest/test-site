**Project ID:** [plumID:22.044]({{ '/' | absolute_url }}eggs/22/044/)  
Stderr for source:  plumed-all-search.dat   
Download: [zipped raw stdout](plumed-all-search.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-all-search.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX_PROPER with label laq4_mat : problem reading switching function description found the following rogue keywords in switching function input : RATIONAL
[fv-az659-178:70144] *** Process received signal ***
[fv-az659-178:70144] Signal: Aborted (6)
[fv-az659-178:70144] Signal code:  (-6)
[fv-az659-178:70144] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd01ae42520]
[fv-az659-178:70144] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd01ae969fc]
[fv-az659-178:70144] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd01ae42476]
[fv-az659-178:70144] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd01ae287f3]
[fv-az659-178:70144] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd01b2a2b9e]
[fv-az659-178:70144] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd01b2ae20c]
[fv-az659-178:70144] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd01b2ae277]
[fv-az659-178:70144] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd01b2ae52b]
[fv-az659-178:70144] [ 8] plumed_master(+0x14274)[0x5650dafdf274]
[fv-az659-178:70144] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd01ae29d90]
[fv-az659-178:70144] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd01ae29e40]
[fv-az659-178:70144] [11] plumed_master(+0x14ed5)[0x5650dafdfed5]
[fv-az659-178:70144] *** End of error message ***
</pre>
{% endraw %}
