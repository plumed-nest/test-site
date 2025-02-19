**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_6d/pca_1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09072] *** Process received signal ***
[fv-az1718-879:09072] Signal: Aborted (6)
[fv-az1718-879:09072] Signal code:  (-6)
[fv-az1718-879:09072] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1499a45330]
[fv-az1718-879:09072] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1499a9eb2c]
[fv-az1718-879:09072] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1499a4527e]
[fv-az1718-879:09072] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1499a288ff]
[fv-az1718-879:09072] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1499ea5ff5]
[fv-az1718-879:09072] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1499ebb0da]
[fv-az1718-879:09072] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1499ea5a55]
[fv-az1718-879:09072] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1499ea5a6f]
[fv-az1718-879:09072] [ 8] plumed_master(+0x146dd)[0x55dcf98346dd]
[fv-az1718-879:09072] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1499a2a1ca]
[fv-az1718-879:09072] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1499a2a28b]
[fv-az1718-879:09072] [11] plumed_master(+0x15365)[0x55dcf9835365]
[fv-az1718-879:09072] *** End of error message ***
</pre>
{% endraw %}
