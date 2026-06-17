**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-A/rep2/steered_A_P_2.dat   
Download: [zipped raw stdout](steered_A_P_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](steered_A_P_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04554] *** Process received signal ***
[runnervm1li68:04554] Signal: Aborted (6)
[runnervm1li68:04554] Signal code:  (-6)
[runnervm1li68:04554] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbb93445330]
[runnervm1li68:04554] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbb9349eb2c]
[runnervm1li68:04554] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbb9344527e]
[runnervm1li68:04554] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbb934288ff]
[runnervm1li68:04554] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbb938a5ff5]
[runnervm1li68:04554] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbb938bb0da]
[runnervm1li68:04554] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbb938a5a55]
[runnervm1li68:04554] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbb938a5a6f]
[runnervm1li68:04554] [ 8] plumed(+0x146dd)[0x56549e5f76dd]
[runnervm1li68:04554] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbb9342a1ca]
[runnervm1li68:04554] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbb9342a28b]
[runnervm1li68:04554] [11] plumed(+0x15365)[0x56549e5f8365]
[runnervm1li68:04554] *** End of error message ***
</pre>
{% endraw %}
