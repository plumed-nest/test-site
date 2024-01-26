**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-VI/4-BiasedCoexistence/COEX_7000.0atm/245.0K/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(opes/OPESexpanded.cpp:434) PLMD::opes::OPESexpanded::OPESexpanded(const PLMD::ActionOptions&)
RESTART requested, but file 'DELTAFS' was not found!
Set RESTART=NO or provide a restart file
[fv-az532-512:06893] *** Process received signal ***
[fv-az532-512:06893] Signal: Aborted (6)
[fv-az532-512:06893] Signal code:  (-6)
[fv-az532-512:06893] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa88b242520]
[fv-az532-512:06893] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa88b2969fc]
[fv-az532-512:06893] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa88b242476]
[fv-az532-512:06893] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa88b2287f3]
[fv-az532-512:06893] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa88b6a4f26]
[fv-az532-512:06893] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa88b6b6d9c]
[fv-az532-512:06893] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa88b6b6e07]
[fv-az532-512:06893] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa88b6b70bb]
[fv-az532-512:06893] [ 8] plumed_master(+0x12ebf)[0x562768e16ebf]
[fv-az532-512:06893] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa88b229d90]
[fv-az532-512:06893] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa88b229e40]
[fv-az532-512:06893] [11] plumed_master(+0x13155)[0x562768e17155]
[fv-az532-512:06893] *** End of error message ***
</pre>
{% endraw %}
