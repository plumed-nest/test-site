**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT3_2-Oxiranimine_and_Amoniac/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05657] *** Process received signal ***
[runnervm1li68:05657] Signal: Aborted (6)
[runnervm1li68:05657] Signal code:  (-6)
[runnervm1li68:05657] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9a7fa45330]
[runnervm1li68:05657] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9a7fa9eb2c]
[runnervm1li68:05657] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9a7fa4527e]
[runnervm1li68:05657] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9a7fa288ff]
[runnervm1li68:05657] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9a7fea5ff5]
[runnervm1li68:05657] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9a7febb0da]
[runnervm1li68:05657] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9a7fea5a55]
[runnervm1li68:05657] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9a7fea5a6f]
[runnervm1li68:05657] [ 8] plumed(+0x146dd)[0x55b0743436dd]
[runnervm1li68:05657] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9a7fa2a1ca]
[runnervm1li68:05657] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9a7fa2a28b]
[runnervm1li68:05657] [11] plumed(+0x15365)[0x55b074344365]
[runnervm1li68:05657] *** End of error message ***
</pre>
{% endraw %}
