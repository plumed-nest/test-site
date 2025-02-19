**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  00_Metadynamics/TEST_meta/Test15_longt/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:06533] *** Process received signal ***
[fv-az1947-39:06533] Signal: Aborted (6)
[fv-az1947-39:06533] Signal code:  (-6)
[fv-az1947-39:06533] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3df9a45330]
[fv-az1947-39:06533] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3df9a9eb2c]
[fv-az1947-39:06533] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3df9a4527e]
[fv-az1947-39:06533] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3df9a288ff]
[fv-az1947-39:06533] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3df9ea5ff5]
[fv-az1947-39:06533] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3df9ebb0da]
[fv-az1947-39:06533] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3df9ea5a55]
[fv-az1947-39:06533] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3df9ea5a6f]
[fv-az1947-39:06533] [ 8] plumed(+0x146dd)[0x55988692b6dd]
[fv-az1947-39:06533] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3df9a2a1ca]
[fv-az1947-39:06533] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3df9a2a28b]
[fv-az1947-39:06533] [11] plumed(+0x15365)[0x55988692c365]
[fv-az1947-39:06533] *** End of error message ***
</pre>
{% endraw %}
