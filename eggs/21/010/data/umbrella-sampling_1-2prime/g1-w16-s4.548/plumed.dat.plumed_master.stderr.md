**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w16-s4.548/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az2027-338:09382] *** Process received signal ***
[fv-az2027-338:09382] Signal: Aborted (6)
[fv-az2027-338:09382] Signal code:  (-6)
[fv-az2027-338:09382] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f62d7a45330]
[fv-az2027-338:09382] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f62d7a9eb2c]
[fv-az2027-338:09382] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f62d7a4527e]
[fv-az2027-338:09382] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f62d7a288ff]
[fv-az2027-338:09382] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f62d7ea5ff5]
[fv-az2027-338:09382] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f62d7ebb0da]
[fv-az2027-338:09382] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f62d7ea5a55]
[fv-az2027-338:09382] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f62d7ea5a6f]
[fv-az2027-338:09382] [ 8] plumed_master(+0x146dd)[0x564d4a6ca6dd]
[fv-az2027-338:09382] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f62d7a2a1ca]
[fv-az2027-338:09382] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f62d7a2a28b]
[fv-az2027-338:09382] [11] plumed_master(+0x15365)[0x564d4a6cb365]
[fv-az2027-338:09382] *** End of error message ***
</pre>
{% endraw %}
