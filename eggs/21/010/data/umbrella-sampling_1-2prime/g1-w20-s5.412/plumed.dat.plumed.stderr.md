**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w20-s5.412/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09629] *** Process received signal ***
[fv-az2027-338:09629] Signal: Aborted (6)
[fv-az2027-338:09629] Signal code:  (-6)
[fv-az2027-338:09629] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2e39845330]
[fv-az2027-338:09629] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2e3989eb2c]
[fv-az2027-338:09629] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2e3984527e]
[fv-az2027-338:09629] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2e398288ff]
[fv-az2027-338:09629] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2e39ca5ff5]
[fv-az2027-338:09629] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2e39cbb0da]
[fv-az2027-338:09629] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2e39ca5a55]
[fv-az2027-338:09629] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2e39ca5a6f]
[fv-az2027-338:09629] [ 8] plumed(+0x146dd)[0x56302fc486dd]
[fv-az2027-338:09629] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2e3982a1ca]
[fv-az2027-338:09629] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2e3982a28b]
[fv-az2027-338:09629] [11] plumed(+0x15365)[0x56302fc49365]
[fv-az2027-338:09629] *** End of error message ***
</pre>
{% endraw %}
