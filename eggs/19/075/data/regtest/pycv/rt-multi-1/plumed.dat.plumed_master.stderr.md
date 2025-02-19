**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PYTHONCV" is not known.
[fv-az1372-996:11937] *** Process received signal ***
[fv-az1372-996:11937] Signal: Aborted (6)
[fv-az1372-996:11937] Signal code:  (-6)
[fv-az1372-996:11937] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6b13a45330]
[fv-az1372-996:11937] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6b13a9eb2c]
[fv-az1372-996:11937] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6b13a4527e]
[fv-az1372-996:11937] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6b13a288ff]
[fv-az1372-996:11937] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6b13ea5ff5]
[fv-az1372-996:11937] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6b13ebb0da]
[fv-az1372-996:11937] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6b13ea5a55]
[fv-az1372-996:11937] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6b13ea5a6f]
[fv-az1372-996:11937] [ 8] plumed_master(+0x146dd)[0x55ddd33f76dd]
[fv-az1372-996:11937] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6b13a2a1ca]
[fv-az1372-996:11937] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6b13a2a28b]
[fv-az1372-996:11937] [11] plumed_master(+0x15365)[0x55ddd33f8365]
[fv-az1372-996:11937] *** End of error message ***
</pre>
{% endraw %}
