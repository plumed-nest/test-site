**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az695-903:05479] *** Process received signal ***
[fv-az695-903:05479] Signal: Aborted (6)
[fv-az695-903:05479] Signal code:  (-6)
[fv-az695-903:05479] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2524842520]
[fv-az695-903:05479] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f25248969fc]
[fv-az695-903:05479] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2524842476]
[fv-az695-903:05479] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f25248287f3]
[fv-az695-903:05479] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f2524ca4f26]
[fv-az695-903:05479] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f2524cb6d9c]
[fv-az695-903:05479] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f2524cb6e07]
[fv-az695-903:05479] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2524cb70bb]
[fv-az695-903:05479] [ 8] plumed_master(+0x12ebf)[0x561d34122ebf]
[fv-az695-903:05479] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2524829d90]
[fv-az695-903:05479] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2524829e40]
[fv-az695-903:05479] [11] plumed_master(+0x13155)[0x561d34123155]
[fv-az695-903:05479] *** End of error message ***
</pre>
{% endraw %}
