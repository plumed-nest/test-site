**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONFUNCTION" is not known.
[fv-az1372-996:11713] *** Process received signal ***
[fv-az1372-996:11713] Signal: Aborted (6)
[fv-az1372-996:11713] Signal code:  (-6)
[fv-az1372-996:11713] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6c67c45330]
[fv-az1372-996:11713] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6c67c9eb2c]
[fv-az1372-996:11713] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6c67c4527e]
[fv-az1372-996:11713] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6c67c288ff]
[fv-az1372-996:11713] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6c680a5ff5]
[fv-az1372-996:11713] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6c680bb0da]
[fv-az1372-996:11713] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6c680a5a55]
[fv-az1372-996:11713] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6c680a5a6f]
[fv-az1372-996:11713] [ 8] plumed(+0x146dd)[0x562af1cf96dd]
[fv-az1372-996:11713] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6c67c2a1ca]
[fv-az1372-996:11713] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6c67c2a28b]
[fv-az1372-996:11713] [11] plumed(+0x15365)[0x562af1cfa365]
[fv-az1372-996:11713] *** End of error message ***
</pre>
{% endraw %}
