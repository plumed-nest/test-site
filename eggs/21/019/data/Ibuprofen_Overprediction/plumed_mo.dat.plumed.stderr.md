**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_mo.dat   
Download: [zipped raw stdout](plumed_mo.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATOMS285=9378,9382" is not known.
[runnervm1li68:11227] *** Process received signal ***
[runnervm1li68:11227] Signal: Aborted (6)
[runnervm1li68:11227] Signal code:  (-6)
[runnervm1li68:11227] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1df7045330]
[runnervm1li68:11227] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1df709eb2c]
[runnervm1li68:11227] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1df704527e]
[runnervm1li68:11227] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1df70288ff]
[runnervm1li68:11227] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1df74a5ff5]
[runnervm1li68:11227] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1df74bb0da]
[runnervm1li68:11227] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1df74a5a55]
[runnervm1li68:11227] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1df74a5a6f]
[runnervm1li68:11227] [ 8] plumed(+0x146dd)[0x55805c83a6dd]
[runnervm1li68:11227] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1df702a1ca]
[runnervm1li68:11227] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1df702a28b]
[runnervm1li68:11227] [11] plumed(+0x15365)[0x55805c83b365]
[runnervm1li68:11227] *** End of error message ***
</pre>
{% endraw %}
