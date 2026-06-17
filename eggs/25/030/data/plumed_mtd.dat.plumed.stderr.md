**Project ID:** [plumID:25.030]({{ '/' | absolute_url }}eggs/25/030/)  
Stderr for source:  plumed_mtd.dat   
Download: [zipped raw stdout](plumed_mtd.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mtd.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm1li68:04195] *** Process received signal ***
[runnervm1li68:04195] Signal: Aborted (6)
[runnervm1li68:04195] Signal code:  (-6)
[runnervm1li68:04195] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbf2ee45330]
[runnervm1li68:04195] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbf2ee9eb2c]
[runnervm1li68:04195] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbf2ee4527e]
[runnervm1li68:04195] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbf2ee288ff]
[runnervm1li68:04195] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbf2f2a5ff5]
[runnervm1li68:04195] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbf2f2bb0da]
[runnervm1li68:04195] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbf2f2a5a55]
[runnervm1li68:04195] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbf2f2a5a6f]
[runnervm1li68:04195] [ 8] plumed(+0x146dd)[0x5567d3ae56dd]
[runnervm1li68:04195] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbf2ee2a1ca]
[runnervm1li68:04195] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbf2ee2a28b]
[runnervm1li68:04195] [11] plumed(+0x15365)[0x5567d3ae6365]
[runnervm1li68:04195] *** End of error message ***
</pre>
{% endraw %}
