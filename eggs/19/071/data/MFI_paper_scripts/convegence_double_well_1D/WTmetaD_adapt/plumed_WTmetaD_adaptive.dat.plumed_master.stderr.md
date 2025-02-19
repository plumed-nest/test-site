**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1947-39:13754] *** Process received signal ***
[fv-az1947-39:13754] Signal: Aborted (6)
[fv-az1947-39:13754] Signal code:  (-6)
[fv-az1947-39:13754] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f63a4245330]
[fv-az1947-39:13754] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f63a429eb2c]
[fv-az1947-39:13754] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f63a424527e]
[fv-az1947-39:13754] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f63a42288ff]
[fv-az1947-39:13754] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f63a46a5ff5]
[fv-az1947-39:13754] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f63a46bb0da]
[fv-az1947-39:13754] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f63a46a5a55]
[fv-az1947-39:13754] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f63a46a5a6f]
[fv-az1947-39:13754] [ 8] plumed_master(+0x146dd)[0x55be2940f6dd]
[fv-az1947-39:13754] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f63a422a1ca]
[fv-az1947-39:13754] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f63a422a28b]
[fv-az1947-39:13754] [11] plumed_master(+0x15365)[0x55be29410365]
[fv-az1947-39:13754] *** End of error message ***
</pre>
{% endraw %}
