**Project ID:** [plumID:21.034]({{ '/' | absolute_url }}eggs/21/034/)  
Stderr for source:  RiD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "DEEPFE" is not known.
[fv-az1718-879:08070] *** Process received signal ***
[fv-az1718-879:08070] Signal: Aborted (6)
[fv-az1718-879:08070] Signal code:  (-6)
[fv-az1718-879:08070] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbc8b245330]
[fv-az1718-879:08070] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbc8b29eb2c]
[fv-az1718-879:08070] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbc8b24527e]
[fv-az1718-879:08070] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbc8b2288ff]
[fv-az1718-879:08070] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbc8b6a5ff5]
[fv-az1718-879:08070] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbc8b6bb0da]
[fv-az1718-879:08070] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbc8b6a5a55]
[fv-az1718-879:08070] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbc8b6a5a6f]
[fv-az1718-879:08070] [ 8] plumed_master(+0x146dd)[0x55b19be546dd]
[fv-az1718-879:08070] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbc8b22a1ca]
[fv-az1718-879:08070] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbc8b22a28b]
[fv-az1718-879:08070] [11] plumed_master(+0x15365)[0x55b19be55365]
[fv-az1718-879:08070] *** End of error message ***
</pre>
{% endraw %}
