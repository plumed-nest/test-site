**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat   
Download: [zipped raw stdout](plumed.order.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az532-512:06530] *** Process received signal ***
[fv-az532-512:06530] Signal: Aborted (6)
[fv-az532-512:06530] Signal code:  (-6)
[fv-az532-512:06530] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f130b242520]
[fv-az532-512:06530] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f130b2969fc]
[fv-az532-512:06530] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f130b242476]
[fv-az532-512:06530] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f130b2287f3]
[fv-az532-512:06530] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f130b6a4f26]
[fv-az532-512:06530] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f130b6b6d9c]
[fv-az532-512:06530] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f130b6b6e07]
[fv-az532-512:06530] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f130b6b70bb]
[fv-az532-512:06530] [ 8] plumed_master(+0x12ebf)[0x55e14974cebf]
[fv-az532-512:06530] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f130b229d90]
[fv-az532-512:06530] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f130b229e40]
[fv-az532-512:06530] [11] plumed_master(+0x13155)[0x55e14974d155]
[fv-az532-512:06530] *** End of error message ***
</pre>
{% endraw %}
