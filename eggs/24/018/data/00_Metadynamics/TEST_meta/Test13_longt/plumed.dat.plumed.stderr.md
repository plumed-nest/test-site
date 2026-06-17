**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  00_Metadynamics/TEST_meta/Test13_longt/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:04885] *** Process received signal ***
[runnervm1li68:04885] Signal: Aborted (6)
[runnervm1li68:04885] Signal code:  (-6)
[runnervm1li68:04885] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8f2e245330]
[runnervm1li68:04885] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f8f2e29eb2c]
[runnervm1li68:04885] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f8f2e24527e]
[runnervm1li68:04885] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f8f2e2288ff]
[runnervm1li68:04885] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f8f2e6a5ff5]
[runnervm1li68:04885] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f8f2e6bb0da]
[runnervm1li68:04885] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f8f2e6a5a55]
[runnervm1li68:04885] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f8f2e6a5a6f]
[runnervm1li68:04885] [ 8] plumed(+0x146dd)[0x556aafa146dd]
[runnervm1li68:04885] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f8f2e22a1ca]
[runnervm1li68:04885] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f8f2e22a28b]
[runnervm1li68:04885] [11] plumed(+0x15365)[0x556aafa15365]
[runnervm1li68:04885] *** End of error message ***
</pre>
{% endraw %}
