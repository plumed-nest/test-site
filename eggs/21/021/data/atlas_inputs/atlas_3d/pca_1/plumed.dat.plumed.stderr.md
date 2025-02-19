**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_3d/pca_1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:08900] *** Process received signal ***
[fv-az1718-879:08900] Signal: Aborted (6)
[fv-az1718-879:08900] Signal code:  (-6)
[fv-az1718-879:08900] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2af4e45330]
[fv-az1718-879:08900] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2af4e9eb2c]
[fv-az1718-879:08900] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2af4e4527e]
[fv-az1718-879:08900] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2af4e288ff]
[fv-az1718-879:08900] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2af52a5ff5]
[fv-az1718-879:08900] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2af52bb0da]
[fv-az1718-879:08900] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2af52a5a55]
[fv-az1718-879:08900] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2af52a5a6f]
[fv-az1718-879:08900] [ 8] plumed(+0x146dd)[0x556f466966dd]
[fv-az1718-879:08900] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2af4e2a1ca]
[fv-az1718-879:08900] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2af4e2a28b]
[fv-az1718-879:08900] [11] plumed(+0x15365)[0x556f46697365]
[fv-az1718-879:08900] *** End of error message ***
</pre>
{% endraw %}
