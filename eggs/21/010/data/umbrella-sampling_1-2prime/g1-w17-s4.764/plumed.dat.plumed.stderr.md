**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w17-s4.764/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09419] *** Process received signal ***
[fv-az2027-338:09419] Signal: Aborted (6)
[fv-az2027-338:09419] Signal code:  (-6)
[fv-az2027-338:09419] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f37ff245330]
[fv-az2027-338:09419] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f37ff29eb2c]
[fv-az2027-338:09419] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f37ff24527e]
[fv-az2027-338:09419] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f37ff2288ff]
[fv-az2027-338:09419] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f37ff6a5ff5]
[fv-az2027-338:09419] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f37ff6bb0da]
[fv-az2027-338:09419] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f37ff6a5a55]
[fv-az2027-338:09419] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f37ff6a5a6f]
[fv-az2027-338:09419] [ 8] plumed(+0x146dd)[0x561a33d0b6dd]
[fv-az2027-338:09419] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f37ff22a1ca]
[fv-az2027-338:09419] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f37ff22a28b]
[fv-az2027-338:09419] [11] plumed(+0x15365)[0x561a33d0c365]
[fv-az2027-338:09419] *** End of error message ***
</pre>
{% endraw %}
