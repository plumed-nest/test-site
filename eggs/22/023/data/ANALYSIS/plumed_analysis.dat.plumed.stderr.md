**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az1326-415:09856] *** Process received signal ***
[fv-az1326-415:09856] Signal: Aborted (6)
[fv-az1326-415:09856] Signal code:  (-6)
[fv-az1326-415:09856] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1a69645330]
[fv-az1326-415:09856] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1a6969eb2c]
[fv-az1326-415:09856] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1a6964527e]
[fv-az1326-415:09856] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1a696288ff]
[fv-az1326-415:09856] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1a69aa5ff5]
[fv-az1326-415:09856] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1a69abb0da]
[fv-az1326-415:09856] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1a69aa5a55]
[fv-az1326-415:09856] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1a69aa5a6f]
[fv-az1326-415:09856] [ 8] plumed(+0x146dd)[0x558ea3c106dd]
[fv-az1326-415:09856] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1a6962a1ca]
[fv-az1326-415:09856] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1a6962a28b]
[fv-az1326-415:09856] [11] plumed(+0x15365)[0x558ea3c11365]
[fv-az1326-415:09856] *** End of error message ***
</pre>
{% endraw %}
