**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[runnervm1li68:10664] *** Process received signal ***
[runnervm1li68:10664] Signal: Aborted (6)
[runnervm1li68:10664] Signal code:  (-6)
[runnervm1li68:10664] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7636245330]
[runnervm1li68:10664] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f763629eb2c]
[runnervm1li68:10664] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f763624527e]
[runnervm1li68:10664] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f76362288ff]
[runnervm1li68:10664] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f76366a5ff5]
[runnervm1li68:10664] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f76366bb0da]
[runnervm1li68:10664] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f76366a5a55]
[runnervm1li68:10664] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f76366a5a6f]
[runnervm1li68:10664] [ 8] plumed_master(+0x146dd)[0x5633dafb76dd]
[runnervm1li68:10664] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f763622a1ca]
[runnervm1li68:10664] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f763622a28b]
[runnervm1li68:10664] [11] plumed_master(+0x15365)[0x5633dafb8365]
[runnervm1li68:10664] *** End of error message ***
</pre>
{% endraw %}
