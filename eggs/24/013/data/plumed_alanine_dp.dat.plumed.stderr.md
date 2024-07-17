**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[fv-az975-63:69596] *** Process received signal ***
[fv-az975-63:69596] Signal: Aborted (6)
[fv-az975-63:69596] Signal code:  (-6)
[fv-az975-63:69596] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f05f8242520]
[fv-az975-63:69596] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f05f82969fc]
[fv-az975-63:69596] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f05f8242476]
[fv-az975-63:69596] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f05f82287f3]
[fv-az975-63:69596] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f05f86a2b9e]
[fv-az975-63:69596] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f05f86ae20c]
[fv-az975-63:69596] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f05f86ae277]
[fv-az975-63:69596] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f05f86ae52b]
[fv-az975-63:69596] [ 8] plumed(+0x12f48)[0x5571de80df48]
[fv-az975-63:69596] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f05f8229d90]
[fv-az975-63:69596] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f05f8229e40]
[fv-az975-63:69596] [11] plumed(+0x131e5)[0x5571de80e1e5]
[fv-az975-63:69596] *** End of error message ***
</pre>
{% endraw %}
