**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w14-s4.116/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09264] *** Process received signal ***
[fv-az2027-338:09264] Signal: Aborted (6)
[fv-az2027-338:09264] Signal code:  (-6)
[fv-az2027-338:09264] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f518a645330]
[fv-az2027-338:09264] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f518a69eb2c]
[fv-az2027-338:09264] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f518a64527e]
[fv-az2027-338:09264] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f518a6288ff]
[fv-az2027-338:09264] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f518aaa5ff5]
[fv-az2027-338:09264] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f518aabb0da]
[fv-az2027-338:09264] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f518aaa5a55]
[fv-az2027-338:09264] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f518aaa5a6f]
[fv-az2027-338:09264] [ 8] plumed(+0x146dd)[0x5577aea856dd]
[fv-az2027-338:09264] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f518a62a1ca]
[fv-az2027-338:09264] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f518a62a28b]
[fv-az2027-338:09264] [11] plumed(+0x15365)[0x5577aea86365]
[fv-az2027-338:09264] *** End of error message ***
</pre>
{% endraw %}
