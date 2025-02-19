**Project ID:** [plumID:24.013]({{ '/' | absolute_url }}eggs/24/013/)  
Stderr for source:  plumed_alanine_dp.dat   
Download: [zipped raw stdout](plumed_alanine_dp.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_alanine_dp.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file reference.pdb
[fv-az1372-996:05899] *** Process received signal ***
[fv-az1372-996:05899] Signal: Aborted (6)
[fv-az1372-996:05899] Signal code:  (-6)
[fv-az1372-996:05899] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2004045330]
[fv-az1372-996:05899] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f200409eb2c]
[fv-az1372-996:05899] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f200404527e]
[fv-az1372-996:05899] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f20040288ff]
[fv-az1372-996:05899] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f20044a5ff5]
[fv-az1372-996:05899] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f20044bb0da]
[fv-az1372-996:05899] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f20044a5a55]
[fv-az1372-996:05899] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f20044a5a6f]
[fv-az1372-996:05899] [ 8] plumed_master(+0x146dd)[0x557e2f9436dd]
[fv-az1372-996:05899] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f200402a1ca]
[fv-az1372-996:05899] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f200402a28b]
[fv-az1372-996:05899] [11] plumed_master(+0x15365)[0x557e2f944365]
[fv-az1372-996:05899] *** End of error message ***
</pre>
{% endraw %}
