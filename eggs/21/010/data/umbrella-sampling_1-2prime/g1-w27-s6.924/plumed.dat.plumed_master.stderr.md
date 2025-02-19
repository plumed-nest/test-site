**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w27-s6.924/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:10007] *** Process received signal ***
[fv-az2027-338:10007] Signal: Aborted (6)
[fv-az2027-338:10007] Signal code:  (-6)
[fv-az2027-338:10007] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff652645330]
[fv-az2027-338:10007] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff65269eb2c]
[fv-az2027-338:10007] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff65264527e]
[fv-az2027-338:10007] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff6526288ff]
[fv-az2027-338:10007] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff652aa5ff5]
[fv-az2027-338:10007] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff652abb0da]
[fv-az2027-338:10007] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff652aa5a55]
[fv-az2027-338:10007] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff652aa5a6f]
[fv-az2027-338:10007] [ 8] plumed_master(+0x146dd)[0x55582cdf86dd]
[fv-az2027-338:10007] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff65262a1ca]
[fv-az2027-338:10007] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff65262a28b]
[fv-az2027-338:10007] [11] plumed_master(+0x15365)[0x55582cdf9365]
[fv-az2027-338:10007] *** End of error message ***
</pre>
{% endraw %}
