**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-V/3-BiasedCoexistence/COEX_5000.0atm/245.0K/plumed.restart.dat   
Download: [zipped raw stdout](plumed.restart.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.restart.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(opes/OPESexpanded.cpp:434) PLMD::opes::OPESexpanded::OPESexpanded(const PLMD::ActionOptions&)
RESTART requested, but file 'DELTAFS' was not found!
Set RESTART=NO or provide a restart file
[fv-az532-512:06825] *** Process received signal ***
[fv-az532-512:06825] Signal: Aborted (6)
[fv-az532-512:06825] Signal code:  (-6)
[fv-az532-512:06825] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9f15242520]
[fv-az532-512:06825] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9f152969fc]
[fv-az532-512:06825] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9f15242476]
[fv-az532-512:06825] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9f152287f3]
[fv-az532-512:06825] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9f156a4f26]
[fv-az532-512:06825] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9f156b6d9c]
[fv-az532-512:06825] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9f156b6e07]
[fv-az532-512:06825] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9f156b70bb]
[fv-az532-512:06825] [ 8] plumed(+0x12f48)[0x556611d52f48]
[fv-az532-512:06825] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9f15229d90]
[fv-az532-512:06825] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9f15229e40]
[fv-az532-512:06825] [11] plumed(+0x131e5)[0x556611d531e5]
[fv-az532-512:06825] *** End of error message ***
</pre>
{% endraw %}
