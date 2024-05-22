**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/2_Entropy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[fv-az1435-553:40003] *** Process received signal ***
[fv-az1435-553:40003] Signal: Aborted (6)
[fv-az1435-553:40003] Signal code:  (-6)
[fv-az1435-553:40003] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6ccd842520]
[fv-az1435-553:40003] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6ccd8969fc]
[fv-az1435-553:40003] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6ccd842476]
[fv-az1435-553:40003] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6ccd8287f3]
[fv-az1435-553:40003] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6ccdca2b9e]
[fv-az1435-553:40003] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6ccdcae20c]
[fv-az1435-553:40003] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6ccdcae277]
[fv-az1435-553:40003] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6ccdcae52b]
[fv-az1435-553:40003] [ 8] plumed_master(+0x14274)[0x55c764f94274]
[fv-az1435-553:40003] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6ccd829d90]
[fv-az1435-553:40003] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6ccd829e40]
[fv-az1435-553:40003] [11] plumed_master(+0x14ed5)[0x55c764f94ed5]
[fv-az1435-553:40003] *** End of error message ***
</pre>
{% endraw %}
