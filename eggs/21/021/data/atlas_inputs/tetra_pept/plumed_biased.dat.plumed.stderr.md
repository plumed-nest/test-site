**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  atlas_inputs/tetra_pept/plumed_biased.dat   
Download: [zipped raw stdout](plumed_biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:09262] *** Process received signal ***
[fv-az1718-879:09262] Signal: Aborted (6)
[fv-az1718-879:09262] Signal code:  (-6)
[fv-az1718-879:09262] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcb0ce45330]
[fv-az1718-879:09262] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcb0ce9eb2c]
[fv-az1718-879:09262] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcb0ce4527e]
[fv-az1718-879:09262] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcb0ce288ff]
[fv-az1718-879:09262] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcb0d2a5ff5]
[fv-az1718-879:09262] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcb0d2bb0da]
[fv-az1718-879:09262] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcb0d2a5a55]
[fv-az1718-879:09262] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcb0d2a5a6f]
[fv-az1718-879:09262] [ 8] plumed(+0x146dd)[0x560ca32216dd]
[fv-az1718-879:09262] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcb0ce2a1ca]
[fv-az1718-879:09262] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcb0ce2a28b]
[fv-az1718-879:09262] [11] plumed(+0x15365)[0x560ca3222365]
[fv-az1718-879:09262] *** End of error message ***
</pre>
{% endraw %}
