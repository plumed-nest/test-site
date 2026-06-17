**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-C/rep1/steered_C_P_1.dat   
Download: [zipped raw stdout](steered_C_P_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](steered_C_P_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04765] *** Process received signal ***
[runnervm1li68:04765] Signal: Aborted (6)
[runnervm1li68:04765] Signal code:  (-6)
[runnervm1li68:04765] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8dfd245330]
[runnervm1li68:04765] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f8dfd29eb2c]
[runnervm1li68:04765] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f8dfd24527e]
[runnervm1li68:04765] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f8dfd2288ff]
[runnervm1li68:04765] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f8dfd6a5ff5]
[runnervm1li68:04765] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f8dfd6bb0da]
[runnervm1li68:04765] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f8dfd6a5a55]
[runnervm1li68:04765] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f8dfd6a5a6f]
[runnervm1li68:04765] [ 8] plumed(+0x146dd)[0x55c021bf26dd]
[runnervm1li68:04765] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f8dfd22a1ca]
[runnervm1li68:04765] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f8dfd22a28b]
[runnervm1li68:04765] [11] plumed(+0x15365)[0x55c021bf3365]
[runnervm1li68:04765] *** End of error message ***
</pre>
{% endraw %}
