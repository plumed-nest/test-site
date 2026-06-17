**Project ID:** [plumID:25.015]({{ '/' | absolute_url }}eggs/25/015/)  
Stderr for source:  PLUMED_Inputs/plumed_torsion.dat   
Download: [zipped raw stdout](plumed_torsion.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_torsion.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPATOMS with label @6 : it was not possible to interpret atom name t1_grp
[runnervm1li68:05398] *** Process received signal ***
[runnervm1li68:05398] Signal: Aborted (6)
[runnervm1li68:05398] Signal code:  (-6)
[runnervm1li68:05398] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f10b0845330]
[runnervm1li68:05398] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f10b089eb2c]
[runnervm1li68:05398] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f10b084527e]
[runnervm1li68:05398] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f10b08288ff]
[runnervm1li68:05398] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f10b0ca5ff5]
[runnervm1li68:05398] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f10b0cbb0da]
[runnervm1li68:05398] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f10b0ca5a55]
[runnervm1li68:05398] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f10b0ca5a6f]
[runnervm1li68:05398] [ 8] plumed(+0x146dd)[0x55d840d1a6dd]
[runnervm1li68:05398] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f10b082a1ca]
[runnervm1li68:05398] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f10b082a28b]
[runnervm1li68:05398] [11] plumed(+0x15365)[0x55d840d1b365]
[runnervm1li68:05398] *** End of error message ***
</pre>
{% endraw %}
