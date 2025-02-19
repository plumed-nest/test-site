**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  01_AIMD_of_intermediates/INT3_2-Oxiranimine_and_Amoniac/FORCE_ESTIMATION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:07153] *** Process received signal ***
[fv-az1947-39:07153] Signal: Aborted (6)
[fv-az1947-39:07153] Signal code:  (-6)
[fv-az1947-39:07153] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7c3ec45330]
[fv-az1947-39:07153] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7c3ec9eb2c]
[fv-az1947-39:07153] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7c3ec4527e]
[fv-az1947-39:07153] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7c3ec288ff]
[fv-az1947-39:07153] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7c3f0a5ff5]
[fv-az1947-39:07153] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7c3f0bb0da]
[fv-az1947-39:07153] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7c3f0a5a55]
[fv-az1947-39:07153] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7c3f0a5a6f]
[fv-az1947-39:07153] [ 8] plumed(+0x146dd)[0x5576ce3536dd]
[fv-az1947-39:07153] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7c3ec2a1ca]
[fv-az1947-39:07153] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7c3ec2a28b]
[fv-az1947-39:07153] [11] plumed(+0x15365)[0x5576ce354365]
[fv-az1947-39:07153] *** End of error message ***
</pre>
{% endraw %}
