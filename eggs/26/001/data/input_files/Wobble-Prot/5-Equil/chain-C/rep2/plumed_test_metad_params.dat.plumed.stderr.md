**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-C/rep2/plumed_test_metad_params.dat   
Download: [zipped raw stdout](plumed_test_metad_params.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_test_metad_params.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Deprot/chain-C/01_box-min/ref.pdb
[runnervm1li68:05178] *** Process received signal ***
[runnervm1li68:05178] Signal: Aborted (6)
[runnervm1li68:05178] Signal code:  (-6)
[runnervm1li68:05178] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7145445330]
[runnervm1li68:05178] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f714549eb2c]
[runnervm1li68:05178] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f714544527e]
[runnervm1li68:05178] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f71454288ff]
[runnervm1li68:05178] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f71458a5ff5]
[runnervm1li68:05178] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f71458bb0da]
[runnervm1li68:05178] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f71458a5a55]
[runnervm1li68:05178] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f71458a5a6f]
[runnervm1li68:05178] [ 8] plumed(+0x146dd)[0x55d707af76dd]
[runnervm1li68:05178] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f714542a1ca]
[runnervm1li68:05178] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f714542a28b]
[runnervm1li68:05178] [11] plumed(+0x15365)[0x55d707af8365]
[runnervm1li68:05178] *** End of error message ***
</pre>
{% endraw %}
