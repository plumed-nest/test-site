**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT3_2-Oxiranimine_and_Amoniac/FORCE_ESTIMATION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05605] *** Process received signal ***
[runnervm1li68:05605] Signal: Aborted (6)
[runnervm1li68:05605] Signal code:  (-6)
[runnervm1li68:05605] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f25d1c45330]
[runnervm1li68:05605] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f25d1c9eb2c]
[runnervm1li68:05605] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f25d1c4527e]
[runnervm1li68:05605] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f25d1c288ff]
[runnervm1li68:05605] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f25d20a5ff5]
[runnervm1li68:05605] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f25d20bb0da]
[runnervm1li68:05605] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f25d20a5a55]
[runnervm1li68:05605] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f25d20a5a6f]
[runnervm1li68:05605] [ 8] plumed(+0x146dd)[0x55efba8876dd]
[runnervm1li68:05605] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f25d1c2a1ca]
[runnervm1li68:05605] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f25d1c2a28b]
[runnervm1li68:05605] [11] plumed(+0x15365)[0x55efba888365]
[runnervm1li68:05605] *** End of error message ***
</pre>
{% endraw %}
