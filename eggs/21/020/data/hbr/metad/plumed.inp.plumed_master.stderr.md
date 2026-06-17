**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  hbr/metad/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s31 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:09326] *** Process received signal ***
[runnervm1li68:09326] Signal: Aborted (6)
[runnervm1li68:09326] Signal code:  (-6)
[runnervm1li68:09326] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbb35645330]
[runnervm1li68:09326] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbb3569eb2c]
[runnervm1li68:09326] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbb3564527e]
[runnervm1li68:09326] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbb356288ff]
[runnervm1li68:09326] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbb35aa5ff5]
[runnervm1li68:09326] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbb35abb0da]
[runnervm1li68:09326] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbb35aa5a55]
[runnervm1li68:09326] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbb35aa5a6f]
[runnervm1li68:09326] [ 8] plumed_master(+0x146dd)[0x561de1bc06dd]
[runnervm1li68:09326] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbb3562a1ca]
[runnervm1li68:09326] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbb3562a28b]
[runnervm1li68:09326] [11] plumed_master(+0x15365)[0x561de1bc1365]
[runnervm1li68:09326] *** End of error message ***
</pre>
{% endraw %}
