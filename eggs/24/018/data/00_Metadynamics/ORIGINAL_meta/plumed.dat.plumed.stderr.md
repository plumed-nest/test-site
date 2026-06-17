**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  00_Metadynamics/ORIGINAL_meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:04679] *** Process received signal ***
[runnervm1li68:04679] Signal: Aborted (6)
[runnervm1li68:04679] Signal code:  (-6)
[runnervm1li68:04679] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5b95a45330]
[runnervm1li68:04679] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5b95a9eb2c]
[runnervm1li68:04679] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5b95a4527e]
[runnervm1li68:04679] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5b95a288ff]
[runnervm1li68:04679] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5b95ea5ff5]
[runnervm1li68:04679] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5b95ebb0da]
[runnervm1li68:04679] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5b95ea5a55]
[runnervm1li68:04679] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5b95ea5a6f]
[runnervm1li68:04679] [ 8] plumed(+0x146dd)[0x564a2be456dd]
[runnervm1li68:04679] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5b95a2a1ca]
[runnervm1li68:04679] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5b95a2a28b]
[runnervm1li68:04679] [11] plumed(+0x15365)[0x564a2be46365]
[runnervm1li68:04679] *** End of error message ***
</pre>
{% endraw %}
