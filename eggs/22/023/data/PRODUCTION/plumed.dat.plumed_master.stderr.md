**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[fv-az695-903:05544] *** Process received signal ***
[fv-az695-903:05544] Signal: Aborted (6)
[fv-az695-903:05544] Signal code:  (-6)
[fv-az695-903:05544] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f349f042520]
[fv-az695-903:05544] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f349f0969fc]
[fv-az695-903:05544] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f349f042476]
[fv-az695-903:05544] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f349f0287f3]
[fv-az695-903:05544] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f349f4a4f26]
[fv-az695-903:05544] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f349f4b6d9c]
[fv-az695-903:05544] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f349f4b6e07]
[fv-az695-903:05544] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f349f4b70bb]
[fv-az695-903:05544] [ 8] plumed_master(+0x12ebf)[0x55d51d539ebf]
[fv-az695-903:05544] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f349f029d90]
[fv-az695-903:05544] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f349f029e40]
[fv-az695-903:05544] [11] plumed_master(+0x13155)[0x55d51d53a155]
[fv-az695-903:05544] *** End of error message ***
</pre>
{% endraw %}
