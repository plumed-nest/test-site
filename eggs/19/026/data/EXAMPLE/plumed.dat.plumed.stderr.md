**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HBOND_COORD" is not known.
[runnervm1li68:10930] *** Process received signal ***
[runnervm1li68:10930] Signal: Aborted (6)
[runnervm1li68:10930] Signal code:  (-6)
[runnervm1li68:10930] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7feccc445330]
[runnervm1li68:10930] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7feccc49eb2c]
[runnervm1li68:10930] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7feccc44527e]
[runnervm1li68:10930] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7feccc4288ff]
[runnervm1li68:10930] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7feccc8a5ff5]
[runnervm1li68:10930] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7feccc8bb0da]
[runnervm1li68:10930] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7feccc8a5a55]
[runnervm1li68:10930] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7feccc8a5a6f]
[runnervm1li68:10930] [ 8] plumed(+0x146dd)[0x55a1401536dd]
[runnervm1li68:10930] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7feccc42a1ca]
[runnervm1li68:10930] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7feccc42a28b]
[runnervm1li68:10930] [11] plumed(+0x15365)[0x55a140154365]
[runnervm1li68:10930] *** End of error message ***
</pre>
{% endraw %}
