**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1493-330:08835] *** Process received signal ***
[fv-az1493-330:08835] Signal: Aborted (6)
[fv-az1493-330:08835] Signal code:  (-6)
[fv-az1493-330:08835] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffbf4642520]
[fv-az1493-330:08835] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffbf46969fc]
[fv-az1493-330:08835] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffbf4642476]
[fv-az1493-330:08835] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffbf46287f3]
[fv-az1493-330:08835] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ffbf4aa4f26]
[fv-az1493-330:08835] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ffbf4ab6d9c]
[fv-az1493-330:08835] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ffbf4ab6e07]
[fv-az1493-330:08835] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffbf4ab70bb]
[fv-az1493-330:08835] [ 8] plumed(+0x12f48)[0x557669045f48]
[fv-az1493-330:08835] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffbf4629d90]
[fv-az1493-330:08835] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffbf4629e40]
[fv-az1493-330:08835] [11] plumed(+0x131e5)[0x5576690461e5]
[fv-az1493-330:08835] *** End of error message ***
</pre>
{% endraw %}
