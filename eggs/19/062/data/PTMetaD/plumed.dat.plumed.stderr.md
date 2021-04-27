**Project ID:** [plumID:19.062]({{ '/' | absolute_url }}eggs/19/062/)  
Stderr for source:  PTMetaD/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label cvbias : cannot understand the following words from the input line : REWEIGHTING_NGRID=5001, REWEIGHTING_NHILLS=10
[fv-az99-305:35931] *** Process received signal ***
[fv-az99-305:35931] Signal: Aborted (6)
[fv-az99-305:35931] Signal code:  (-6)
[fv-az99-305:35931] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdd4b0a6210]
[fv-az99-305:35931] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdd4b0a618b]
[fv-az99-305:35931] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdd4b085859]
[fv-az99-305:35931] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdd4b30d951]
[fv-az99-305:35931] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdd4b31947c]
[fv-az99-305:35931] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdd4b3194e7]
[fv-az99-305:35931] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdd4b319799]
[fv-az99-305:35931] [ 7] plumed(+0xf47d)[0x55f49488947d]
[fv-az99-305:35931] [ 8] plumed(+0x14004)[0x55f49488e004]
[fv-az99-305:35931] [ 9] plumed(+0xf698)[0x55f494889698]
[fv-az99-305:35931] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdd4b0870b3]
[fv-az99-305:35931] [11] plumed(+0xf76e)[0x55f49488976e]
[fv-az99-305:35931] *** End of error message ***
</pre>
{% endraw %}
