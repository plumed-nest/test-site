**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis_unbiased.dat   
Download: [zipped raw stdout](plumed_analysis_unbiased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis_unbiased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az695-903:05503] *** Process received signal ***
[fv-az695-903:05503] Signal: Aborted (6)
[fv-az695-903:05503] Signal code:  (-6)
[fv-az695-903:05503] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8d04442520]
[fv-az695-903:05503] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8d044969fc]
[fv-az695-903:05503] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8d04442476]
[fv-az695-903:05503] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8d044287f3]
[fv-az695-903:05503] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f8d048a4f26]
[fv-az695-903:05503] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f8d048b6d9c]
[fv-az695-903:05503] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f8d048b6e07]
[fv-az695-903:05503] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8d048b70bb]
[fv-az695-903:05503] [ 8] plumed(+0x12f48)[0x55dce85aaf48]
[fv-az695-903:05503] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8d04429d90]
[fv-az695-903:05503] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8d04429e40]
[fv-az695-903:05503] [11] plumed(+0x131e5)[0x55dce85ab1e5]
[fv-az695-903:05503] *** End of error message ***
</pre>
{% endraw %}
