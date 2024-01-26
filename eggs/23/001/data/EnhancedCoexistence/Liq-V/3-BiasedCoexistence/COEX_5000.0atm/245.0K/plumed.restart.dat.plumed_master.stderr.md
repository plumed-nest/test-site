**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.restart.dat   
Download: [zipped raw stdout](plumed.restart.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.restart.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(opes/OPESexpanded.cpp:434) PLMD::opes::OPESexpanded::OPESexpanded(const PLMD::ActionOptions&)
RESTART requested, but file 'DELTAFS' was not found!
Set RESTART=NO or provide a restart file
[fv-az532-512:06833] *** Process received signal ***
[fv-az532-512:06833] Signal: Aborted (6)
[fv-az532-512:06833] Signal code:  (-6)
[fv-az532-512:06833] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f809bc42520]
[fv-az532-512:06833] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f809bc969fc]
[fv-az532-512:06833] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f809bc42476]
[fv-az532-512:06833] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f809bc287f3]
[fv-az532-512:06833] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f809c0a4f26]
[fv-az532-512:06833] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f809c0b6d9c]
[fv-az532-512:06833] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f809c0b6e07]
[fv-az532-512:06833] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f809c0b70bb]
[fv-az532-512:06833] [ 8] plumed_master(+0x12ebf)[0x55d8978beebf]
[fv-az532-512:06833] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f809bc29d90]
[fv-az532-512:06833] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f809bc29e40]
[fv-az532-512:06833] [11] plumed_master(+0x13155)[0x55d8978bf155]
[fv-az532-512:06833] *** End of error message ***
</pre>
{% endraw %}
