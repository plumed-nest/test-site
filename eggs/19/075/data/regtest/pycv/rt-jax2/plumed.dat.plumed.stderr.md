**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[fv-az1372-996:11815] *** Process received signal ***
[fv-az1372-996:11815] Signal: Aborted (6)
[fv-az1372-996:11815] Signal code:  (-6)
[fv-az1372-996:11815] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f930ae45330]
[fv-az1372-996:11815] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f930ae9eb2c]
[fv-az1372-996:11815] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f930ae4527e]
[fv-az1372-996:11815] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f930ae288ff]
[fv-az1372-996:11815] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f930b2a5ff5]
[fv-az1372-996:11815] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f930b2bb0da]
[fv-az1372-996:11815] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f930b2a5a55]
[fv-az1372-996:11815] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f930b2a5a6f]
[fv-az1372-996:11815] [ 8] plumed(+0x146dd)[0x55f0926ac6dd]
[fv-az1372-996:11815] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f930ae2a1ca]
[fv-az1372-996:11815] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f930ae2a28b]
[fv-az1372-996:11815] [11] plumed(+0x15365)[0x55f0926ad365]
[fv-az1372-996:11815] *** End of error message ***
</pre>
{% endraw %}
