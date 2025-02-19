**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w16-s4.548/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09366] *** Process received signal ***
[fv-az2027-338:09366] Signal: Aborted (6)
[fv-az2027-338:09366] Signal code:  (-6)
[fv-az2027-338:09366] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe88c045330]
[fv-az2027-338:09366] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe88c09eb2c]
[fv-az2027-338:09366] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe88c04527e]
[fv-az2027-338:09366] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe88c0288ff]
[fv-az2027-338:09366] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe88c4a5ff5]
[fv-az2027-338:09366] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe88c4bb0da]
[fv-az2027-338:09366] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe88c4a5a55]
[fv-az2027-338:09366] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe88c4a5a6f]
[fv-az2027-338:09366] [ 8] plumed(+0x146dd)[0x563dac1cd6dd]
[fv-az2027-338:09366] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe88c02a1ca]
[fv-az2027-338:09366] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe88c02a28b]
[fv-az2027-338:09366] [11] plumed(+0x15365)[0x563dac1ce365]
[fv-az2027-338:09366] *** End of error message ***
</pre>
{% endraw %}
