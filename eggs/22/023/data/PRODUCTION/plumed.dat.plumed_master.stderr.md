**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[fv-az1108-41:71151] *** Process received signal ***
[fv-az1108-41:71151] Signal: Aborted (6)
[fv-az1108-41:71151] Signal code:  (-6)
[fv-az1108-41:71151] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7aaf842520]
[fv-az1108-41:71151] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7aaf8969fc]
[fv-az1108-41:71151] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7aaf842476]
[fv-az1108-41:71151] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7aaf8287f3]
[fv-az1108-41:71151] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7aafca2b9e]
[fv-az1108-41:71151] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7aafcae20c]
[fv-az1108-41:71151] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7aafcae277]
[fv-az1108-41:71151] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7aafcae52b]
[fv-az1108-41:71151] [ 8] plumed_master(+0x14274)[0x555795230274]
[fv-az1108-41:71151] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7aaf829d90]
[fv-az1108-41:71151] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7aaf829e40]
[fv-az1108-41:71151] [11] plumed_master(+0x14ed5)[0x555795230ed5]
[fv-az1108-41:71151] *** End of error message ***
</pre>
{% endraw %}
