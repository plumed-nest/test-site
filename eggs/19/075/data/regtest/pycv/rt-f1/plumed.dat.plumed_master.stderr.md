**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONFUNCTION" is not known.
[fv-az1372-996:11676] *** Process received signal ***
[fv-az1372-996:11676] Signal: Aborted (6)
[fv-az1372-996:11676] Signal code:  (-6)
[fv-az1372-996:11676] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7faf7a845330]
[fv-az1372-996:11676] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7faf7a89eb2c]
[fv-az1372-996:11676] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7faf7a84527e]
[fv-az1372-996:11676] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7faf7a8288ff]
[fv-az1372-996:11676] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7faf7aca5ff5]
[fv-az1372-996:11676] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7faf7acbb0da]
[fv-az1372-996:11676] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7faf7aca5a55]
[fv-az1372-996:11676] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7faf7aca5a6f]
[fv-az1372-996:11676] [ 8] plumed_master(+0x146dd)[0x55ed0a4d86dd]
[fv-az1372-996:11676] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7faf7a82a1ca]
[fv-az1372-996:11676] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7faf7a82a28b]
[fv-az1372-996:11676] [11] plumed_master(+0x15365)[0x55ed0a4d9365]
[fv-az1372-996:11676] *** End of error message ***
</pre>
{% endraw %}
