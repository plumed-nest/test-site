**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/di_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09211] *** Process received signal ***
[fv-az1718-879:09211] Signal: Aborted (6)
[fv-az1718-879:09211] Signal code:  (-6)
[fv-az1718-879:09211] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0fe9e45330]
[fv-az1718-879:09211] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0fe9e9eb2c]
[fv-az1718-879:09211] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0fe9e4527e]
[fv-az1718-879:09211] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0fe9e288ff]
[fv-az1718-879:09211] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0fea2a5ff5]
[fv-az1718-879:09211] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0fea2bb0da]
[fv-az1718-879:09211] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0fea2a5a55]
[fv-az1718-879:09211] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0fea2a5a6f]
[fv-az1718-879:09211] [ 8] plumed(+0x146dd)[0x5559cce3a6dd]
[fv-az1718-879:09211] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0fe9e2a1ca]
[fv-az1718-879:09211] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0fe9e2a28b]
[fv-az1718-879:09211] [11] plumed(+0x15365)[0x5559cce3b365]
[fv-az1718-879:09211] *** End of error message ***
</pre>
{% endraw %}
