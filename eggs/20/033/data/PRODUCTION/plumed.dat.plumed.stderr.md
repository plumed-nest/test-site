**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[fv-az1106-239:43665] *** Process received signal ***
[fv-az1106-239:43665] Signal: Aborted (6)
[fv-az1106-239:43665] Signal code:  (-6)
[fv-az1106-239:43665] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8bb3c42520]
[fv-az1106-239:43665] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8bb3c969fc]
[fv-az1106-239:43665] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8bb3c42476]
[fv-az1106-239:43665] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8bb3c287f3]
[fv-az1106-239:43665] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8bb40a2b9e]
[fv-az1106-239:43665] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8bb40ae20c]
[fv-az1106-239:43665] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8bb40ae277]
[fv-az1106-239:43665] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8bb40ae52b]
[fv-az1106-239:43665] [ 8] plumed(+0x12f48)[0x562efa3b2f48]
[fv-az1106-239:43665] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8bb3c29d90]
[fv-az1106-239:43665] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8bb3c29e40]
[fv-az1106-239:43665] [11] plumed(+0x131e5)[0x562efa3b31e5]
[fv-az1106-239:43665] *** End of error message ***
</pre>
{% endraw %}
