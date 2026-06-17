**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  00_Metadynamics/TEST_meta/Test15_longt/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:04988] *** Process received signal ***
[runnervm1li68:04988] Signal: Aborted (6)
[runnervm1li68:04988] Signal code:  (-6)
[runnervm1li68:04988] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4eb0845330]
[runnervm1li68:04988] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4eb089eb2c]
[runnervm1li68:04988] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4eb084527e]
[runnervm1li68:04988] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4eb08288ff]
[runnervm1li68:04988] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4eb0ca5ff5]
[runnervm1li68:04988] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4eb0cbb0da]
[runnervm1li68:04988] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4eb0ca5a55]
[runnervm1li68:04988] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4eb0ca5a6f]
[runnervm1li68:04988] [ 8] plumed(+0x146dd)[0x55c4e60086dd]
[runnervm1li68:04988] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4eb082a1ca]
[runnervm1li68:04988] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4eb082a28b]
[runnervm1li68:04988] [11] plumed(+0x15365)[0x55c4e6009365]
[runnervm1li68:04988] *** End of error message ***
</pre>
{% endraw %}
