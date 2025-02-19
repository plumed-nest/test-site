**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[fv-az1372-996:05883] *** Process received signal ***
[fv-az1372-996:05883] Signal: Aborted (6)
[fv-az1372-996:05883] Signal code:  (-6)
[fv-az1372-996:05883] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0183a45330]
[fv-az1372-996:05883] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0183a9eb2c]
[fv-az1372-996:05883] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0183a4527e]
[fv-az1372-996:05883] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0183a288ff]
[fv-az1372-996:05883] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0183ea5ff5]
[fv-az1372-996:05883] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0183ebb0da]
[fv-az1372-996:05883] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0183ea5a55]
[fv-az1372-996:05883] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0183ea5a6f]
[fv-az1372-996:05883] [ 8] plumed(+0x146dd)[0x5640760606dd]
[fv-az1372-996:05883] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0183a2a1ca]
[fv-az1372-996:05883] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0183a2a28b]
[fv-az1372-996:05883] [11] plumed(+0x15365)[0x564076061365]
[fv-az1372-996:05883] *** End of error message ***
</pre>
{% endraw %}
