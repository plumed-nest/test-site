**Project ID:** [plumID:25.030]({{ '/' | absolute_url }}eggs/25/030/)  
Stderr for source:  plumed_pulling.dat   
Download: [zipped raw stdout](plumed_pulling.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_pulling.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm1li68:04264] *** Process received signal ***
[runnervm1li68:04264] Signal: Aborted (6)
[runnervm1li68:04264] Signal code:  (-6)
[runnervm1li68:04264] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe9cb045330]
[runnervm1li68:04264] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe9cb09eb2c]
[runnervm1li68:04264] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe9cb04527e]
[runnervm1li68:04264] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe9cb0288ff]
[runnervm1li68:04264] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe9cb4a5ff5]
[runnervm1li68:04264] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe9cb4bb0da]
[runnervm1li68:04264] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe9cb4a5a55]
[runnervm1li68:04264] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe9cb4a5a6f]
[runnervm1li68:04264] [ 8] plumed_master(+0x146dd)[0x559aafc0f6dd]
[runnervm1li68:04264] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe9cb02a1ca]
[runnervm1li68:04264] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe9cb02a28b]
[runnervm1li68:04264] [11] plumed_master(+0x15365)[0x559aafc10365]
[runnervm1li68:04264] *** End of error message ***
</pre>
{% endraw %}
