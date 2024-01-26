**Project ID:** [plumID:19.032]({{ '/' | absolute_url }}eggs/19/032/)  
Stderr for source:  plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file HILLS not found
[fv-az1148-6:10146] *** Process received signal ***
[fv-az1148-6:10146] Signal: Aborted (6)
[fv-az1148-6:10146] Signal code:  (-6)
[fv-az1148-6:10146] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3f41242520]
[fv-az1148-6:10146] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3f412969fc]
[fv-az1148-6:10146] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3f41242476]
[fv-az1148-6:10146] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3f412287f3]
[fv-az1148-6:10146] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f3f416a4f26]
[fv-az1148-6:10146] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f3f416b6d9c]
[fv-az1148-6:10146] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f3f416b6e07]
[fv-az1148-6:10146] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3f416b70bb]
[fv-az1148-6:10146] [ 8] plumed(+0x12f48)[0x562327d07f48]
[fv-az1148-6:10146] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3f41229d90]
[fv-az1148-6:10146] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3f41229e40]
[fv-az1148-6:10146] [11] plumed(+0x131e5)[0x562327d081e5]
[fv-az1148-6:10146] *** End of error message ***
</pre>
{% endraw %}
