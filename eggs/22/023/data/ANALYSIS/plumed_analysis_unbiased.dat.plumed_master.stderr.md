**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[runnervm1li68:08206] *** Process received signal ***
[runnervm1li68:08206] Signal: Aborted (6)
[runnervm1li68:08206] Signal code:  (-6)
[runnervm1li68:08206] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb3bba45330]
[runnervm1li68:08206] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb3bba9eb2c]
[runnervm1li68:08206] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb3bba4527e]
[runnervm1li68:08206] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb3bba288ff]
[runnervm1li68:08206] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb3bbea5ff5]
[runnervm1li68:08206] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb3bbebb0da]
[runnervm1li68:08206] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb3bbea5a55]
[runnervm1li68:08206] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb3bbea5a6f]
[runnervm1li68:08206] [ 8] plumed_master(+0x146dd)[0x55daf620c6dd]
[runnervm1li68:08206] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb3bba2a1ca]
[runnervm1li68:08206] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb3bba2a28b]
[runnervm1li68:08206] [11] plumed_master(+0x15365)[0x55daf620d365]
[runnervm1li68:08206] *** End of error message ***
</pre>
{% endraw %}
