**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1435-553:39103] *** Process received signal ***
[fv-az1435-553:39103] Signal: Aborted (6)
[fv-az1435-553:39103] Signal code:  (-6)
[fv-az1435-553:39103] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5679a42520]
[fv-az1435-553:39103] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5679a969fc]
[fv-az1435-553:39103] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5679a42476]
[fv-az1435-553:39103] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5679a287f3]
[fv-az1435-553:39103] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5679ea2b9e]
[fv-az1435-553:39103] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5679eae20c]
[fv-az1435-553:39103] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5679eae277]
[fv-az1435-553:39103] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5679eae52b]
[fv-az1435-553:39103] [ 8] plumed_master(+0x14274)[0x559ca6979274]
[fv-az1435-553:39103] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5679a29d90]
[fv-az1435-553:39103] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5679a29e40]
[fv-az1435-553:39103] [11] plumed_master(+0x14ed5)[0x559ca6979ed5]
[fv-az1435-553:39103] *** End of error message ***
</pre>
{% endraw %}
