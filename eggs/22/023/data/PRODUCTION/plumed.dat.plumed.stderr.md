**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[fv-az1108-41:71143] *** Process received signal ***
[fv-az1108-41:71143] Signal: Aborted (6)
[fv-az1108-41:71143] Signal code:  (-6)
[fv-az1108-41:71143] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb132442520]
[fv-az1108-41:71143] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb1324969fc]
[fv-az1108-41:71143] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb132442476]
[fv-az1108-41:71143] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb1324287f3]
[fv-az1108-41:71143] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb1328a2b9e]
[fv-az1108-41:71143] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb1328ae20c]
[fv-az1108-41:71143] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb1328ae277]
[fv-az1108-41:71143] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb1328ae52b]
[fv-az1108-41:71143] [ 8] plumed(+0x12f48)[0x55a88562df48]
[fv-az1108-41:71143] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb132429d90]
[fv-az1108-41:71143] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb132429e40]
[fv-az1108-41:71143] [11] plumed(+0x131e5)[0x55a88562e1e5]
[fv-az1108-41:71143] *** End of error message ***
</pre>
{% endraw %}
