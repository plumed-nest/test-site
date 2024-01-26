**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[fv-az1200-577:09096] *** Process received signal ***
[fv-az1200-577:09096] Signal: Aborted (6)
[fv-az1200-577:09096] Signal code:  (-6)
[fv-az1200-577:09096] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7efe9ce42520]
[fv-az1200-577:09096] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7efe9ce969fc]
[fv-az1200-577:09096] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7efe9ce42476]
[fv-az1200-577:09096] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7efe9ce287f3]
[fv-az1200-577:09096] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7efe9d2a4f26]
[fv-az1200-577:09096] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7efe9d2b6d9c]
[fv-az1200-577:09096] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7efe9d2b6e07]
[fv-az1200-577:09096] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7efe9d2b70bb]
[fv-az1200-577:09096] [ 8] plumed_master(+0x12ebf)[0x562f39858ebf]
[fv-az1200-577:09096] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7efe9ce29d90]
[fv-az1200-577:09096] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7efe9ce29e40]
[fv-az1200-577:09096] [11] plumed_master(+0x13155)[0x562f39859155]
[fv-az1200-577:09096] *** End of error message ***
</pre>
{% endraw %}
