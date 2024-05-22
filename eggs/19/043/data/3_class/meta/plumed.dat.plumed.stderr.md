**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az659-568:43302] *** Process received signal ***
[fv-az659-568:43302] Signal: Aborted (6)
[fv-az659-568:43302] Signal code:  (-6)
[fv-az659-568:43302] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f64e7842520]
[fv-az659-568:43302] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f64e78969fc]
[fv-az659-568:43302] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f64e7842476]
[fv-az659-568:43302] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f64e78287f3]
[fv-az659-568:43302] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f64e7ca2b9e]
[fv-az659-568:43302] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f64e7cae20c]
[fv-az659-568:43302] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f64e7cae277]
[fv-az659-568:43302] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f64e7cae52b]
[fv-az659-568:43302] [ 8] plumed(+0x12f48)[0x556d886acf48]
[fv-az659-568:43302] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f64e7829d90]
[fv-az659-568:43302] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f64e7829e40]
[fv-az659-568:43302] [11] plumed(+0x131e5)[0x556d886ad1e5]
[fv-az659-568:43302] *** End of error message ***
</pre>
{% endraw %}
