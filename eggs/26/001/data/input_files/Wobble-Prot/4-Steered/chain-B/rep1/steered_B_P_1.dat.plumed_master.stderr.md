**Project ID:** [plumID:26.001]({{ '/' | absolute_url }}eggs/26/001/)  
Stderr for source:  input_files/Wobble-Prot/4-Steered/chain-B/rep1/steered_B_P_1.dat   
Download: [zipped raw stdout](steered_B_P_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](steered_B_P_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ERMSD with label ermsd : missing input file /leonardo_scratch/large/userexternal/tfernand/Projects/Alx-ribo/A-Prot/ermsd_ref.pdb
[runnervm1li68:04987] *** Process received signal ***
[runnervm1li68:04987] Signal: Aborted (6)
[runnervm1li68:04987] Signal code:  (-6)
[runnervm1li68:04987] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7faf24845330]
[runnervm1li68:04987] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7faf2489eb2c]
[runnervm1li68:04987] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7faf2484527e]
[runnervm1li68:04987] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7faf248288ff]
[runnervm1li68:04987] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7faf24ca5ff5]
[runnervm1li68:04987] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7faf24cbb0da]
[runnervm1li68:04987] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7faf24ca5a55]
[runnervm1li68:04987] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7faf24ca5a6f]
[runnervm1li68:04987] [ 8] plumed_master(+0x146dd)[0x55b3f8c7b6dd]
[runnervm1li68:04987] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7faf2482a1ca]
[runnervm1li68:04987] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7faf2482a28b]
[runnervm1li68:04987] [11] plumed_master(+0x15365)[0x55b3f8c7c365]
[runnervm1li68:04987] *** End of error message ***
</pre>
{% endraw %}
