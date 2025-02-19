**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/tetra_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09279] *** Process received signal ***
[fv-az1718-879:09279] Signal: Aborted (6)
[fv-az1718-879:09279] Signal code:  (-6)
[fv-az1718-879:09279] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd299645330]
[fv-az1718-879:09279] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd29969eb2c]
[fv-az1718-879:09279] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd29964527e]
[fv-az1718-879:09279] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd2996288ff]
[fv-az1718-879:09279] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd299aa5ff5]
[fv-az1718-879:09279] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd299abb0da]
[fv-az1718-879:09279] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd299aa5a55]
[fv-az1718-879:09279] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd299aa5a6f]
[fv-az1718-879:09279] [ 8] plumed_master(+0x146dd)[0x561f79ca06dd]
[fv-az1718-879:09279] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd29962a1ca]
[fv-az1718-879:09279] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd29962a28b]
[fv-az1718-879:09279] [11] plumed_master(+0x15365)[0x561f79ca1365]
[fv-az1718-879:09279] *** End of error message ***
</pre>
{% endraw %}
