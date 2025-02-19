**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT1_Methanal_and_Cyanide_and_Amoniac/OLD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:06809] *** Process received signal ***
[fv-az1947-39:06809] Signal: Aborted (6)
[fv-az1947-39:06809] Signal code:  (-6)
[fv-az1947-39:06809] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4b15045330]
[fv-az1947-39:06809] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4b1509eb2c]
[fv-az1947-39:06809] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4b1504527e]
[fv-az1947-39:06809] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4b150288ff]
[fv-az1947-39:06809] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4b154a5ff5]
[fv-az1947-39:06809] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4b154bb0da]
[fv-az1947-39:06809] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4b154a5a55]
[fv-az1947-39:06809] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4b154a5a6f]
[fv-az1947-39:06809] [ 8] plumed_master(+0x146dd)[0x55dee32e46dd]
[fv-az1947-39:06809] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4b1502a1ca]
[fv-az1947-39:06809] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4b1502a28b]
[fv-az1947-39:06809] [11] plumed_master(+0x15365)[0x55dee32e5365]
[fv-az1947-39:06809] *** End of error message ***
</pre>
{% endraw %}
