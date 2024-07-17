**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1efa.dat   
Download: [zipped raw stdout](plumed_print_1efa.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print_1efa.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_noTet_99sbws_proc_mod_resID.pdb
[fv-az841-65:69778] *** Process received signal ***
[fv-az841-65:69778] Signal: Aborted (6)
[fv-az841-65:69778] Signal code:  (-6)
[fv-az841-65:69778] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4d2c042520]
[fv-az841-65:69778] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4d2c0969fc]
[fv-az841-65:69778] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4d2c042476]
[fv-az841-65:69778] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4d2c0287f3]
[fv-az841-65:69778] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4d2c4a2b9e]
[fv-az841-65:69778] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4d2c4ae20c]
[fv-az841-65:69778] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4d2c4ae277]
[fv-az841-65:69778] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4d2c4ae52b]
[fv-az841-65:69778] [ 8] plumed(+0x12f48)[0x563425d2ef48]
[fv-az841-65:69778] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4d2c029d90]
[fv-az841-65:69778] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4d2c029e40]
[fv-az841-65:69778] [11] plumed(+0x131e5)[0x563425d2f1e5]
[fv-az841-65:69778] *** End of error message ***
</pre>
{% endraw %}
