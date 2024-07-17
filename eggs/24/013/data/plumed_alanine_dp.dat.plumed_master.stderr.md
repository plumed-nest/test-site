**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[fv-az975-63:69605] *** Process received signal ***
[fv-az975-63:69605] Signal: Aborted (6)
[fv-az975-63:69605] Signal code:  (-6)
[fv-az975-63:69605] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa8a7a42520]
[fv-az975-63:69605] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa8a7a969fc]
[fv-az975-63:69605] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa8a7a42476]
[fv-az975-63:69605] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa8a7a287f3]
[fv-az975-63:69605] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa8a7ea2b9e]
[fv-az975-63:69605] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa8a7eae20c]
[fv-az975-63:69605] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa8a7eae277]
[fv-az975-63:69605] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa8a7eae52b]
[fv-az975-63:69605] [ 8] plumed_master(+0x14274)[0x555ba5887274]
[fv-az975-63:69605] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa8a7a29d90]
[fv-az975-63:69605] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa8a7a29e40]
[fv-az975-63:69605] [11] plumed_master(+0x14ed5)[0x555ba5887ed5]
[fv-az975-63:69605] *** End of error message ***
</pre>
{% endraw %}
