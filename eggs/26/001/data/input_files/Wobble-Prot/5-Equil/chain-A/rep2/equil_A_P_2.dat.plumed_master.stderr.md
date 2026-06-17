**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-A/rep2/equil_A_P_2.dat   
Download: [zipped raw stdout](equil_A_P_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](equil_A_P_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:05038] *** Process received signal ***
[runnervm1li68:05038] Signal: Aborted (6)
[runnervm1li68:05038] Signal code:  (-6)
[runnervm1li68:05038] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2edc045330]
[runnervm1li68:05038] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2edc09eb2c]
[runnervm1li68:05038] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2edc04527e]
[runnervm1li68:05038] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2edc0288ff]
[runnervm1li68:05038] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2edc4a5ff5]
[runnervm1li68:05038] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2edc4bb0da]
[runnervm1li68:05038] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2edc4a5a55]
[runnervm1li68:05038] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2edc4a5a6f]
[runnervm1li68:05038] [ 8] plumed_master(+0x146dd)[0x557a0a2a46dd]
[runnervm1li68:05038] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2edc02a1ca]
[runnervm1li68:05038] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2edc02a28b]
[runnervm1li68:05038] [11] plumed_master(+0x15365)[0x557a0a2a5365]
[runnervm1li68:05038] *** End of error message ***
</pre>
{% endraw %}
