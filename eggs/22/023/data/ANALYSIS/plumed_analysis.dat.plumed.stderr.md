**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  ANALYSIS/plumed_analysis.dat   
Download: [zipped raw stdout](plumed_analysis.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_analysis.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file structure.pdb
[fv-az695-903:05470] *** Process received signal ***
[fv-az695-903:05470] Signal: Aborted (6)
[fv-az695-903:05470] Signal code:  (-6)
[fv-az695-903:05470] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe4ac442520]
[fv-az695-903:05470] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe4ac4969fc]
[fv-az695-903:05470] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe4ac442476]
[fv-az695-903:05470] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe4ac4287f3]
[fv-az695-903:05470] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe4ac8a4f26]
[fv-az695-903:05470] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe4ac8b6d9c]
[fv-az695-903:05470] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe4ac8b6e07]
[fv-az695-903:05470] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe4ac8b70bb]
[fv-az695-903:05470] [ 8] plumed(+0x12f48)[0x55cc78a7ff48]
[fv-az695-903:05470] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe4ac429d90]
[fv-az695-903:05470] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe4ac429e40]
[fv-az695-903:05470] [11] plumed(+0x131e5)[0x55cc78a801e5]
[fv-az695-903:05470] *** End of error message ***
</pre>
{% endraw %}
