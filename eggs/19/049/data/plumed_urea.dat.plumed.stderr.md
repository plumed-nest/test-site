**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_urea.dat   
Download: [zipped raw stdout](plumed_urea.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_urea.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCES with label m1 : cannot understand the following words from the input line : LOCATION1=1, LOCATION2=9, COMPONENTS
[fv-az774-16:74015] *** Process received signal ***
[fv-az774-16:74015] Signal: Aborted (6)
[fv-az774-16:74015] Signal code:  (-6)
[fv-az774-16:74015] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7fd1642520]
[fv-az774-16:74015] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7fd16969fc]
[fv-az774-16:74015] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7fd1642476]
[fv-az774-16:74015] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7fd16287f3]
[fv-az774-16:74015] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7fd1aa2b9e]
[fv-az774-16:74015] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7fd1aae20c]
[fv-az774-16:74015] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7fd1aae277]
[fv-az774-16:74015] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7fd1aae52b]
[fv-az774-16:74015] [ 8] plumed(+0x12f48)[0x55a6f80caf48]
[fv-az774-16:74015] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7fd1629d90]
[fv-az774-16:74015] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7fd1629e40]
[fv-az774-16:74015] [11] plumed(+0x131e5)[0x55a6f80cb1e5]
[fv-az774-16:74015] *** End of error message ***
</pre>
{% endraw %}
