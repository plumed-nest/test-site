**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-C/rep2/plumed_test_metad_params.dat   
Download: [zipped raw stdout](plumed_test_metad_params.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_test_metad_params.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Deprot/chain-C/01_box-min/ref.pdb
[runnervm1li68:04712] *** Process received signal ***
[runnervm1li68:04712] Signal: Aborted (6)
[runnervm1li68:04712] Signal code:  (-6)
[runnervm1li68:04712] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f50e9a45330]
[runnervm1li68:04712] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f50e9a9eb2c]
[runnervm1li68:04712] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f50e9a4527e]
[runnervm1li68:04712] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f50e9a288ff]
[runnervm1li68:04712] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f50e9ea5ff5]
[runnervm1li68:04712] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f50e9ebb0da]
[runnervm1li68:04712] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f50e9ea5a55]
[runnervm1li68:04712] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f50e9ea5a6f]
[runnervm1li68:04712] [ 8] plumed(+0x146dd)[0x55c1d09946dd]
[runnervm1li68:04712] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f50e9a2a1ca]
[runnervm1li68:04712] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f50e9a2a28b]
[runnervm1li68:04712] [11] plumed(+0x15365)[0x55c1d0995365]
[runnervm1li68:04712] *** End of error message ***
</pre>
{% endraw %}
