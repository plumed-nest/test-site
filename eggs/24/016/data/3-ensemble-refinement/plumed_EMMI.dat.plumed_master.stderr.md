**Project ID:** [plumID:24.016]({{ '/' | absolute_url }}eggs/24/016/)  
Stderr for source:  3-ensemble-refinement/plumed_EMMI.dat   
Download: [zipped raw stdout](plumed_EMMI.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action EMMIVOX with label emmi : Cannot find status file EMMIStatus

[fv-az774-16:69409] *** Process received signal ***
[fv-az774-16:69409] Signal: Aborted (6)
[fv-az774-16:69409] Signal code:  (-6)
[fv-az774-16:69409] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2ba9442520]
[fv-az774-16:69409] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2ba94969fc]
[fv-az774-16:69409] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2ba9442476]
[fv-az774-16:69409] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2ba94287f3]
[fv-az774-16:69409] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2ba98a2b9e]
[fv-az774-16:69409] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2ba98ae20c]
[fv-az774-16:69409] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2ba98ae277]
[fv-az774-16:69409] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2ba98ae52b]
[fv-az774-16:69409] [ 8] plumed_master(+0x14274)[0x5569ab6c0274]
[fv-az774-16:69409] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2ba9429d90]
[fv-az774-16:69409] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2ba9429e40]
[fv-az774-16:69409] [11] plumed_master(+0x14ed5)[0x5569ab6c0ed5]
[fv-az774-16:69409] *** End of error message ***
</pre>
{% endraw %}
