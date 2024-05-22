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
[fv-az659-568:39437] *** Process received signal ***
[fv-az659-568:39437] Signal: Aborted (6)
[fv-az659-568:39437] Signal code:  (-6)
[fv-az659-568:39437] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa9adc42520]
[fv-az659-568:39437] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa9adc969fc]
[fv-az659-568:39437] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa9adc42476]
[fv-az659-568:39437] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa9adc287f3]
[fv-az659-568:39437] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa9ae0a2b9e]
[fv-az659-568:39437] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa9ae0ae20c]
[fv-az659-568:39437] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa9ae0ae277]
[fv-az659-568:39437] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa9ae0ae52b]
[fv-az659-568:39437] [ 8] plumed_master(+0x14274)[0x55837f08c274]
[fv-az659-568:39437] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa9adc29d90]
[fv-az659-568:39437] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa9adc29e40]
[fv-az659-568:39437] [11] plumed_master(+0x14ed5)[0x55837f08ced5]
[fv-az659-568:39437] *** End of error message ***
</pre>
{% endraw %}
