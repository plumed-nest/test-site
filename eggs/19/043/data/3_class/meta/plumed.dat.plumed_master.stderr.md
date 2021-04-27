**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az99-305:38732] *** Process received signal ***
[fv-az99-305:38732] Signal: Aborted (6)
[fv-az99-305:38732] Signal code:  (-6)
[fv-az99-305:38732] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f32ca512210]
[fv-az99-305:38732] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f32ca51218b]
[fv-az99-305:38732] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f32ca4f1859]
[fv-az99-305:38732] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f32ca779951]
[fv-az99-305:38732] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f32ca78547c]
[fv-az99-305:38732] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f32ca7854e7]
[fv-az99-305:38732] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f32ca7857ed]
[fv-az99-305:38732] [ 7] plumed_master(+0xf568)[0x556445ce2568]
[fv-az99-305:38732] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f32ca4f30b3]
[fv-az99-305:38732] [ 9] plumed_master(+0xf79e)[0x556445ce279e]
[fv-az99-305:38732] *** End of error message ***
</pre>
{% endraw %}
