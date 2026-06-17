**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[runnervm1li68:05901] *** Process received signal ***
[runnervm1li68:05901] Signal: Aborted (6)
[runnervm1li68:05901] Signal code:  (-6)
[runnervm1li68:05901] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9dc7a45330]
[runnervm1li68:05901] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9dc7a9eb2c]
[runnervm1li68:05901] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9dc7a4527e]
[runnervm1li68:05901] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9dc7a288ff]
[runnervm1li68:05901] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9dc7ea5ff5]
[runnervm1li68:05901] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9dc7ebb0da]
[runnervm1li68:05901] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9dc7ea5a55]
[runnervm1li68:05901] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9dc7ea5a6f]
[runnervm1li68:05901] [ 8] plumed_master(+0x146dd)[0x55882ed4e6dd]
[runnervm1li68:05901] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9dc7a2a1ca]
[runnervm1li68:05901] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9dc7a2a28b]
[runnervm1li68:05901] [11] plumed_master(+0x15365)[0x55882ed4f365]
[runnervm1li68:05901] *** End of error message ***
</pre>
{% endraw %}
