**Project ID:** [plumID:19.083]({{ '/' | absolute_url }}eggs/19/083/)  
Stderr for source:  Reaction_discovery/2.ICl/step1/B/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label restraint : restart file ..//HILLS.2 not found
[fv-az99-305:24898] *** Process received signal ***
[fv-az99-305:24898] Signal: Aborted (6)
[fv-az99-305:24898] Signal code:  (-6)
[fv-az99-305:24898] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f23efc6a210]
[fv-az99-305:24898] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f23efc6a18b]
[fv-az99-305:24898] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f23efc49859]
[fv-az99-305:24898] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f23efed1951]
[fv-az99-305:24898] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f23efedd47c]
[fv-az99-305:24898] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f23efedd4e7]
[fv-az99-305:24898] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f23efedd7ed]
[fv-az99-305:24898] [ 7] plumed_master(+0xf568)[0x55f3c1831568]
[fv-az99-305:24898] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f23efc4b0b3]
[fv-az99-305:24898] [ 9] plumed_master(+0xf79e)[0x55f3c183179e]
[fv-az99-305:24898] *** End of error message ***
</pre>
{% endraw %}
