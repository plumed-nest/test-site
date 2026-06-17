**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT3_2-Oxiranimine_and_Amoniac/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05673] *** Process received signal ***
[runnervm1li68:05673] Signal: Aborted (6)
[runnervm1li68:05673] Signal code:  (-6)
[runnervm1li68:05673] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7feee2445330]
[runnervm1li68:05673] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7feee249eb2c]
[runnervm1li68:05673] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7feee244527e]
[runnervm1li68:05673] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7feee24288ff]
[runnervm1li68:05673] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7feee28a5ff5]
[runnervm1li68:05673] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7feee28bb0da]
[runnervm1li68:05673] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7feee28a5a55]
[runnervm1li68:05673] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7feee28a5a6f]
[runnervm1li68:05673] [ 8] plumed_master(+0x146dd)[0x55722529c6dd]
[runnervm1li68:05673] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7feee242a1ca]
[runnervm1li68:05673] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7feee242a28b]
[runnervm1li68:05673] [11] plumed_master(+0x15365)[0x55722529d365]
[runnervm1li68:05673] *** End of error message ***
</pre>
{% endraw %}
