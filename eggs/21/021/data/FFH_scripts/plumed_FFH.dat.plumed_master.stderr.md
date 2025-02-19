**Project ID:** [plumID:21.021]({{ '/' | absolute_url }}eggs/21/021/)  
Stderr for source:  FFH_scripts/plumed_FFH.dat   
Download: [zipped raw stdout](plumed_FFH.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FFH.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "ATLAS" is not known.
[fv-az1718-879:08705] *** Process received signal ***
[fv-az1718-879:08705] Signal: Aborted (6)
[fv-az1718-879:08705] Signal code:  (-6)
[fv-az1718-879:08705] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb364245330]
[fv-az1718-879:08705] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb36429eb2c]
[fv-az1718-879:08705] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb36424527e]
[fv-az1718-879:08705] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb3642288ff]
[fv-az1718-879:08705] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb3646a5ff5]
[fv-az1718-879:08705] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb3646bb0da]
[fv-az1718-879:08705] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb3646a5a55]
[fv-az1718-879:08705] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb3646a5a6f]
[fv-az1718-879:08705] [ 8] plumed_master(+0x146dd)[0x5601933416dd]
[fv-az1718-879:08705] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb36422a1ca]
[fv-az1718-879:08705] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb36422a28b]
[fv-az1718-879:08705] [11] plumed_master(+0x15365)[0x560193342365]
[fv-az1718-879:08705] *** End of error message ***
</pre>
{% endraw %}
