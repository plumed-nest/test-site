**Project ID:** [plumID:21.034]({{ '/' | absolute_url }}eggs/21/034/)  
Stderr for source:  RiD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "DEEPFE" is not known.
[fv-az1718-879:08054] *** Process received signal ***
[fv-az1718-879:08054] Signal: Aborted (6)
[fv-az1718-879:08054] Signal code:  (-6)
[fv-az1718-879:08054] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9263c45330]
[fv-az1718-879:08054] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9263c9eb2c]
[fv-az1718-879:08054] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9263c4527e]
[fv-az1718-879:08054] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9263c288ff]
[fv-az1718-879:08054] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f92640a5ff5]
[fv-az1718-879:08054] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f92640bb0da]
[fv-az1718-879:08054] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f92640a5a55]
[fv-az1718-879:08054] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f92640a5a6f]
[fv-az1718-879:08054] [ 8] plumed(+0x146dd)[0x5577b92906dd]
[fv-az1718-879:08054] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9263c2a1ca]
[fv-az1718-879:08054] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9263c2a28b]
[fv-az1718-879:08054] [11] plumed(+0x15365)[0x5577b9291365]
[fv-az1718-879:08054] *** End of error message ***
</pre>
{% endraw %}
