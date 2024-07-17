**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1osl.dat   
Download: [zipped raw stdout](plumed_print_1osl.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_print_1osl.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_NOD_S99_mod_ID.pdb
[fv-az841-65:69818] *** Process received signal ***
[fv-az841-65:69818] Signal: Aborted (6)
[fv-az841-65:69818] Signal code:  (-6)
[fv-az841-65:69818] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fea1fe42520]
[fv-az841-65:69818] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fea1fe969fc]
[fv-az841-65:69818] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fea1fe42476]
[fv-az841-65:69818] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fea1fe287f3]
[fv-az841-65:69818] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fea202a2b9e]
[fv-az841-65:69818] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fea202ae20c]
[fv-az841-65:69818] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fea202ae277]
[fv-az841-65:69818] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fea202ae52b]
[fv-az841-65:69818] [ 8] plumed_master(+0x14274)[0x55babb8ce274]
[fv-az841-65:69818] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fea1fe29d90]
[fv-az841-65:69818] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fea1fe29e40]
[fv-az841-65:69818] [11] plumed_master(+0x14ed5)[0x55babb8ceed5]
[fv-az841-65:69818] *** End of error message ***
</pre>
{% endraw %}
