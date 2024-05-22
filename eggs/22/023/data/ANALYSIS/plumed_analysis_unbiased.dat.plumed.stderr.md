**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az659-568:40768] *** Process received signal ***
[fv-az659-568:40768] Signal: Aborted (6)
[fv-az659-568:40768] Signal code:  (-6)
[fv-az659-568:40768] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3e03842520]
[fv-az659-568:40768] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3e038969fc]
[fv-az659-568:40768] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3e03842476]
[fv-az659-568:40768] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3e038287f3]
[fv-az659-568:40768] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3e03ca2b9e]
[fv-az659-568:40768] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3e03cae20c]
[fv-az659-568:40768] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3e03cae277]
[fv-az659-568:40768] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3e03cae52b]
[fv-az659-568:40768] [ 8] plumed(+0x12f48)[0x55f05e483f48]
[fv-az659-568:40768] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3e03829d90]
[fv-az659-568:40768] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3e03829e40]
[fv-az659-568:40768] [11] plumed(+0x131e5)[0x55f05e4841e5]
[fv-az659-568:40768] *** End of error message ***
</pre>
{% endraw %}
