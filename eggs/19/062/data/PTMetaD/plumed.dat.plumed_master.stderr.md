**Project ID:** [plumID:19.062]({{ '/' | absolute_url }}eggs/19/062/)  
Stderr for source:  PTMetaD/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label cvbias : cannot understand the following words from the input line : REWEIGHTING_NGRID=5001, REWEIGHTING_NHILLS=10
[fv-az99-305:35939] *** Process received signal ***
[fv-az99-305:35939] Signal: Aborted (6)
[fv-az99-305:35939] Signal code:  (-6)
[fv-az99-305:35939] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9a09fdd210]
[fv-az99-305:35939] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f9a09fdd18b]
[fv-az99-305:35939] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9a09fbc859]
[fv-az99-305:35939] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f9a0a244951]
[fv-az99-305:35939] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f9a0a25047c]
[fv-az99-305:35939] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f9a0a2504e7]
[fv-az99-305:35939] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f9a0a2507ed]
[fv-az99-305:35939] [ 7] plumed_master(+0xf568)[0x557621f83568]
[fv-az99-305:35939] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f9a09fbe0b3]
[fv-az99-305:35939] [ 9] plumed_master(+0xf79e)[0x557621f8379e]
[fv-az99-305:35939] *** End of error message ***
</pre>
{% endraw %}
