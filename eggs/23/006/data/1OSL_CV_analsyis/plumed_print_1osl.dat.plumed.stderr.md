**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  1OSL_CV_analsyis/plumed_print_1osl.dat   
Download: [zipped raw stdout](plumed_print_1osl.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print_1osl.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1efa_NOD_S99_mod_ID.pdb
[fv-az841-65:69810] *** Process received signal ***
[fv-az841-65:69810] Signal: Aborted (6)
[fv-az841-65:69810] Signal code:  (-6)
[fv-az841-65:69810] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb354642520]
[fv-az841-65:69810] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb3546969fc]
[fv-az841-65:69810] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb354642476]
[fv-az841-65:69810] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb3546287f3]
[fv-az841-65:69810] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb354aa2b9e]
[fv-az841-65:69810] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb354aae20c]
[fv-az841-65:69810] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb354aae277]
[fv-az841-65:69810] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb354aae52b]
[fv-az841-65:69810] [ 8] plumed(+0x12f48)[0x55b53d1bdf48]
[fv-az841-65:69810] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb354629d90]
[fv-az841-65:69810] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb354629e40]
[fv-az841-65:69810] [11] plumed(+0x131e5)[0x55b53d1be1e5]
[fv-az841-65:69810] *** End of error message ***
</pre>
{% endraw %}
