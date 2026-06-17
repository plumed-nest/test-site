**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT2pr_Hydroxydeacetonitrile_and_Amoniac/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05553] *** Process received signal ***
[runnervm1li68:05553] Signal: Aborted (6)
[runnervm1li68:05553] Signal code:  (-6)
[runnervm1li68:05553] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f25c4a45330]
[runnervm1li68:05553] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f25c4a9eb2c]
[runnervm1li68:05553] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f25c4a4527e]
[runnervm1li68:05553] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f25c4a288ff]
[runnervm1li68:05553] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f25c4ea5ff5]
[runnervm1li68:05553] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f25c4ebb0da]
[runnervm1li68:05553] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f25c4ea5a55]
[runnervm1li68:05553] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f25c4ea5a6f]
[runnervm1li68:05553] [ 8] plumed(+0x146dd)[0x5582989a86dd]
[runnervm1li68:05553] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f25c4a2a1ca]
[runnervm1li68:05553] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f25c4a2a28b]
[runnervm1li68:05553] [11] plumed(+0x15365)[0x5582989a9365]
[runnervm1li68:05553] *** End of error message ***
</pre>
{% endraw %}
