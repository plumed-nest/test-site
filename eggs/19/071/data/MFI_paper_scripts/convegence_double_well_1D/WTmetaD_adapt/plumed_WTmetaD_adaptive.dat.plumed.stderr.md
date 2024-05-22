**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1435-553:43869] *** Process received signal ***
[fv-az1435-553:43869] Signal: Aborted (6)
[fv-az1435-553:43869] Signal code:  (-6)
[fv-az1435-553:43869] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbce7e42520]
[fv-az1435-553:43869] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbce7e969fc]
[fv-az1435-553:43869] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbce7e42476]
[fv-az1435-553:43869] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbce7e287f3]
[fv-az1435-553:43869] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbce82a2b9e]
[fv-az1435-553:43869] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbce82ae20c]
[fv-az1435-553:43869] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbce82ae277]
[fv-az1435-553:43869] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbce82ae52b]
[fv-az1435-553:43869] [ 8] plumed(+0x12f48)[0x55d00980df48]
[fv-az1435-553:43869] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbce7e29d90]
[fv-az1435-553:43869] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbce7e29e40]
[fv-az1435-553:43869] [11] plumed(+0x131e5)[0x55d00980e1e5]
[fv-az1435-553:43869] *** End of error message ***
</pre>
{% endraw %}
