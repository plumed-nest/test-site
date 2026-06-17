**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-D/rep2/steered_D_P_2.dat   
Download: [zipped raw stdout](steered_D_P_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](steered_D_P_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04816] *** Process received signal ***
[runnervm1li68:04816] Signal: Aborted (6)
[runnervm1li68:04816] Signal code:  (-6)
[runnervm1li68:04816] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcf66045330]
[runnervm1li68:04816] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcf6609eb2c]
[runnervm1li68:04816] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcf6604527e]
[runnervm1li68:04816] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcf660288ff]
[runnervm1li68:04816] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcf664a5ff5]
[runnervm1li68:04816] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcf664bb0da]
[runnervm1li68:04816] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcf664a5a55]
[runnervm1li68:04816] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcf664a5a6f]
[runnervm1li68:04816] [ 8] plumed(+0x146dd)[0x564ded0bd6dd]
[runnervm1li68:04816] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcf6602a1ca]
[runnervm1li68:04816] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcf6602a28b]
[runnervm1li68:04816] [11] plumed(+0x15365)[0x564ded0be365]
[runnervm1li68:04816] *** End of error message ***
</pre>
{% endraw %}
