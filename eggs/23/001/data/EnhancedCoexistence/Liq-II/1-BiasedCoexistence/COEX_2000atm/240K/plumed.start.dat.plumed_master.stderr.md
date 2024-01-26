**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az532-512:06561] *** Process received signal ***
[fv-az532-512:06561] Signal: Aborted (6)
[fv-az532-512:06561] Signal code:  (-6)
[fv-az532-512:06561] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f122c842520]
[fv-az532-512:06561] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f122c8969fc]
[fv-az532-512:06561] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f122c842476]
[fv-az532-512:06561] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f122c8287f3]
[fv-az532-512:06561] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f122cca4f26]
[fv-az532-512:06561] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f122ccb6d9c]
[fv-az532-512:06561] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f122ccb6e07]
[fv-az532-512:06561] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f122ccb70bb]
[fv-az532-512:06561] [ 8] plumed_master(+0x12ebf)[0x561c711fcebf]
[fv-az532-512:06561] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f122c829d90]
[fv-az532-512:06561] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f122c829e40]
[fv-az532-512:06561] [11] plumed_master(+0x13155)[0x561c711fd155]
[fv-az532-512:06561] *** End of error message ***
</pre>
{% endraw %}
