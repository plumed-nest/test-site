**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1110-714:74102] *** Process received signal ***
[fv-az1110-714:74102] Signal: Aborted (6)
[fv-az1110-714:74102] Signal code:  (-6)
[fv-az1110-714:74102] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd488c42520]
[fv-az1110-714:74102] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd488c969fc]
[fv-az1110-714:74102] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd488c42476]
[fv-az1110-714:74102] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd488c287f3]
[fv-az1110-714:74102] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd4890a2b9e]
[fv-az1110-714:74102] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd4890ae20c]
[fv-az1110-714:74102] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd4890ae277]
[fv-az1110-714:74102] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd4890ae52b]
[fv-az1110-714:74102] [ 8] plumed_master(+0x14274)[0x561234f64274]
[fv-az1110-714:74102] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd488c29d90]
[fv-az1110-714:74102] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd488c29e40]
[fv-az1110-714:74102] [11] plumed_master(+0x14ed5)[0x561234f64ed5]
[fv-az1110-714:74102] *** End of error message ***
</pre>
{% endraw %}
