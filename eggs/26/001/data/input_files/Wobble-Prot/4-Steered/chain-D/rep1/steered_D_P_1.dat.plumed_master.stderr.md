**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-D/rep1/steered_D_P_1.dat   
Download: [zipped raw stdout](steered_D_P_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](steered_D_P_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04884] *** Process received signal ***
[runnervm1li68:04884] Signal: Aborted (6)
[runnervm1li68:04884] Signal code:  (-6)
[runnervm1li68:04884] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbc94e45330]
[runnervm1li68:04884] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbc94e9eb2c]
[runnervm1li68:04884] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbc94e4527e]
[runnervm1li68:04884] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbc94e288ff]
[runnervm1li68:04884] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbc952a5ff5]
[runnervm1li68:04884] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbc952bb0da]
[runnervm1li68:04884] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbc952a5a55]
[runnervm1li68:04884] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbc952a5a6f]
[runnervm1li68:04884] [ 8] plumed_master(+0x146dd)[0x55d86621c6dd]
[runnervm1li68:04884] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbc94e2a1ca]
[runnervm1li68:04884] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbc94e2a28b]
[runnervm1li68:04884] [11] plumed_master(+0x15365)[0x55d86621d365]
[runnervm1li68:04884] *** End of error message ***
</pre>
{% endraw %}
