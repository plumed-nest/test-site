**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Native-Deprot/4-Steered/chain-A/rep1/steered_A_1.dat   
Download: [zipped raw stdout](steered_A_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](steered_A_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Deprot/ermsd_ref.pdb
[runnervm1li68:05538] *** Process received signal ***
[runnervm1li68:05538] Signal: Aborted (6)
[runnervm1li68:05538] Signal code:  (-6)
[runnervm1li68:05538] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9e99a45330]
[runnervm1li68:05538] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9e99a9eb2c]
[runnervm1li68:05538] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9e99a4527e]
[runnervm1li68:05538] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9e99a288ff]
[runnervm1li68:05538] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9e99ea5ff5]
[runnervm1li68:05538] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9e99ebb0da]
[runnervm1li68:05538] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9e99ea5a55]
[runnervm1li68:05538] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9e99ea5a6f]
[runnervm1li68:05538] [ 8] plumed(+0x146dd)[0x55a7b1f946dd]
[runnervm1li68:05538] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9e99a2a1ca]
[runnervm1li68:05538] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9e99a2a28b]
[runnervm1li68:05538] [11] plumed(+0x15365)[0x55a7b1f95365]
[runnervm1li68:05538] *** End of error message ***
</pre>
{% endraw %}
