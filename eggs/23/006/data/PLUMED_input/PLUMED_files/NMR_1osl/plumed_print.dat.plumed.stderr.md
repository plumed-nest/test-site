**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  PLUMED_input/PLUMED_files/NMR_1osl/plumed_print.dat   
Download: [zipped raw stdout](plumed_print.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1osl_C52V_GMX_new_numbering.pdb
[fv-az841-65:69841] *** Process received signal ***
[fv-az841-65:69841] Signal: Aborted (6)
[fv-az841-65:69841] Signal code:  (-6)
[fv-az841-65:69841] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5831042520]
[fv-az841-65:69841] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f58310969fc]
[fv-az841-65:69841] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5831042476]
[fv-az841-65:69841] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f58310287f3]
[fv-az841-65:69841] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f58314a2b9e]
[fv-az841-65:69841] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f58314ae20c]
[fv-az841-65:69841] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f58314ae277]
[fv-az841-65:69841] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f58314ae52b]
[fv-az841-65:69841] [ 8] plumed(+0x12f48)[0x559511114f48]
[fv-az841-65:69841] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5831029d90]
[fv-az841-65:69841] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5831029e40]
[fv-az841-65:69841] [11] plumed(+0x131e5)[0x5595111151e5]
[fv-az841-65:69841] *** End of error message ***
</pre>
{% endraw %}
