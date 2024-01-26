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
[fv-az1542-52:04641] *** Process received signal ***
[fv-az1542-52:04641] Signal: Aborted (6)
[fv-az1542-52:04641] Signal code:  (-6)
[fv-az1542-52:04641] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f688d442520]
[fv-az1542-52:04641] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f688d4969fc]
[fv-az1542-52:04641] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f688d442476]
[fv-az1542-52:04641] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f688d4287f3]
[fv-az1542-52:04641] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f688d8a4f26]
[fv-az1542-52:04641] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f688d8b6d9c]
[fv-az1542-52:04641] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f688d8b6e07]
[fv-az1542-52:04641] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f688d8b70bb]
[fv-az1542-52:04641] [ 8] plumed_master(+0x12ebf)[0x55f2b3338ebf]
[fv-az1542-52:04641] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f688d429d90]
[fv-az1542-52:04641] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f688d429e40]
[fv-az1542-52:04641] [11] plumed_master(+0x13155)[0x55f2b3339155]
[fv-az1542-52:04641] *** End of error message ***
</pre>
{% endraw %}
