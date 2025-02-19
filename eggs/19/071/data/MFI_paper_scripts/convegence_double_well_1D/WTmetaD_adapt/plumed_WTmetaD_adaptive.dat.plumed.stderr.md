**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
Download: [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_WTmetaD_adaptive.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1947-39:13738] *** Process received signal ***
[fv-az1947-39:13738] Signal: Aborted (6)
[fv-az1947-39:13738] Signal code:  (-6)
[fv-az1947-39:13738] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f65fe645330]
[fv-az1947-39:13738] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f65fe69eb2c]
[fv-az1947-39:13738] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f65fe64527e]
[fv-az1947-39:13738] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f65fe6288ff]
[fv-az1947-39:13738] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f65feaa5ff5]
[fv-az1947-39:13738] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f65feabb0da]
[fv-az1947-39:13738] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f65feaa5a55]
[fv-az1947-39:13738] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f65feaa5a6f]
[fv-az1947-39:13738] [ 8] plumed(+0x146dd)[0x55fe74b7f6dd]
[fv-az1947-39:13738] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f65fe62a1ca]
[fv-az1947-39:13738] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f65fe62a28b]
[fv-az1947-39:13738] [11] plumed(+0x15365)[0x55fe74b80365]
[fv-az1947-39:13738] *** End of error message ***
</pre>
{% endraw %}
