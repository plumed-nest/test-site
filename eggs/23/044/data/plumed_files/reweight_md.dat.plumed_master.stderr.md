**Project ID:** [plumID:23.044]({{ '/' | absolute_url }}eggs/23/044/)  
Stderr for source:  plumed_files/reweight_md.dat   
Download: [zipped raw stdout](reweight_md.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](reweight_md.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @22 : keyword ARG is compulsory for this action
[runnervm1li68:06084] *** Process received signal ***
[runnervm1li68:06084] Signal: Aborted (6)
[runnervm1li68:06084] Signal code:  (-6)
[runnervm1li68:06084] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9e34645330]
[runnervm1li68:06084] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9e3469eb2c]
[runnervm1li68:06084] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9e3464527e]
[runnervm1li68:06084] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9e346288ff]
[runnervm1li68:06084] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9e34aa5ff5]
[runnervm1li68:06084] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9e34abb0da]
[runnervm1li68:06084] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9e34aa5a55]
[runnervm1li68:06084] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9e34aa5a6f]
[runnervm1li68:06084] [ 8] plumed_master(+0x146dd)[0x55a696ddc6dd]
[runnervm1li68:06084] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9e3462a1ca]
[runnervm1li68:06084] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9e3462a28b]
[runnervm1li68:06084] [11] plumed_master(+0x15365)[0x55a696ddd365]
[runnervm1li68:06084] *** End of error message ***
</pre>
{% endraw %}
