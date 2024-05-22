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
[fv-az659-568:40807] *** Process received signal ***
[fv-az659-568:40807] Signal: Aborted (6)
[fv-az659-568:40807] Signal code:  (-6)
[fv-az659-568:40807] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdf54e42520]
[fv-az659-568:40807] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdf54e969fc]
[fv-az659-568:40807] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdf54e42476]
[fv-az659-568:40807] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdf54e287f3]
[fv-az659-568:40807] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdf552a2b9e]
[fv-az659-568:40807] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdf552ae20c]
[fv-az659-568:40807] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdf552ae277]
[fv-az659-568:40807] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdf552ae52b]
[fv-az659-568:40807] [ 8] plumed_master(+0x14274)[0x563f474c0274]
[fv-az659-568:40807] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdf54e29d90]
[fv-az659-568:40807] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdf54e29e40]
[fv-az659-568:40807] [11] plumed_master(+0x14ed5)[0x563f474c0ed5]
[fv-az659-568:40807] *** End of error message ***
</pre>
{% endraw %}
