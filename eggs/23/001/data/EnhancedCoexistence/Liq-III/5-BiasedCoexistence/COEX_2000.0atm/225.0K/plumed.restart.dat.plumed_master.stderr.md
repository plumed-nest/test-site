**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-III/5-BiasedCoexistence/COEX_2000.0atm/225.0K/plumed.restart.dat   
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
[fv-az532-512:06681] *** Process received signal ***
[fv-az532-512:06681] Signal: Aborted (6)
[fv-az532-512:06681] Signal code:  (-6)
[fv-az532-512:06681] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe35b842520]
[fv-az532-512:06681] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe35b8969fc]
[fv-az532-512:06681] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe35b842476]
[fv-az532-512:06681] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe35b8287f3]
[fv-az532-512:06681] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe35bca4f26]
[fv-az532-512:06681] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe35bcb6d9c]
[fv-az532-512:06681] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe35bcb6e07]
[fv-az532-512:06681] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe35bcb70bb]
[fv-az532-512:06681] [ 8] plumed_master(+0x12ebf)[0x55de0840eebf]
[fv-az532-512:06681] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe35b829d90]
[fv-az532-512:06681] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe35b829e40]
[fv-az532-512:06681] [11] plumed_master(+0x13155)[0x55de0840f155]
[fv-az532-512:06681] *** End of error message ***
</pre>
{% endraw %}
