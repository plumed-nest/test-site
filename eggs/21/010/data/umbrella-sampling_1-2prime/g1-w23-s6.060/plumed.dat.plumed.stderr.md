**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w23-s6.060/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09783] *** Process received signal ***
[fv-az2027-338:09783] Signal: Aborted (6)
[fv-az2027-338:09783] Signal code:  (-6)
[fv-az2027-338:09783] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd93e045330]
[fv-az2027-338:09783] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd93e09eb2c]
[fv-az2027-338:09783] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd93e04527e]
[fv-az2027-338:09783] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd93e0288ff]
[fv-az2027-338:09783] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd93e4a5ff5]
[fv-az2027-338:09783] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd93e4bb0da]
[fv-az2027-338:09783] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd93e4a5a55]
[fv-az2027-338:09783] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd93e4a5a6f]
[fv-az2027-338:09783] [ 8] plumed(+0x146dd)[0x556affbda6dd]
[fv-az2027-338:09783] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd93e02a1ca]
[fv-az2027-338:09783] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd93e02a28b]
[fv-az2027-338:09783] [11] plumed(+0x15365)[0x556affbdb365]
[fv-az2027-338:09783] *** End of error message ***
</pre>
{% endraw %}
