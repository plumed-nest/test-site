**Project ID:** [plumID:19.081]({{ '/' | absolute_url }}eggs/19/081/)  
Stderr for source:  Na/03_MultithermalMultibaric/Reweight/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @29 : keyword ARG is compulsory for this action
[runnervm1li68:10509] *** Process received signal ***
[runnervm1li68:10509] Signal: Aborted (6)
[runnervm1li68:10509] Signal code:  (-6)
[runnervm1li68:10509] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f60c4e45330]
[runnervm1li68:10509] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f60c4e9eb2c]
[runnervm1li68:10509] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f60c4e4527e]
[runnervm1li68:10509] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f60c4e288ff]
[runnervm1li68:10509] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f60c52a5ff5]
[runnervm1li68:10509] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f60c52bb0da]
[runnervm1li68:10509] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f60c52a5a55]
[runnervm1li68:10509] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f60c52a5a6f]
[runnervm1li68:10509] [ 8] plumed_master(+0x146dd)[0x5555a74c26dd]
[runnervm1li68:10509] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f60c4e2a1ca]
[runnervm1li68:10509] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f60c4e2a28b]
[runnervm1li68:10509] [11] plumed_master(+0x15365)[0x5555a74c3365]
[runnervm1li68:10509] *** End of error message ***
</pre>
{% endraw %}
