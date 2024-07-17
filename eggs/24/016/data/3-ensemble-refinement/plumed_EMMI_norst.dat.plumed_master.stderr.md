**Project ID:** [plumID:24.016]({{ '/' | absolute_url }}eggs/24/016/)  
Stderr for source:  3-ensemble-refinement/plumed_EMMI_norst.dat   
Download: [zipped raw stdout](plumed_EMMI_norst.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI_norst.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action EMMIVOX with label emmi : Cannot find status file EMMIStatus

[fv-az774-16:69450] *** Process received signal ***
[fv-az774-16:69450] Signal: Aborted (6)
[fv-az774-16:69450] Signal code:  (-6)
[fv-az774-16:69450] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f114ba42520]
[fv-az774-16:69450] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f114ba969fc]
[fv-az774-16:69450] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f114ba42476]
[fv-az774-16:69450] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f114ba287f3]
[fv-az774-16:69450] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f114bea2b9e]
[fv-az774-16:69450] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f114beae20c]
[fv-az774-16:69450] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f114beae277]
[fv-az774-16:69450] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f114beae52b]
[fv-az774-16:69450] [ 8] plumed_master(+0x14274)[0x55b3f6bda274]
[fv-az774-16:69450] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f114ba29d90]
[fv-az774-16:69450] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f114ba29e40]
[fv-az774-16:69450] [11] plumed_master(+0x14ed5)[0x55b3f6bdaed5]
[fv-az774-16:69450] *** End of error message ***
</pre>
{% endraw %}
