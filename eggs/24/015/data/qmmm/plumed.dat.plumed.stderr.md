**Project ID:** [plumID:24.015]({{ '/' | absolute_url }}eggs/24/015/)  
Stderr for source:  qmmm/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "PATHCV" is not known.
[fv-az2027-338:05873] *** Process received signal ***
[fv-az2027-338:05873] Signal: Aborted (6)
[fv-az2027-338:05873] Signal code:  (-6)
[fv-az2027-338:05873] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9cb5445330]
[fv-az2027-338:05873] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9cb549eb2c]
[fv-az2027-338:05873] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9cb544527e]
[fv-az2027-338:05873] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9cb54288ff]
[fv-az2027-338:05873] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9cb58a5ff5]
[fv-az2027-338:05873] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9cb58bb0da]
[fv-az2027-338:05873] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9cb58a5a55]
[fv-az2027-338:05873] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9cb58a5a6f]
[fv-az2027-338:05873] [ 8] plumed(+0x146dd)[0x5591022e36dd]
[fv-az2027-338:05873] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9cb542a1ca]
[fv-az2027-338:05873] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9cb542a28b]
[fv-az2027-338:05873] [11] plumed(+0x15365)[0x5591022e4365]
[fv-az2027-338:05873] *** End of error message ***
</pre>
{% endraw %}
