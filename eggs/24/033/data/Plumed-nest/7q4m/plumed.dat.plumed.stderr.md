**Project ID:** [plumID:24.033]({{ '/' | absolute_url }}eggs/24/033/)  
Stderr for source:  Plumed-nest/7q4m/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action EMMI with label gmm : REWEIGHT can only be used in parallel with 2 or more replicas
[runnervm1li68:05342] *** Process received signal ***
[runnervm1li68:05342] Signal: Aborted (6)
[runnervm1li68:05342] Signal code:  (-6)
[runnervm1li68:05342] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f259cc45330]
[runnervm1li68:05342] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f259cc9eb2c]
[runnervm1li68:05342] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f259cc4527e]
[runnervm1li68:05342] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f259cc288ff]
[runnervm1li68:05342] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f259d0a5ff5]
[runnervm1li68:05342] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f259d0bb0da]
[runnervm1li68:05342] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f259d0a5a55]
[runnervm1li68:05342] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f259d0a5a6f]
[runnervm1li68:05342] [ 8] plumed(+0x146dd)[0x5606dfaca6dd]
[runnervm1li68:05342] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f259cc2a1ca]
[runnervm1li68:05342] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f259cc2a28b]
[runnervm1li68:05342] [11] plumed(+0x15365)[0x5606dfacb365]
[runnervm1li68:05342] *** End of error message ***
</pre>
{% endraw %}
