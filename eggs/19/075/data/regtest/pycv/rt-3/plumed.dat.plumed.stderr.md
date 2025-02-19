**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[fv-az1372-996:11608] *** Process received signal ***
[fv-az1372-996:11608] Signal: Aborted (6)
[fv-az1372-996:11608] Signal code:  (-6)
[fv-az1372-996:11608] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ffb1fe45330]
[fv-az1372-996:11608] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ffb1fe9eb2c]
[fv-az1372-996:11608] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ffb1fe4527e]
[fv-az1372-996:11608] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ffb1fe288ff]
[fv-az1372-996:11608] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ffb202a5ff5]
[fv-az1372-996:11608] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ffb202bb0da]
[fv-az1372-996:11608] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ffb202a5a55]
[fv-az1372-996:11608] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ffb202a5a6f]
[fv-az1372-996:11608] [ 8] plumed(+0x146dd)[0x558b8a2e86dd]
[fv-az1372-996:11608] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ffb1fe2a1ca]
[fv-az1372-996:11608] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ffb1fe2a28b]
[fv-az1372-996:11608] [11] plumed(+0x15365)[0x558b8a2e9365]
[fv-az1372-996:11608] *** End of error message ***
</pre>
{% endraw %}
