**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/atlas_6d/res/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09176] *** Process received signal ***
[fv-az1718-879:09176] Signal: Aborted (6)
[fv-az1718-879:09176] Signal code:  (-6)
[fv-az1718-879:09176] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7dda845330]
[fv-az1718-879:09176] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7dda89eb2c]
[fv-az1718-879:09176] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7dda84527e]
[fv-az1718-879:09176] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7dda8288ff]
[fv-az1718-879:09176] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7ddaca5ff5]
[fv-az1718-879:09176] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7ddacbb0da]
[fv-az1718-879:09176] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7ddaca5a55]
[fv-az1718-879:09176] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7ddaca5a6f]
[fv-az1718-879:09176] [ 8] plumed_master(+0x146dd)[0x55b370d646dd]
[fv-az1718-879:09176] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7dda82a1ca]
[fv-az1718-879:09176] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7dda82a28b]
[fv-az1718-879:09176] [11] plumed_master(+0x15365)[0x55b370d65365]
[fv-az1718-879:09176] *** End of error message ***
</pre>
{% endraw %}
