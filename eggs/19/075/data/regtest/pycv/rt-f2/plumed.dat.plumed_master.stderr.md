**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONFUNCTION" is not known.
[fv-az1372-996:11729] *** Process received signal ***
[fv-az1372-996:11729] Signal: Aborted (6)
[fv-az1372-996:11729] Signal code:  (-6)
[fv-az1372-996:11729] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8441a45330]
[fv-az1372-996:11729] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f8441a9eb2c]
[fv-az1372-996:11729] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f8441a4527e]
[fv-az1372-996:11729] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f8441a288ff]
[fv-az1372-996:11729] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f8441ea5ff5]
[fv-az1372-996:11729] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f8441ebb0da]
[fv-az1372-996:11729] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f8441ea5a55]
[fv-az1372-996:11729] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f8441ea5a6f]
[fv-az1372-996:11729] [ 8] plumed_master(+0x146dd)[0x56458f5136dd]
[fv-az1372-996:11729] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f8441a2a1ca]
[fv-az1372-996:11729] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f8441a2a28b]
[fv-az1372-996:11729] [11] plumed_master(+0x15365)[0x56458f514365]
[fv-az1372-996:11729] *** End of error message ***
</pre>
{% endraw %}
