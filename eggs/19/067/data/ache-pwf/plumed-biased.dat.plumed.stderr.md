**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pwf/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1106-239:44464] *** Process received signal ***
[fv-az1106-239:44464] Signal: Aborted (6)
[fv-az1106-239:44464] Signal code:  (-6)
[fv-az1106-239:44464] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2086a42520]
[fv-az1106-239:44464] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2086a969fc]
[fv-az1106-239:44464] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2086a42476]
[fv-az1106-239:44464] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2086a287f3]
[fv-az1106-239:44464] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2086ea2b9e]
[fv-az1106-239:44464] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2086eae20c]
[fv-az1106-239:44464] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2086eae277]
[fv-az1106-239:44464] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2086eae52b]
[fv-az1106-239:44464] [ 8] plumed(+0x12f48)[0x557693819f48]
[fv-az1106-239:44464] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2086a29d90]
[fv-az1106-239:44464] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2086a29e40]
[fv-az1106-239:44464] [11] plumed(+0x131e5)[0x55769381a1e5]
[fv-az1106-239:44464] *** End of error message ***
</pre>
{% endraw %}
