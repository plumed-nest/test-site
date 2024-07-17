**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az1108-41:71120] *** Process received signal ***
[fv-az1108-41:71120] Signal: Aborted (6)
[fv-az1108-41:71120] Signal code:  (-6)
[fv-az1108-41:71120] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f476bc42520]
[fv-az1108-41:71120] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f476bc969fc]
[fv-az1108-41:71120] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f476bc42476]
[fv-az1108-41:71120] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f476bc287f3]
[fv-az1108-41:71120] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f476c0a2b9e]
[fv-az1108-41:71120] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f476c0ae20c]
[fv-az1108-41:71120] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f476c0ae277]
[fv-az1108-41:71120] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f476c0ae52b]
[fv-az1108-41:71120] [ 8] plumed_master(+0x14274)[0x561b40710274]
[fv-az1108-41:71120] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f476bc29d90]
[fv-az1108-41:71120] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f476bc29e40]
[fv-az1108-41:71120] [11] plumed_master(+0x14ed5)[0x561b40710ed5]
[fv-az1108-41:71120] *** End of error message ***
</pre>
{% endraw %}
