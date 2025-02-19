**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/di_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09227] *** Process received signal ***
[fv-az1718-879:09227] Signal: Aborted (6)
[fv-az1718-879:09227] Signal code:  (-6)
[fv-az1718-879:09227] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0efd845330]
[fv-az1718-879:09227] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0efd89eb2c]
[fv-az1718-879:09227] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0efd84527e]
[fv-az1718-879:09227] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0efd8288ff]
[fv-az1718-879:09227] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0efdca5ff5]
[fv-az1718-879:09227] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0efdcbb0da]
[fv-az1718-879:09227] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0efdca5a55]
[fv-az1718-879:09227] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0efdca5a6f]
[fv-az1718-879:09227] [ 8] plumed_master(+0x146dd)[0x556956d5f6dd]
[fv-az1718-879:09227] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0efd82a1ca]
[fv-az1718-879:09227] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0efd82a28b]
[fv-az1718-879:09227] [11] plumed_master(+0x15365)[0x556956d60365]
[fv-az1718-879:09227] *** End of error message ***
</pre>
{% endraw %}
