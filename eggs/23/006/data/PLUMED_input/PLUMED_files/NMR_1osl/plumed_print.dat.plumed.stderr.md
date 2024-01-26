**Project ID:** [plumID:23.006]({{ '/' | absolute_url }}eggs/23/006/)  
Stderr for source:  PLUMED_input/PLUMED_files/NMR_1osl/plumed_print.dat   
Download: [zipped raw stdout](plumed_print.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_print.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file 1osl_C52V_GMX_new_numbering.pdb
[fv-az1542-52:04665] *** Process received signal ***
[fv-az1542-52:04665] Signal: Aborted (6)
[fv-az1542-52:04665] Signal code:  (-6)
[fv-az1542-52:04665] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd194242520]
[fv-az1542-52:04665] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd1942969fc]
[fv-az1542-52:04665] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd194242476]
[fv-az1542-52:04665] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd1942287f3]
[fv-az1542-52:04665] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fd1946a4f26]
[fv-az1542-52:04665] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fd1946b6d9c]
[fv-az1542-52:04665] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fd1946b6e07]
[fv-az1542-52:04665] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd1946b70bb]
[fv-az1542-52:04665] [ 8] plumed(+0x12f48)[0x55fbf28b2f48]
[fv-az1542-52:04665] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd194229d90]
[fv-az1542-52:04665] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd194229e40]
[fv-az1542-52:04665] [11] plumed(+0x131e5)[0x55fbf28b31e5]
[fv-az1542-52:04665] *** End of error message ***
</pre>
{% endraw %}
