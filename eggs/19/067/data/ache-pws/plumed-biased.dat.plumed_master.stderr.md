**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pws/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az774-16:74953] *** Process received signal ***
[fv-az774-16:74953] Signal: Aborted (6)
[fv-az774-16:74953] Signal code:  (-6)
[fv-az774-16:74953] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f50cb842520]
[fv-az774-16:74953] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f50cb8969fc]
[fv-az774-16:74953] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f50cb842476]
[fv-az774-16:74953] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f50cb8287f3]
[fv-az774-16:74953] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f50cbca2b9e]
[fv-az774-16:74953] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f50cbcae20c]
[fv-az774-16:74953] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f50cbcae277]
[fv-az774-16:74953] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f50cbcae52b]
[fv-az774-16:74953] [ 8] plumed_master(+0x14274)[0x556372c65274]
[fv-az774-16:74953] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f50cb829d90]
[fv-az774-16:74953] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f50cb829e40]
[fv-az774-16:74953] [11] plumed_master(+0x14ed5)[0x556372c65ed5]
[fv-az774-16:74953] *** End of error message ***
</pre>
{% endraw %}
