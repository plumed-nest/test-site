**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pwf/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1436-30:12823] *** Process received signal ***
[fv-az1436-30:12823] Signal: Aborted (6)
[fv-az1436-30:12823] Signal code:  (-6)
[fv-az1436-30:12823] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa3d8645330]
[fv-az1436-30:12823] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa3d869eb2c]
[fv-az1436-30:12823] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa3d864527e]
[fv-az1436-30:12823] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa3d86288ff]
[fv-az1436-30:12823] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa3d8aa5ff5]
[fv-az1436-30:12823] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa3d8abb0da]
[fv-az1436-30:12823] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa3d8aa5a55]
[fv-az1436-30:12823] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa3d8aa5a6f]
[fv-az1436-30:12823] [ 8] plumed(+0x146dd)[0x562bf9bcf6dd]
[fv-az1436-30:12823] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa3d862a1ca]
[fv-az1436-30:12823] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa3d862a28b]
[fv-az1436-30:12823] [11] plumed(+0x15365)[0x562bf9bd0365]
[fv-az1436-30:12823] *** End of error message ***
</pre>
{% endraw %}
