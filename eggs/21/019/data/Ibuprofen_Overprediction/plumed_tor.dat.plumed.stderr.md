**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATOMS141=9314,9319,9310,9313" is not known.
[runnervm1li68:11278] *** Process received signal ***
[runnervm1li68:11278] Signal: Aborted (6)
[runnervm1li68:11278] Signal code:  (-6)
[runnervm1li68:11278] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe875a45330]
[runnervm1li68:11278] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe875a9eb2c]
[runnervm1li68:11278] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe875a4527e]
[runnervm1li68:11278] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe875a288ff]
[runnervm1li68:11278] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe875ea5ff5]
[runnervm1li68:11278] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe875ebb0da]
[runnervm1li68:11278] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe875ea5a55]
[runnervm1li68:11278] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe875ea5a6f]
[runnervm1li68:11278] [ 8] plumed(+0x146dd)[0x55918d1646dd]
[runnervm1li68:11278] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe875a2a1ca]
[runnervm1li68:11278] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe875a2a28b]
[runnervm1li68:11278] [11] plumed(+0x15365)[0x55918d165365]
[runnervm1li68:11278] *** End of error message ***
</pre>
{% endraw %}
