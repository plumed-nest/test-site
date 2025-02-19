**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "SPHERICAL_EXPANSION" is not known.
[fv-az1718-879:06272] *** Process received signal ***
[fv-az1718-879:06272] Signal: Aborted (6)
[fv-az1718-879:06272] Signal code:  (-6)
[fv-az1718-879:06272] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fde08645330]
[fv-az1718-879:06272] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fde0869eb2c]
[fv-az1718-879:06272] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fde0864527e]
[fv-az1718-879:06272] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fde086288ff]
[fv-az1718-879:06272] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fde08aa5ff5]
[fv-az1718-879:06272] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fde08abb0da]
[fv-az1718-879:06272] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fde08aa5a55]
[fv-az1718-879:06272] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fde08aa5a6f]
[fv-az1718-879:06272] [ 8] plumed_master(+0x146dd)[0x5645c4abf6dd]
[fv-az1718-879:06272] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fde0862a1ca]
[fv-az1718-879:06272] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fde0862a28b]
[fv-az1718-879:06272] [11] plumed_master(+0x15365)[0x5645c4ac0365]
[fv-az1718-879:06272] *** End of error message ***
</pre>
{% endraw %}
