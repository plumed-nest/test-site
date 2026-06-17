**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT2_Cyanomethanolate_and_Amoniac/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05415] *** Process received signal ***
[runnervm1li68:05415] Signal: Aborted (6)
[runnervm1li68:05415] Signal code:  (-6)
[runnervm1li68:05415] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6a1be45330]
[runnervm1li68:05415] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6a1be9eb2c]
[runnervm1li68:05415] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6a1be4527e]
[runnervm1li68:05415] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6a1be288ff]
[runnervm1li68:05415] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6a1c2a5ff5]
[runnervm1li68:05415] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6a1c2bb0da]
[runnervm1li68:05415] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6a1c2a5a55]
[runnervm1li68:05415] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6a1c2a5a6f]
[runnervm1li68:05415] [ 8] plumed_master(+0x146dd)[0x560e69a706dd]
[runnervm1li68:05415] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6a1be2a1ca]
[runnervm1li68:05415] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6a1be2a28b]
[runnervm1li68:05415] [11] plumed_master(+0x15365)[0x560e69a71365]
[runnervm1li68:05415] *** End of error message ***
</pre>
{% endraw %}
