**Project ID:** [plumID:21.011]({{ '/' | absolute_url }}eggs/21/011/)  
Stderr for source:  NaCl_at_graphite-cmumd/coordination-profiles.plmd   
Download: [zipped raw stdout](coordination-profiles.plmd.plumed_master.stdout.txt.zip) - [zipped raw stderr](coordination-profiles.plmd.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'std::out_of_range'
what():  map::at
[runnervm1li68:09835] *** Process received signal ***
[runnervm1li68:09835] Signal: Aborted (6)
[runnervm1li68:09835] Signal code:  (-6)
[runnervm1li68:09835] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9cf5a45330]
[runnervm1li68:09835] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9cf5a9eb2c]
[runnervm1li68:09835] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9cf5a4527e]
[runnervm1li68:09835] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9cf5a288ff]
[runnervm1li68:09835] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9cf5ea5ff5]
[runnervm1li68:09835] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9cf5ebb0da]
[runnervm1li68:09835] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9cf5ea5a55]
[runnervm1li68:09835] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9cf5ea5a6f]
[runnervm1li68:09835] [ 8] plumed_master(+0x146dd)[0x55a182ff16dd]
[runnervm1li68:09835] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9cf5a2a1ca]
[runnervm1li68:09835] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9cf5a2a28b]
[runnervm1li68:09835] [11] plumed_master(+0x15365)[0x55a182ff2365]
[runnervm1li68:09835] *** End of error message ***
</pre>
{% endraw %}
