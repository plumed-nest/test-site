**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pws/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1106-239:44525] *** Process received signal ***
[fv-az1106-239:44525] Signal: Aborted (6)
[fv-az1106-239:44525] Signal code:  (-6)
[fv-az1106-239:44525] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3c10242520]
[fv-az1106-239:44525] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3c102969fc]
[fv-az1106-239:44525] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3c10242476]
[fv-az1106-239:44525] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3c102287f3]
[fv-az1106-239:44525] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3c106a2b9e]
[fv-az1106-239:44525] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3c106ae20c]
[fv-az1106-239:44525] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3c106ae277]
[fv-az1106-239:44525] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3c106ae52b]
[fv-az1106-239:44525] [ 8] plumed(+0x12f48)[0x5587a935cf48]
[fv-az1106-239:44525] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3c10229d90]
[fv-az1106-239:44525] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3c10229e40]
[fv-az1106-239:44525] [11] plumed(+0x131e5)[0x5587a935d1e5]
[fv-az1106-239:44525] *** End of error message ***
</pre>
{% endraw %}
