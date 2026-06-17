**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "SPHERICAL_EXPANSION" is not known.
[runnervm1li68:05645] *** Process received signal ***
[runnervm1li68:05645] Signal: Aborted (6)
[runnervm1li68:05645] Signal code:  (-6)
[runnervm1li68:05645] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcabee45330]
[runnervm1li68:05645] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcabee9eb2c]
[runnervm1li68:05645] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcabee4527e]
[runnervm1li68:05645] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcabee288ff]
[runnervm1li68:05645] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcabf2a5ff5]
[runnervm1li68:05645] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcabf2bb0da]
[runnervm1li68:05645] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcabf2a5a55]
[runnervm1li68:05645] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcabf2a5a6f]
[runnervm1li68:05645] [ 8] plumed_master(+0x146dd)[0x55f0ac8b86dd]
[runnervm1li68:05645] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcabee2a1ca]
[runnervm1li68:05645] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcabee2a28b]
[runnervm1li68:05645] [11] plumed_master(+0x15365)[0x55f0ac8b9365]
[runnervm1li68:05645] *** End of error message ***
</pre>
{% endraw %}
