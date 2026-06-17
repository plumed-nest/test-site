**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-C/rep2/plumed_test_metad_params.dat   
Download: [zipped raw stdout](plumed_test_metad_params.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_test_metad_params.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Deprot/chain-C/01_box-min/ref.pdb
[runnervm1li68:05194] *** Process received signal ***
[runnervm1li68:05194] Signal: Aborted (6)
[runnervm1li68:05194] Signal code:  (-6)
[runnervm1li68:05194] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbaaf245330]
[runnervm1li68:05194] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbaaf29eb2c]
[runnervm1li68:05194] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbaaf24527e]
[runnervm1li68:05194] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbaaf2288ff]
[runnervm1li68:05194] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbaaf6a5ff5]
[runnervm1li68:05194] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbaaf6bb0da]
[runnervm1li68:05194] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbaaf6a5a55]
[runnervm1li68:05194] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbaaf6a5a6f]
[runnervm1li68:05194] [ 8] plumed_master(+0x146dd)[0x558ebaf406dd]
[runnervm1li68:05194] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbaaf22a1ca]
[runnervm1li68:05194] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbaaf22a28b]
[runnervm1li68:05194] [11] plumed_master(+0x15365)[0x558ebaf41365]
[runnervm1li68:05194] *** End of error message ***
</pre>
{% endraw %}
