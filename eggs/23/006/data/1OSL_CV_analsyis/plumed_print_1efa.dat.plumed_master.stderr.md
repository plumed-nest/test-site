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
[fv-az1542-52:04607] *** Process received signal ***
[fv-az1542-52:04607] Signal: Aborted (6)
[fv-az1542-52:04607] Signal code:  (-6)
[fv-az1542-52:04607] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbe8f442520]
[fv-az1542-52:04607] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbe8f4969fc]
[fv-az1542-52:04607] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbe8f442476]
[fv-az1542-52:04607] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbe8f4287f3]
[fv-az1542-52:04607] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fbe8f8a4f26]
[fv-az1542-52:04607] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fbe8f8b6d9c]
[fv-az1542-52:04607] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fbe8f8b6e07]
[fv-az1542-52:04607] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbe8f8b70bb]
[fv-az1542-52:04607] [ 8] plumed_master(+0x12ebf)[0x5617295c9ebf]
[fv-az1542-52:04607] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbe8f429d90]
[fv-az1542-52:04607] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbe8f429e40]
[fv-az1542-52:04607] [11] plumed_master(+0x13155)[0x5617295ca155]
[fv-az1542-52:04607] *** End of error message ***
</pre>
{% endraw %}
