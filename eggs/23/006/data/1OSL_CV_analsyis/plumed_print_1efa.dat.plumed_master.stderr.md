**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1efa.dat   
Download: [zipped raw stdout](plumed_print_1efa.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_print_1efa.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_noTet_99sbws_proc_mod_resID.pdb
[fv-az841-65:69786] *** Process received signal ***
[fv-az841-65:69786] Signal: Aborted (6)
[fv-az841-65:69786] Signal code:  (-6)
[fv-az841-65:69786] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa9b7c42520]
[fv-az841-65:69786] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa9b7c969fc]
[fv-az841-65:69786] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa9b7c42476]
[fv-az841-65:69786] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa9b7c287f3]
[fv-az841-65:69786] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa9b80a2b9e]
[fv-az841-65:69786] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa9b80ae20c]
[fv-az841-65:69786] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa9b80ae277]
[fv-az841-65:69786] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa9b80ae52b]
[fv-az841-65:69786] [ 8] plumed_master(+0x14274)[0x565414e00274]
[fv-az841-65:69786] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa9b7c29d90]
[fv-az841-65:69786] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa9b7c29e40]
[fv-az841-65:69786] [11] plumed_master(+0x14ed5)[0x565414e00ed5]
[fv-az841-65:69786] *** End of error message ***
</pre>
{% endraw %}
