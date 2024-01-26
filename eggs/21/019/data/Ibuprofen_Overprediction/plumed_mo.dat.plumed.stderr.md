**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_mo.dat   
Download: [zipped raw stdout](plumed_mo.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_mo.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label @0 : Number of specified atoms should be 2
[fv-az532-512:09389] *** Process received signal ***
[fv-az532-512:09389] Signal: Aborted (6)
[fv-az532-512:09389] Signal code:  (-6)
[fv-az532-512:09389] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7e57242520]
[fv-az532-512:09389] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7e572969fc]
[fv-az532-512:09389] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7e57242476]
[fv-az532-512:09389] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7e572287f3]
[fv-az532-512:09389] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7e576a4f26]
[fv-az532-512:09389] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7e576b6d9c]
[fv-az532-512:09389] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7e576b6e07]
[fv-az532-512:09389] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7e576b70bb]
[fv-az532-512:09389] [ 8] plumed(+0x12f48)[0x55d67d7a2f48]
[fv-az532-512:09389] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7e57229d90]
[fv-az532-512:09389] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7e57229e40]
[fv-az532-512:09389] [11] plumed(+0x131e5)[0x55d67d7a31e5]
[fv-az532-512:09389] *** End of error message ***
</pre>
{% endraw %}
