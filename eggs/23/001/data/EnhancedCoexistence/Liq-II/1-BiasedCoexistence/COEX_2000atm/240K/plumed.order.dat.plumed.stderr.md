**Project ID:** [plumID:23.001]({{ '/' | absolute_url }}eggs/23/001/)  
Stderr for source:  EnhancedCoexistence/Liq-II/1-BiasedCoexistence/COEX_2000atm/240K/plumed.order.dat   
Download: [zipped raw stdout](plumed.order.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.order.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label refcv : No environments have been found! Please specify a PDB file in the REFERENCE or in the REFERENCE_1, REFERENCE_2, etc keywords
[fv-az1113-981:41237] *** Process received signal ***
[fv-az1113-981:41237] Signal: Aborted (6)
[fv-az1113-981:41237] Signal code:  (-6)
[fv-az1113-981:41237] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f459dc42520]
[fv-az1113-981:41237] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f459dc969fc]
[fv-az1113-981:41237] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f459dc42476]
[fv-az1113-981:41237] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f459dc287f3]
[fv-az1113-981:41237] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f459e0a2b9e]
[fv-az1113-981:41237] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f459e0ae20c]
[fv-az1113-981:41237] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f459e0ae277]
[fv-az1113-981:41237] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f459e0ae52b]
[fv-az1113-981:41237] [ 8] plumed(+0x12f48)[0x561724a0df48]
[fv-az1113-981:41237] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f459dc29d90]
[fv-az1113-981:41237] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f459dc29e40]
[fv-az1113-981:41237] [11] plumed(+0x131e5)[0x561724a0e1e5]
[fv-az1113-981:41237] *** End of error message ***
</pre>
{% endraw %}
