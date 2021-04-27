**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_REWE.dat   
(download [zipped raw stdout](plumed_REWE.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az99-305:31680] *** Process received signal ***
[fv-az99-305:31680] Signal: Aborted (6)
[fv-az99-305:31680] Signal code:  (-6)
[fv-az99-305:31680] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f8f7a5e8210]
[fv-az99-305:31680] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f8f7a5e818b]
[fv-az99-305:31680] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f8f7a5c7859]
[fv-az99-305:31680] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f8f7a84f951]
[fv-az99-305:31680] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f8f7a85b47c]
[fv-az99-305:31680] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f8f7a85b4e7]
[fv-az99-305:31680] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f8f7a85b7ed]
[fv-az99-305:31680] [ 7] plumed_master(+0xf568)[0x56050d9cf568]
[fv-az99-305:31680] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f8f7a5c90b3]
[fv-az99-305:31680] [ 9] plumed_master(+0xf79e)[0x56050d9cf79e]
[fv-az99-305:31680] *** End of error message ***
</pre>
{% endraw %}
