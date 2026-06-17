**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_REWE.dat   
Download: [zipped raw stdout](plumed_REWE.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_REWE.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[runnervm1li68:11419] *** Process received signal ***
[runnervm1li68:11419] Signal: Aborted (6)
[runnervm1li68:11419] Signal code:  (-6)
[runnervm1li68:11419] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4b11245330]
[runnervm1li68:11419] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4b1129eb2c]
[runnervm1li68:11419] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4b1124527e]
[runnervm1li68:11419] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4b112288ff]
[runnervm1li68:11419] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4b116a5ff5]
[runnervm1li68:11419] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4b116bb0da]
[runnervm1li68:11419] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4b116a5a55]
[runnervm1li68:11419] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4b116a5a6f]
[runnervm1li68:11419] [ 8] plumed(+0x146dd)[0x5593c4f806dd]
[runnervm1li68:11419] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4b1122a1ca]
[runnervm1li68:11419] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4b1122a28b]
[runnervm1li68:11419] [11] plumed(+0x15365)[0x5593c4f81365]
[runnervm1li68:11419] *** End of error message ***
</pre>
{% endraw %}
