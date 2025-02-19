**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[fv-az1326-415:09965] *** Process received signal ***
[fv-az1326-415:09965] Signal: Aborted (6)
[fv-az1326-415:09965] Signal code:  (-6)
[fv-az1326-415:09965] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5bcfc45330]
[fv-az1326-415:09965] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5bcfc9eb2c]
[fv-az1326-415:09965] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5bcfc4527e]
[fv-az1326-415:09965] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5bcfc288ff]
[fv-az1326-415:09965] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5bd00a5ff5]
[fv-az1326-415:09965] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5bd00bb0da]
[fv-az1326-415:09965] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5bd00a5a55]
[fv-az1326-415:09965] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5bd00a5a6f]
[fv-az1326-415:09965] [ 8] plumed(+0x146dd)[0x55abbe7bf6dd]
[fv-az1326-415:09965] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5bcfc2a1ca]
[fv-az1326-415:09965] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5bcfc2a28b]
[fv-az1326-415:09965] [11] plumed(+0x15365)[0x55abbe7c0365]
[fv-az1326-415:09965] *** End of error message ***
</pre>
{% endraw %}
