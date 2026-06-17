**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-A/rep2/equil_A_P_2.dat   
Download: [zipped raw stdout](equil_A_P_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](equil_A_P_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:05022] *** Process received signal ***
[runnervm1li68:05022] Signal: Aborted (6)
[runnervm1li68:05022] Signal code:  (-6)
[runnervm1li68:05022] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff23f045330]
[runnervm1li68:05022] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff23f09eb2c]
[runnervm1li68:05022] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff23f04527e]
[runnervm1li68:05022] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff23f0288ff]
[runnervm1li68:05022] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff23f4a5ff5]
[runnervm1li68:05022] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff23f4bb0da]
[runnervm1li68:05022] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff23f4a5a55]
[runnervm1li68:05022] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff23f4a5a6f]
[runnervm1li68:05022] [ 8] plumed(+0x146dd)[0x55811a65b6dd]
[runnervm1li68:05022] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff23f02a1ca]
[runnervm1li68:05022] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff23f02a28b]
[runnervm1li68:05022] [11] plumed(+0x15365)[0x55811a65c365]
[runnervm1li68:05022] *** End of error message ***
</pre>
{% endraw %}
