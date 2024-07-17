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
[fv-az1108-41:71112] *** Process received signal ***
[fv-az1108-41:71112] Signal: Aborted (6)
[fv-az1108-41:71112] Signal code:  (-6)
[fv-az1108-41:71112] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f977a842520]
[fv-az1108-41:71112] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f977a8969fc]
[fv-az1108-41:71112] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f977a842476]
[fv-az1108-41:71112] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f977a8287f3]
[fv-az1108-41:71112] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f977aca2b9e]
[fv-az1108-41:71112] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f977acae20c]
[fv-az1108-41:71112] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f977acae277]
[fv-az1108-41:71112] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f977acae52b]
[fv-az1108-41:71112] [ 8] plumed(+0x12f48)[0x564a37542f48]
[fv-az1108-41:71112] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f977a829d90]
[fv-az1108-41:71112] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f977a829e40]
[fv-az1108-41:71112] [11] plumed(+0x131e5)[0x564a375431e5]
[fv-az1108-41:71112] *** End of error message ***
</pre>
{% endraw %}
