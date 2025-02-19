**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az1326-415:09908] *** Process received signal ***
[fv-az1326-415:09908] Signal: Aborted (6)
[fv-az1326-415:09908] Signal code:  (-6)
[fv-az1326-415:09908] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc9a5445330]
[fv-az1326-415:09908] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc9a549eb2c]
[fv-az1326-415:09908] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc9a544527e]
[fv-az1326-415:09908] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc9a54288ff]
[fv-az1326-415:09908] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc9a58a5ff5]
[fv-az1326-415:09908] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc9a58bb0da]
[fv-az1326-415:09908] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc9a58a5a55]
[fv-az1326-415:09908] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc9a58a5a6f]
[fv-az1326-415:09908] [ 8] plumed(+0x146dd)[0x55da6b5016dd]
[fv-az1326-415:09908] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc9a542a1ca]
[fv-az1326-415:09908] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc9a542a28b]
[fv-az1326-415:09908] [11] plumed(+0x15365)[0x55da6b502365]
[fv-az1326-415:09908] *** End of error message ***
</pre>
{% endraw %}
