**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[runnervm1li68:05885] *** Process received signal ***
[runnervm1li68:05885] Signal: Aborted (6)
[runnervm1li68:05885] Signal code:  (-6)
[runnervm1li68:05885] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1c96845330]
[runnervm1li68:05885] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1c9689eb2c]
[runnervm1li68:05885] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1c9684527e]
[runnervm1li68:05885] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1c968288ff]
[runnervm1li68:05885] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1c96ca5ff5]
[runnervm1li68:05885] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1c96cbb0da]
[runnervm1li68:05885] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1c96ca5a55]
[runnervm1li68:05885] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1c96ca5a6f]
[runnervm1li68:05885] [ 8] plumed(+0x146dd)[0x562b529bd6dd]
[runnervm1li68:05885] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1c9682a1ca]
[runnervm1li68:05885] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1c9682a28b]
[runnervm1li68:05885] [11] plumed(+0x15365)[0x562b529be365]
[runnervm1li68:05885] *** End of error message ***
</pre>
{% endraw %}
