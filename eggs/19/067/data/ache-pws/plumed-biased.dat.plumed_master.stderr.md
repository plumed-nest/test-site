**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pws/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1436-30:12919] *** Process received signal ***
[fv-az1436-30:12919] Signal: Aborted (6)
[fv-az1436-30:12919] Signal code:  (-6)
[fv-az1436-30:12919] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe9c3e45330]
[fv-az1436-30:12919] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe9c3e9eb2c]
[fv-az1436-30:12919] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe9c3e4527e]
[fv-az1436-30:12919] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe9c3e288ff]
[fv-az1436-30:12919] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe9c42a5ff5]
[fv-az1436-30:12919] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe9c42bb0da]
[fv-az1436-30:12919] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe9c42a5a55]
[fv-az1436-30:12919] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe9c42a5a6f]
[fv-az1436-30:12919] [ 8] plumed_master(+0x146dd)[0x55afd353a6dd]
[fv-az1436-30:12919] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe9c3e2a1ca]
[fv-az1436-30:12919] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe9c3e2a28b]
[fv-az1436-30:12919] [11] plumed_master(+0x15365)[0x55afd353b365]
[fv-az1436-30:12919] *** End of error message ***
</pre>
{% endraw %}
