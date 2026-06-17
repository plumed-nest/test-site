**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  5FU/iMetaD_Input/plumed_imetad.dat   
Download: [zipped raw stdout](plumed_imetad.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_imetad.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action PATH with label @s13 : keyword LAMBDA is compulsory for this action
[runnervm1li68:05916] *** Process received signal ***
[runnervm1li68:05916] Signal: Aborted (6)
[runnervm1li68:05916] Signal code:  (-6)
[runnervm1li68:05916] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7708c45330]
[runnervm1li68:05916] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7708c9eb2c]
[runnervm1li68:05916] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7708c4527e]
[runnervm1li68:05916] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7708c288ff]
[runnervm1li68:05916] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f77090a5ff5]
[runnervm1li68:05916] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f77090bb0da]
[runnervm1li68:05916] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f77090a5a55]
[runnervm1li68:05916] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f77090a5a6f]
[runnervm1li68:05916] [ 8] plumed_master(+0x146dd)[0x55e84c2e06dd]
[runnervm1li68:05916] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7708c2a1ca]
[runnervm1li68:05916] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7708c2a28b]
[runnervm1li68:05916] [11] plumed_master(+0x15365)[0x55e84c2e1365]
[runnervm1li68:05916] *** End of error message ***
</pre>
{% endraw %}
