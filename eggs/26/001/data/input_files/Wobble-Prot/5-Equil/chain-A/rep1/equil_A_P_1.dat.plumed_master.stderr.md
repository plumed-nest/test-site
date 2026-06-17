**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/5-Equil/chain-A/rep1/equil_A_P_1.dat   
Download: [zipped raw stdout](equil_A_P_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](equil_A_P_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:05089] *** Process received signal ***
[runnervm1li68:05089] Signal: Aborted (6)
[runnervm1li68:05089] Signal code:  (-6)
[runnervm1li68:05089] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f810aa45330]
[runnervm1li68:05089] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f810aa9eb2c]
[runnervm1li68:05089] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f810aa4527e]
[runnervm1li68:05089] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f810aa288ff]
[runnervm1li68:05089] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f810aea5ff5]
[runnervm1li68:05089] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f810aebb0da]
[runnervm1li68:05089] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f810aea5a55]
[runnervm1li68:05089] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f810aea5a6f]
[runnervm1li68:05089] [ 8] plumed_master(+0x146dd)[0x562636bb86dd]
[runnervm1li68:05089] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f810aa2a1ca]
[runnervm1li68:05089] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f810aa2a28b]
[runnervm1li68:05089] [11] plumed_master(+0x15365)[0x562636bb9365]
[runnervm1li68:05089] *** End of error message ***
</pre>
{% endraw %}
