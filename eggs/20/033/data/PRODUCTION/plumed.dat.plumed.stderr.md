**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[fv-az1200-577:09088] *** Process received signal ***
[fv-az1200-577:09088] Signal: Aborted (6)
[fv-az1200-577:09088] Signal code:  (-6)
[fv-az1200-577:09088] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f24fc842520]
[fv-az1200-577:09088] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f24fc8969fc]
[fv-az1200-577:09088] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f24fc842476]
[fv-az1200-577:09088] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f24fc8287f3]
[fv-az1200-577:09088] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f24fcca4f26]
[fv-az1200-577:09088] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f24fccb6d9c]
[fv-az1200-577:09088] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f24fccb6e07]
[fv-az1200-577:09088] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f24fccb70bb]
[fv-az1200-577:09088] [ 8] plumed(+0x12f48)[0x55c9d461bf48]
[fv-az1200-577:09088] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f24fc829d90]
[fv-az1200-577:09088] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f24fc829e40]
[fv-az1200-577:09088] [11] plumed(+0x131e5)[0x55c9d461c1e5]
[fv-az1200-577:09088] *** End of error message ***
</pre>
{% endraw %}
