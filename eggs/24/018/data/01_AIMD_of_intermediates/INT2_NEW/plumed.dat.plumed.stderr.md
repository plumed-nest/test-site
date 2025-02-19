**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT2_NEW/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:06998] *** Process received signal ***
[fv-az1947-39:06998] Signal: Aborted (6)
[fv-az1947-39:06998] Signal code:  (-6)
[fv-az1947-39:06998] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0ab0845330]
[fv-az1947-39:06998] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0ab089eb2c]
[fv-az1947-39:06998] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0ab084527e]
[fv-az1947-39:06998] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0ab08288ff]
[fv-az1947-39:06998] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0ab0ca5ff5]
[fv-az1947-39:06998] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0ab0cbb0da]
[fv-az1947-39:06998] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0ab0ca5a55]
[fv-az1947-39:06998] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0ab0ca5a6f]
[fv-az1947-39:06998] [ 8] plumed(+0x146dd)[0x55d366e216dd]
[fv-az1947-39:06998] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0ab082a1ca]
[fv-az1947-39:06998] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0ab082a28b]
[fv-az1947-39:06998] [11] plumed(+0x15365)[0x55d366e22365]
[fv-az1947-39:06998] *** End of error message ***
</pre>
{% endraw %}
