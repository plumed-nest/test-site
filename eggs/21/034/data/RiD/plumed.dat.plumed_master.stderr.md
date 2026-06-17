**Project ID:** [plumID:21.034]({{ '/' | absolute_url }}eggs/21/034/)  
Stderr for source:  RiD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "DEEPFE" is not known.
[runnervm1li68:09396] *** Process received signal ***
[runnervm1li68:09396] Signal: Aborted (6)
[runnervm1li68:09396] Signal code:  (-6)
[runnervm1li68:09396] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f943a445330]
[runnervm1li68:09396] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f943a49eb2c]
[runnervm1li68:09396] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f943a44527e]
[runnervm1li68:09396] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f943a4288ff]
[runnervm1li68:09396] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f943a8a5ff5]
[runnervm1li68:09396] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f943a8bb0da]
[runnervm1li68:09396] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f943a8a5a55]
[runnervm1li68:09396] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f943a8a5a6f]
[runnervm1li68:09396] [ 8] plumed_master(+0x146dd)[0x5579979316dd]
[runnervm1li68:09396] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f943a42a1ca]
[runnervm1li68:09396] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f943a42a28b]
[runnervm1li68:09396] [11] plumed_master(+0x15365)[0x557997932365]
[runnervm1li68:09396] *** End of error message ***
</pre>
{% endraw %}
