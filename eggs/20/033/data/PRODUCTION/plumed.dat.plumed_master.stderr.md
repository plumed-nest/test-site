**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  PRODUCTION/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action WHOLEMOLECULES with label @5 : cannot understand the following words from the input line : REF0=16.995,21.964,24.520, REF1=26.253,18.440,24.5030, REF2=24.616,28.069,24.203
[fv-az99-305:19039] *** Process received signal ***
[fv-az99-305:19039] Signal: Aborted (6)
[fv-az99-305:19039] Signal code:  (-6)
[fv-az99-305:19039] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f10a136c210]
[fv-az99-305:19039] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f10a136c18b]
[fv-az99-305:19039] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f10a134b859]
[fv-az99-305:19039] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f10a15d3951]
[fv-az99-305:19039] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f10a15df47c]
[fv-az99-305:19039] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f10a15df4e7]
[fv-az99-305:19039] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f10a15df7ed]
[fv-az99-305:19039] [ 7] plumed_master(+0xf568)[0x562c798b0568]
[fv-az99-305:19039] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f10a134d0b3]
[fv-az99-305:19039] [ 9] plumed_master(+0xf79e)[0x562c798b079e]
[fv-az99-305:19039] *** End of error message ***
</pre>
{% endraw %}
