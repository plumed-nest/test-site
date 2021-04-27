**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/LJ-38/plumed_reweight.dat   
(download [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action MATHEVAL with label ns : action nsa has no component named nsa (hint! the components in this actions are: )
[fv-az99-305:27021] *** Process received signal ***
[fv-az99-305:27021] Signal: Aborted (6)
[fv-az99-305:27021] Signal code:  (-6)
[fv-az99-305:27021] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc9d88a8210]
[fv-az99-305:27021] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc9d88a818b]
[fv-az99-305:27021] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc9d8887859]
[fv-az99-305:27021] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc9d8b0f951]
[fv-az99-305:27021] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc9d8b1b47c]
[fv-az99-305:27021] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc9d8b1b4e7]
[fv-az99-305:27021] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fc9d8b1b7ed]
[fv-az99-305:27021] [ 7] plumed_master(+0xf568)[0x5647eae08568]
[fv-az99-305:27021] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc9d88890b3]
[fv-az99-305:27021] [ 9] plumed_master(+0xf79e)[0x5647eae0879e]
[fv-az99-305:27021] *** End of error message ***
</pre>
{% endraw %}
