**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pwf/plumed-biased.dat   
(download [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az99-305:32063] *** Process received signal ***
[fv-az99-305:32063] Signal: Aborted (6)
[fv-az99-305:32063] Signal code:  (-6)
[fv-az99-305:32063] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9737477210]
[fv-az99-305:32063] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f973747718b]
[fv-az99-305:32063] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9737456859]
[fv-az99-305:32063] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f97376de951]
[fv-az99-305:32063] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f97376ea47c]
[fv-az99-305:32063] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f97376ea4e7]
[fv-az99-305:32063] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f97376ea7ed]
[fv-az99-305:32063] [ 7] plumed_master(+0xf568)[0x55e0215a6568]
[fv-az99-305:32063] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f97374580b3]
[fv-az99-305:32063] [ 9] plumed_master(+0xf79e)[0x55e0215a679e]
[fv-az99-305:32063] *** End of error message ***
</pre>
{% endraw %}
