**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az1108-41:71081] *** Process received signal ***
[fv-az1108-41:71081] Signal: Aborted (6)
[fv-az1108-41:71081] Signal code:  (-6)
[fv-az1108-41:71081] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc1dfe42520]
[fv-az1108-41:71081] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc1dfe969fc]
[fv-az1108-41:71081] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc1dfe42476]
[fv-az1108-41:71081] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc1dfe287f3]
[fv-az1108-41:71081] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc1e02a2b9e]
[fv-az1108-41:71081] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc1e02ae20c]
[fv-az1108-41:71081] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc1e02ae277]
[fv-az1108-41:71081] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc1e02ae52b]
[fv-az1108-41:71081] [ 8] plumed(+0x12f48)[0x564571e19f48]
[fv-az1108-41:71081] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc1dfe29d90]
[fv-az1108-41:71081] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc1dfe29e40]
[fv-az1108-41:71081] [11] plumed(+0x131e5)[0x564571e1a1e5]
[fv-az1108-41:71081] *** End of error message ***
</pre>
{% endraw %}