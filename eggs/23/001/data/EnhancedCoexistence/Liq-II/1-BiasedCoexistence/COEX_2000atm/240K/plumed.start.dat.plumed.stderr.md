**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.start.dat   
Download: [zipped raw stdout](plumed.start.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.start.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az532-512:06553] *** Process received signal ***
[fv-az532-512:06553] Signal: Aborted (6)
[fv-az532-512:06553] Signal code:  (-6)
[fv-az532-512:06553] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3b1ca42520]
[fv-az532-512:06553] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3b1ca969fc]
[fv-az532-512:06553] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3b1ca42476]
[fv-az532-512:06553] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3b1ca287f3]
[fv-az532-512:06553] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f3b1cea4f26]
[fv-az532-512:06553] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f3b1ceb6d9c]
[fv-az532-512:06553] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f3b1ceb6e07]
[fv-az532-512:06553] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3b1ceb70bb]
[fv-az532-512:06553] [ 8] plumed(+0x12f48)[0x557d71041f48]
[fv-az532-512:06553] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3b1ca29d90]
[fv-az532-512:06553] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3b1ca29e40]
[fv-az532-512:06553] [11] plumed(+0x131e5)[0x557d710421e5]
[fv-az532-512:06553] *** End of error message ***
</pre>
{% endraw %}
