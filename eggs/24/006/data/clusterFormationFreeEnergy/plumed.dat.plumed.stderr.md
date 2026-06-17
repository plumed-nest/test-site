**Project ID:** [plumID:24.006]({{ '/' | absolute_url }}eggs/24/006/)  
Stderr for source:  clusterFormationFreeEnergy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CLUSTER_PROPERTIES with label @s22 : keyword ARG is compulsory for this action
[runnervm1li68:06967] *** Process received signal ***
[runnervm1li68:06967] Signal: Aborted (6)
[runnervm1li68:06967] Signal code:  (-6)
[runnervm1li68:06967] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcc6e045330]
[runnervm1li68:06967] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcc6e09eb2c]
[runnervm1li68:06967] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcc6e04527e]
[runnervm1li68:06967] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcc6e0288ff]
[runnervm1li68:06967] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcc6e4a5ff5]
[runnervm1li68:06967] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcc6e4bb0da]
[runnervm1li68:06967] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcc6e4a5a55]
[runnervm1li68:06967] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcc6e4a5a6f]
[runnervm1li68:06967] [ 8] plumed(+0x146dd)[0x5619d697f6dd]
[runnervm1li68:06967] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcc6e02a1ca]
[runnervm1li68:06967] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcc6e02a28b]
[runnervm1li68:06967] [11] plumed(+0x15365)[0x5619d6980365]
[runnervm1li68:06967] *** End of error message ***
</pre>
{% endraw %}
