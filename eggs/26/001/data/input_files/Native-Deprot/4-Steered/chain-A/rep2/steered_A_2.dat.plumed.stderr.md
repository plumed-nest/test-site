**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Native-Deprot/4-Steered/chain-A/rep2/steered_A_2.dat   
Download: [zipped raw stdout](steered_A_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](steered_A_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Deprot/ermsd_ref.pdb
[runnervm1li68:05487] *** Process received signal ***
[runnervm1li68:05487] Signal: Aborted (6)
[runnervm1li68:05487] Signal code:  (-6)
[runnervm1li68:05487] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fde8fa45330]
[runnervm1li68:05487] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fde8fa9eb2c]
[runnervm1li68:05487] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fde8fa4527e]
[runnervm1li68:05487] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fde8fa288ff]
[runnervm1li68:05487] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fde8fea5ff5]
[runnervm1li68:05487] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fde8febb0da]
[runnervm1li68:05487] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fde8fea5a55]
[runnervm1li68:05487] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fde8fea5a6f]
[runnervm1li68:05487] [ 8] plumed(+0x146dd)[0x56277216d6dd]
[runnervm1li68:05487] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fde8fa2a1ca]
[runnervm1li68:05487] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fde8fa2a28b]
[runnervm1li68:05487] [11] plumed(+0x15365)[0x56277216e365]
[runnervm1li68:05487] *** End of error message ***
</pre>
{% endraw %}
