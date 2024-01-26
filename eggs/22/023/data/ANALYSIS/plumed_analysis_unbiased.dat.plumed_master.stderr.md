**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az695-903:05513] *** Process received signal ***
[fv-az695-903:05513] Signal: Aborted (6)
[fv-az695-903:05513] Signal code:  (-6)
[fv-az695-903:05513] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7feab6a42520]
[fv-az695-903:05513] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7feab6a969fc]
[fv-az695-903:05513] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7feab6a42476]
[fv-az695-903:05513] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7feab6a287f3]
[fv-az695-903:05513] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7feab6ea4f26]
[fv-az695-903:05513] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7feab6eb6d9c]
[fv-az695-903:05513] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7feab6eb6e07]
[fv-az695-903:05513] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7feab6eb70bb]
[fv-az695-903:05513] [ 8] plumed_master(+0x12ebf)[0x55a72068eebf]
[fv-az695-903:05513] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7feab6a29d90]
[fv-az695-903:05513] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7feab6a29e40]
[fv-az695-903:05513] [11] plumed_master(+0x13155)[0x55a72068f155]
[fv-az695-903:05513] *** End of error message ***
</pre>
{% endraw %}
