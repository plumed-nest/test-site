**Project ID:** [plumID:24.009]({{ '/' | absolute_url }}eggs/24/009/)  
Stderr for source:  actin_lda_setup/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "LDA_PROJ" is not known.
[runnervm1li68:05691] *** Process received signal ***
[runnervm1li68:05691] Signal: Aborted (6)
[runnervm1li68:05691] Signal code:  (-6)
[runnervm1li68:05691] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc4eb245330]
[runnervm1li68:05691] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc4eb29eb2c]
[runnervm1li68:05691] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc4eb24527e]
[runnervm1li68:05691] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc4eb2288ff]
[runnervm1li68:05691] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc4eb6a5ff5]
[runnervm1li68:05691] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc4eb6bb0da]
[runnervm1li68:05691] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc4eb6a5a55]
[runnervm1li68:05691] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc4eb6a5a6f]
[runnervm1li68:05691] [ 8] plumed_master(+0x146dd)[0x556c7361f6dd]
[runnervm1li68:05691] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc4eb22a1ca]
[runnervm1li68:05691] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc4eb22a28b]
[runnervm1li68:05691] [11] plumed_master(+0x15365)[0x556c73620365]
[runnervm1li68:05691] *** End of error message ***
</pre>
{% endraw %}
