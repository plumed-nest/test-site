**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATOMS141=9314,9319,9310,9313" is not known.
[fv-az1372-996:10008] *** Process received signal ***
[fv-az1372-996:10008] Signal: Aborted (6)
[fv-az1372-996:10008] Signal code:  (-6)
[fv-az1372-996:10008] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd6ff045330]
[fv-az1372-996:10008] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd6ff09eb2c]
[fv-az1372-996:10008] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd6ff04527e]
[fv-az1372-996:10008] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd6ff0288ff]
[fv-az1372-996:10008] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd6ff4a5ff5]
[fv-az1372-996:10008] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd6ff4bb0da]
[fv-az1372-996:10008] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd6ff4a5a55]
[fv-az1372-996:10008] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd6ff4a5a6f]
[fv-az1372-996:10008] [ 8] plumed(+0x146dd)[0x560faf2696dd]
[fv-az1372-996:10008] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd6ff02a1ca]
[fv-az1372-996:10008] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd6ff02a28b]
[fv-az1372-996:10008] [11] plumed(+0x15365)[0x560faf26a365]
[fv-az1372-996:10008] *** End of error message ***
</pre>
{% endraw %}
