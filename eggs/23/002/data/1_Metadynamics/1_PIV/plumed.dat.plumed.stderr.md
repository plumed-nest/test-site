**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/1_PIV/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[runnervm1li68:07620] *** Process received signal ***
[runnervm1li68:07620] Signal: Aborted (6)
[runnervm1li68:07620] Signal code:  (-6)
[runnervm1li68:07620] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb91f445330]
[runnervm1li68:07620] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb91f49eb2c]
[runnervm1li68:07620] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb91f44527e]
[runnervm1li68:07620] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb91f4288ff]
[runnervm1li68:07620] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb91f8a5ff5]
[runnervm1li68:07620] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb91f8bb0da]
[runnervm1li68:07620] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb91f8a5a55]
[runnervm1li68:07620] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb91f8a5a6f]
[runnervm1li68:07620] [ 8] plumed(+0x146dd)[0x5580b25a86dd]
[runnervm1li68:07620] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb91f42a1ca]
[runnervm1li68:07620] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb91f42a28b]
[runnervm1li68:07620] [11] plumed(+0x15365)[0x5580b25a9365]
[runnervm1li68:07620] *** End of error message ***
</pre>
{% endraw %}
