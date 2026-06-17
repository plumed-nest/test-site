**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-C/rep2/equil_C_P_2.dat   
Download: [zipped raw stdout](equil_C_P_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](equil_C_P_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:05142] *** Process received signal ***
[runnervm1li68:05142] Signal: Aborted (6)
[runnervm1li68:05142] Signal code:  (-6)
[runnervm1li68:05142] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8de4a45330]
[runnervm1li68:05142] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f8de4a9eb2c]
[runnervm1li68:05142] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f8de4a4527e]
[runnervm1li68:05142] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f8de4a288ff]
[runnervm1li68:05142] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f8de4ea5ff5]
[runnervm1li68:05142] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f8de4ebb0da]
[runnervm1li68:05142] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f8de4ea5a55]
[runnervm1li68:05142] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f8de4ea5a6f]
[runnervm1li68:05142] [ 8] plumed_master(+0x146dd)[0x5600b8f8b6dd]
[runnervm1li68:05142] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f8de4a2a1ca]
[runnervm1li68:05142] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f8de4a2a28b]
[runnervm1li68:05142] [11] plumed_master(+0x15365)[0x5600b8f8c365]
[runnervm1li68:05142] *** End of error message ***
</pre>
{% endraw %}
