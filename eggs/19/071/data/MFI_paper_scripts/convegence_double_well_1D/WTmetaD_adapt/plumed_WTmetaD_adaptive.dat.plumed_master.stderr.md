**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1493-330:08843] *** Process received signal ***
[fv-az1493-330:08843] Signal: Aborted (6)
[fv-az1493-330:08843] Signal code:  (-6)
[fv-az1493-330:08843] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f38e4642520]
[fv-az1493-330:08843] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f38e46969fc]
[fv-az1493-330:08843] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f38e4642476]
[fv-az1493-330:08843] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f38e46287f3]
[fv-az1493-330:08843] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f38e4aa4f26]
[fv-az1493-330:08843] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f38e4ab6d9c]
[fv-az1493-330:08843] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f38e4ab6e07]
[fv-az1493-330:08843] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f38e4ab70bb]
[fv-az1493-330:08843] [ 8] plumed_master(+0x12ebf)[0x56324f63bebf]
[fv-az1493-330:08843] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f38e4629d90]
[fv-az1493-330:08843] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f38e4629e40]
[fv-az1493-330:08843] [11] plumed_master(+0x13155)[0x56324f63c155]
[fv-az1493-330:08843] *** End of error message ***
</pre>
{% endraw %}
