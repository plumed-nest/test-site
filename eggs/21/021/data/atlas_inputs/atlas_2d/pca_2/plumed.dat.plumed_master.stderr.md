**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_2d/pca_2/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:08864] *** Process received signal ***
[fv-az1718-879:08864] Signal: Aborted (6)
[fv-az1718-879:08864] Signal code:  (-6)
[fv-az1718-879:08864] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7ec9645330]
[fv-az1718-879:08864] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7ec969eb2c]
[fv-az1718-879:08864] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7ec964527e]
[fv-az1718-879:08864] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7ec96288ff]
[fv-az1718-879:08864] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7ec9aa5ff5]
[fv-az1718-879:08864] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7ec9abb0da]
[fv-az1718-879:08864] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7ec9aa5a55]
[fv-az1718-879:08864] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7ec9aa5a6f]
[fv-az1718-879:08864] [ 8] plumed_master(+0x146dd)[0x562b4477c6dd]
[fv-az1718-879:08864] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7ec962a1ca]
[fv-az1718-879:08864] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7ec962a28b]
[fv-az1718-879:08864] [11] plumed_master(+0x15365)[0x562b4477d365]
[fv-az1718-879:08864] *** End of error message ***
</pre>
{% endraw %}
