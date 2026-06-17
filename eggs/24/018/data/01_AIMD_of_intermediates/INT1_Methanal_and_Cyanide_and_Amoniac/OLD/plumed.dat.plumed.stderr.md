**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT1_Methanal_and_Cyanide_and_Amoniac/OLD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[runnervm1li68:05247] *** Process received signal ***
[runnervm1li68:05247] Signal: Aborted (6)
[runnervm1li68:05247] Signal code:  (-6)
[runnervm1li68:05247] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f134fe45330]
[runnervm1li68:05247] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f134fe9eb2c]
[runnervm1li68:05247] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f134fe4527e]
[runnervm1li68:05247] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f134fe288ff]
[runnervm1li68:05247] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f13502a5ff5]
[runnervm1li68:05247] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f13502bb0da]
[runnervm1li68:05247] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f13502a5a55]
[runnervm1li68:05247] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f13502a5a6f]
[runnervm1li68:05247] [ 8] plumed(+0x146dd)[0x560b706ad6dd]
[runnervm1li68:05247] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f134fe2a1ca]
[runnervm1li68:05247] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f134fe2a28b]
[runnervm1li68:05247] [11] plumed(+0x15365)[0x560b706ae365]
[runnervm1li68:05247] *** End of error message ***
</pre>
{% endraw %}
