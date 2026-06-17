**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[runnervm1li68:08140] *** Process received signal ***
[runnervm1li68:08140] Signal: Aborted (6)
[runnervm1li68:08140] Signal code:  (-6)
[runnervm1li68:08140] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f68a5645330]
[runnervm1li68:08140] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f68a569eb2c]
[runnervm1li68:08140] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f68a564527e]
[runnervm1li68:08140] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f68a56288ff]
[runnervm1li68:08140] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f68a5aa5ff5]
[runnervm1li68:08140] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f68a5abb0da]
[runnervm1li68:08140] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f68a5aa5a55]
[runnervm1li68:08140] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f68a5aa5a6f]
[runnervm1li68:08140] [ 8] plumed(+0x146dd)[0x55ee433236dd]
[runnervm1li68:08140] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f68a562a1ca]
[runnervm1li68:08140] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f68a562a28b]
[runnervm1li68:08140] [11] plumed(+0x15365)[0x55ee43324365]
[runnervm1li68:08140] *** End of error message ***
</pre>
{% endraw %}
