**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w1-s1.308/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09007] *** Process received signal ***
[fv-az2027-338:09007] Signal: Aborted (6)
[fv-az2027-338:09007] Signal code:  (-6)
[fv-az2027-338:09007] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbd5a445330]
[fv-az2027-338:09007] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbd5a49eb2c]
[fv-az2027-338:09007] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbd5a44527e]
[fv-az2027-338:09007] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbd5a4288ff]
[fv-az2027-338:09007] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbd5a8a5ff5]
[fv-az2027-338:09007] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbd5a8bb0da]
[fv-az2027-338:09007] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbd5a8a5a55]
[fv-az2027-338:09007] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbd5a8a5a6f]
[fv-az2027-338:09007] [ 8] plumed(+0x146dd)[0x55e5f8f096dd]
[fv-az2027-338:09007] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbd5a42a1ca]
[fv-az2027-338:09007] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbd5a42a28b]
[fv-az2027-338:09007] [11] plumed(+0x15365)[0x55e5f8f0a365]
[fv-az2027-338:09007] *** End of error message ***
</pre>
{% endraw %}
