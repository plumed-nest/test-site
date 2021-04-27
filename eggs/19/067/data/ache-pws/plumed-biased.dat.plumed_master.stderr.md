**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pws/plumed-biased.dat   
(download [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az99-305:32109] *** Process received signal ***
[fv-az99-305:32109] Signal: Aborted (6)
[fv-az99-305:32109] Signal code:  (-6)
[fv-az99-305:32109] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb3e16ad210]
[fv-az99-305:32109] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb3e16ad18b]
[fv-az99-305:32109] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb3e168c859]
[fv-az99-305:32109] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb3e1914951]
[fv-az99-305:32109] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb3e192047c]
[fv-az99-305:32109] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb3e19204e7]
[fv-az99-305:32109] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fb3e19207ed]
[fv-az99-305:32109] [ 7] plumed_master(+0xf568)[0x563d989e9568]
[fv-az99-305:32109] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb3e168e0b3]
[fv-az99-305:32109] [ 9] plumed_master(+0xf79e)[0x563d989e979e]
[fv-az99-305:32109] *** End of error message ***
</pre>
{% endraw %}
