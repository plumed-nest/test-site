**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1osl.dat   
Download: [zipped raw stdout](plumed_print_1osl.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_print_1osl.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_NOD_S99_mod_ID.pdb
[fv-az1770-999:06489] *** Process received signal ***
[fv-az1770-999:06489] Signal: Aborted (6)
[fv-az1770-999:06489] Signal code:  (-6)
[fv-az1770-999:06489] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6b45245330]
[fv-az1770-999:06489] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6b4529eb2c]
[fv-az1770-999:06489] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6b4524527e]
[fv-az1770-999:06489] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6b452288ff]
[fv-az1770-999:06489] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6b456a5ff5]
[fv-az1770-999:06489] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6b456bb0da]
[fv-az1770-999:06489] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6b456a5a55]
[fv-az1770-999:06489] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6b456a5a6f]
[fv-az1770-999:06489] [ 8] plumed_master(+0x146dd)[0x5563f7f636dd]
[fv-az1770-999:06489] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6b4522a1ca]
[fv-az1770-999:06489] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6b4522a28b]
[fv-az1770-999:06489] [11] plumed_master(+0x15365)[0x5563f7f64365]
[fv-az1770-999:06489] *** End of error message ***
</pre>
{% endraw %}
