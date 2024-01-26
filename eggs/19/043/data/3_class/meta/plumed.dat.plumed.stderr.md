**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1542-52:08621] *** Process received signal ***
[fv-az1542-52:08621] Signal: Aborted (6)
[fv-az1542-52:08621] Signal code:  (-6)
[fv-az1542-52:08621] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f56df842520]
[fv-az1542-52:08621] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f56df8969fc]
[fv-az1542-52:08621] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f56df842476]
[fv-az1542-52:08621] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f56df8287f3]
[fv-az1542-52:08621] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f56dfca4f26]
[fv-az1542-52:08621] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f56dfcb6d9c]
[fv-az1542-52:08621] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f56dfcb6e07]
[fv-az1542-52:08621] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f56dfcb70bb]
[fv-az1542-52:08621] [ 8] plumed(+0x12f48)[0x5652f9c49f48]
[fv-az1542-52:08621] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f56df829d90]
[fv-az1542-52:08621] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f56df829e40]
[fv-az1542-52:08621] [11] plumed(+0x131e5)[0x5652f9c4a1e5]
[fv-az1542-52:08621] *** End of error message ***
</pre>
{% endraw %}
