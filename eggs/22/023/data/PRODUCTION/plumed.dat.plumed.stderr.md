**Project ID:** [plumID:22.023]({{ '/' | absolute_url }}eggs/22/023/)  
Stderr for source:  PRODUCTION/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file ../structure.pdb
[fv-az695-903:05536] *** Process received signal ***
[fv-az695-903:05536] Signal: Aborted (6)
[fv-az695-903:05536] Signal code:  (-6)
[fv-az695-903:05536] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f44d4842520]
[fv-az695-903:05536] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f44d48969fc]
[fv-az695-903:05536] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f44d4842476]
[fv-az695-903:05536] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f44d48287f3]
[fv-az695-903:05536] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f44d4ca4f26]
[fv-az695-903:05536] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f44d4cb6d9c]
[fv-az695-903:05536] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f44d4cb6e07]
[fv-az695-903:05536] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f44d4cb70bb]
[fv-az695-903:05536] [ 8] plumed(+0x12f48)[0x5616b0392f48]
[fv-az695-903:05536] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f44d4829d90]
[fv-az695-903:05536] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f44d4829e40]
[fv-az695-903:05536] [11] plumed(+0x131e5)[0x5616b03931e5]
[fv-az695-903:05536] *** End of error message ***
</pre>
{% endraw %}
