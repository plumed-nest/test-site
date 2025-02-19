**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "SPHERICAL_EXPANSION" is not known.
[fv-az1718-879:06255] *** Process received signal ***
[fv-az1718-879:06255] Signal: Aborted (6)
[fv-az1718-879:06255] Signal code:  (-6)
[fv-az1718-879:06255] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efecc045330]
[fv-az1718-879:06255] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efecc09eb2c]
[fv-az1718-879:06255] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efecc04527e]
[fv-az1718-879:06255] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efecc0288ff]
[fv-az1718-879:06255] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efecc4a5ff5]
[fv-az1718-879:06255] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efecc4bb0da]
[fv-az1718-879:06255] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efecc4a5a55]
[fv-az1718-879:06255] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efecc4a5a6f]
[fv-az1718-879:06255] [ 8] plumed(+0x146dd)[0x562ed32d16dd]
[fv-az1718-879:06255] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efecc02a1ca]
[fv-az1718-879:06255] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efecc02a28b]
[fv-az1718-879:06255] [11] plumed(+0x15365)[0x562ed32d2365]
[fv-az1718-879:06255] *** End of error message ***
</pre>
{% endraw %}
