**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATOMS141=9314,9319,9310,9313" is not known.
[fv-az1372-996:10024] *** Process received signal ***
[fv-az1372-996:10024] Signal: Aborted (6)
[fv-az1372-996:10024] Signal code:  (-6)
[fv-az1372-996:10024] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcf05445330]
[fv-az1372-996:10024] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcf0549eb2c]
[fv-az1372-996:10024] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcf0544527e]
[fv-az1372-996:10024] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcf054288ff]
[fv-az1372-996:10024] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcf058a5ff5]
[fv-az1372-996:10024] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcf058bb0da]
[fv-az1372-996:10024] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcf058a5a55]
[fv-az1372-996:10024] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcf058a5a6f]
[fv-az1372-996:10024] [ 8] plumed_master(+0x146dd)[0x55ae4b2496dd]
[fv-az1372-996:10024] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcf0542a1ca]
[fv-az1372-996:10024] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcf0542a28b]
[fv-az1372-996:10024] [11] plumed_master(+0x15365)[0x55ae4b24a365]
[fv-az1372-996:10024] *** End of error message ***
</pre>
{% endraw %}
