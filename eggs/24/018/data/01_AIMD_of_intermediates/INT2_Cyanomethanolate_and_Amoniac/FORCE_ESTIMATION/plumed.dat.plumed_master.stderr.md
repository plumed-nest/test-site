**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT2_Cyanomethanolate_and_Amoniac/FORCE_ESTIMATION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:06911] *** Process received signal ***
[fv-az1947-39:06911] Signal: Aborted (6)
[fv-az1947-39:06911] Signal code:  (-6)
[fv-az1947-39:06911] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7a06445330]
[fv-az1947-39:06911] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7a0649eb2c]
[fv-az1947-39:06911] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7a0644527e]
[fv-az1947-39:06911] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7a064288ff]
[fv-az1947-39:06911] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7a068a5ff5]
[fv-az1947-39:06911] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7a068bb0da]
[fv-az1947-39:06911] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7a068a5a55]
[fv-az1947-39:06911] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7a068a5a6f]
[fv-az1947-39:06911] [ 8] plumed_master(+0x146dd)[0x56300c8f96dd]
[fv-az1947-39:06911] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7a0642a1ca]
[fv-az1947-39:06911] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7a0642a28b]
[fv-az1947-39:06911] [11] plumed_master(+0x15365)[0x56300c8fa365]
[fv-az1947-39:06911] *** End of error message ***
</pre>
{% endraw %}
