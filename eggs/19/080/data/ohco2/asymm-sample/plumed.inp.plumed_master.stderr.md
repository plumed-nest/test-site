**Project ID:** [plumID:19.080]({{ '/' | absolute_url }}eggs/19/080/)  
Stderr for source:  ohco2/asymm-sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @24 : keyword ARG is compulsory for this action
[runnervm1li68:09395] *** Process received signal ***
[runnervm1li68:09395] Signal: Aborted (6)
[runnervm1li68:09395] Signal code:  (-6)
[runnervm1li68:09395] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb571045330]
[runnervm1li68:09395] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb57109eb2c]
[runnervm1li68:09395] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb57104527e]
[runnervm1li68:09395] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb5710288ff]
[runnervm1li68:09395] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb5714a5ff5]
[runnervm1li68:09395] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb5714bb0da]
[runnervm1li68:09395] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb5714a5a55]
[runnervm1li68:09395] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb5714a5a6f]
[runnervm1li68:09395] [ 8] plumed_master(+0x146dd)[0x55c1fc7a46dd]
[runnervm1li68:09395] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb57102a1ca]
[runnervm1li68:09395] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb57102a28b]
[runnervm1li68:09395] [11] plumed_master(+0x15365)[0x55c1fc7a5365]
[runnervm1li68:09395] *** End of error message ***
</pre>
{% endraw %}
