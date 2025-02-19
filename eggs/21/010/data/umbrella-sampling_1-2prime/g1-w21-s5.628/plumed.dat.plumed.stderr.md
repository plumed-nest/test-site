**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w21-s5.628/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09680] *** Process received signal ***
[fv-az2027-338:09680] Signal: Aborted (6)
[fv-az2027-338:09680] Signal code:  (-6)
[fv-az2027-338:09680] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f73b3445330]
[fv-az2027-338:09680] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f73b349eb2c]
[fv-az2027-338:09680] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f73b344527e]
[fv-az2027-338:09680] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f73b34288ff]
[fv-az2027-338:09680] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f73b38a5ff5]
[fv-az2027-338:09680] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f73b38bb0da]
[fv-az2027-338:09680] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f73b38a5a55]
[fv-az2027-338:09680] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f73b38a5a6f]
[fv-az2027-338:09680] [ 8] plumed(+0x146dd)[0x564e3d7166dd]
[fv-az2027-338:09680] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f73b342a1ca]
[fv-az2027-338:09680] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f73b342a28b]
[fv-az2027-338:09680] [11] plumed(+0x15365)[0x564e3d717365]
[fv-az2027-338:09680] *** End of error message ***
</pre>
{% endraw %}
