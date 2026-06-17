**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-C/rep2/steered_C_P_2.dat   
Download: [zipped raw stdout](steered_C_P_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](steered_C_P_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04676] *** Process received signal ***
[runnervm1li68:04676] Signal: Aborted (6)
[runnervm1li68:04676] Signal code:  (-6)
[runnervm1li68:04676] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9ab1a45330]
[runnervm1li68:04676] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9ab1a9eb2c]
[runnervm1li68:04676] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9ab1a4527e]
[runnervm1li68:04676] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9ab1a288ff]
[runnervm1li68:04676] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9ab1ea5ff5]
[runnervm1li68:04676] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9ab1ebb0da]
[runnervm1li68:04676] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9ab1ea5a55]
[runnervm1li68:04676] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9ab1ea5a6f]
[runnervm1li68:04676] [ 8] plumed_master(+0x146dd)[0x56120755f6dd]
[runnervm1li68:04676] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9ab1a2a1ca]
[runnervm1li68:04676] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9ab1a2a28b]
[runnervm1li68:04676] [11] plumed_master(+0x15365)[0x561207560365]
[runnervm1li68:04676] *** End of error message ***
</pre>
{% endraw %}
