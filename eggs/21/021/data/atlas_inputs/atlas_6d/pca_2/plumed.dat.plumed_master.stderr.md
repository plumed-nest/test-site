**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_6d/pca_2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09124] *** Process received signal ***
[fv-az1718-879:09124] Signal: Aborted (6)
[fv-az1718-879:09124] Signal code:  (-6)
[fv-az1718-879:09124] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd2fa445330]
[fv-az1718-879:09124] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd2fa49eb2c]
[fv-az1718-879:09124] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd2fa44527e]
[fv-az1718-879:09124] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd2fa4288ff]
[fv-az1718-879:09124] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd2fa8a5ff5]
[fv-az1718-879:09124] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd2fa8bb0da]
[fv-az1718-879:09124] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd2fa8a5a55]
[fv-az1718-879:09124] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd2fa8a5a6f]
[fv-az1718-879:09124] [ 8] plumed_master(+0x146dd)[0x5622d655d6dd]
[fv-az1718-879:09124] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd2fa42a1ca]
[fv-az1718-879:09124] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd2fa42a28b]
[fv-az1718-879:09124] [11] plumed_master(+0x15365)[0x5622d655e365]
[fv-az1718-879:09124] *** End of error message ***
</pre>
{% endraw %}
