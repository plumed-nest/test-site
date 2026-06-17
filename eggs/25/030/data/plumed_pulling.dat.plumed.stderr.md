**Project ID:** [plumID:25.030]({{ '/' | absolute_url }}eggs/25/030/)  
Stderr for source:  plumed_pulling.dat   
Download: [zipped raw stdout](plumed_pulling.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_pulling.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[runnervm1li68:04248] *** Process received signal ***
[runnervm1li68:04248] Signal: Aborted (6)
[runnervm1li68:04248] Signal code:  (-6)
[runnervm1li68:04248] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8524445330]
[runnervm1li68:04248] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f852449eb2c]
[runnervm1li68:04248] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f852444527e]
[runnervm1li68:04248] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f85244288ff]
[runnervm1li68:04248] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f85248a5ff5]
[runnervm1li68:04248] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f85248bb0da]
[runnervm1li68:04248] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f85248a5a55]
[runnervm1li68:04248] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f85248a5a6f]
[runnervm1li68:04248] [ 8] plumed(+0x146dd)[0x55fe06bfe6dd]
[runnervm1li68:04248] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f852442a1ca]
[runnervm1li68:04248] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f852442a28b]
[runnervm1li68:04248] [11] plumed(+0x15365)[0x55fe06bff365]
[runnervm1li68:04248] *** End of error message ***
</pre>
{% endraw %}
