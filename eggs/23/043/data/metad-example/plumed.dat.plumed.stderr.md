**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "SPHERICAL_EXPANSION" is not known.
[runnervm1li68:05629] *** Process received signal ***
[runnervm1li68:05629] Signal: Aborted (6)
[runnervm1li68:05629] Signal code:  (-6)
[runnervm1li68:05629] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7dc4245330]
[runnervm1li68:05629] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7dc429eb2c]
[runnervm1li68:05629] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7dc424527e]
[runnervm1li68:05629] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7dc42288ff]
[runnervm1li68:05629] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7dc46a5ff5]
[runnervm1li68:05629] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7dc46bb0da]
[runnervm1li68:05629] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7dc46a5a55]
[runnervm1li68:05629] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7dc46a5a6f]
[runnervm1li68:05629] [ 8] plumed(+0x146dd)[0x56428222b6dd]
[runnervm1li68:05629] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7dc422a1ca]
[runnervm1li68:05629] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7dc422a28b]
[runnervm1li68:05629] [11] plumed(+0x15365)[0x56428222c365]
[runnervm1li68:05629] *** End of error message ***
</pre>
{% endraw %}
