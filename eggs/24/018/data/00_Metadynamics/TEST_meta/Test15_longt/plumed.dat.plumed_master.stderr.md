**Project ID:** [plumID:24.018]({{ '/' | absolute_url }}eggs/24/018/)  
Stderr for source:  00_Metadynamics/TEST_meta/Test15_longt/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "HILLS" is not known.
[fv-az1947-39:06550] *** Process received signal ***
[fv-az1947-39:06550] Signal: Aborted (6)
[fv-az1947-39:06550] Signal code:  (-6)
[fv-az1947-39:06550] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdf67645330]
[fv-az1947-39:06550] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdf6769eb2c]
[fv-az1947-39:06550] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdf6764527e]
[fv-az1947-39:06550] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdf676288ff]
[fv-az1947-39:06550] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdf67aa5ff5]
[fv-az1947-39:06550] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdf67abb0da]
[fv-az1947-39:06550] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdf67aa5a55]
[fv-az1947-39:06550] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdf67aa5a6f]
[fv-az1947-39:06550] [ 8] plumed_master(+0x146dd)[0x55934fe766dd]
[fv-az1947-39:06550] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdf6762a1ca]
[fv-az1947-39:06550] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdf6762a28b]
[fv-az1947-39:06550] [11] plumed_master(+0x15365)[0x55934fe77365]
[fv-az1947-39:06550] *** End of error message ***
</pre>
{% endraw %}
