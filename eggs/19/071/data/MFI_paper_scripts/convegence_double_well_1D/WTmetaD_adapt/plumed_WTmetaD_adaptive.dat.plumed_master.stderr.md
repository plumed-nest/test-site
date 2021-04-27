**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/convegence_double_well_1D/WTmetaD_adapt/plumed_WTmetaD_adaptive.dat   
(download [zipped raw stdout](plumed_WTmetaD_adaptive.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az99-305:31584] *** Process received signal ***
[fv-az99-305:31584] Signal: Aborted (6)
[fv-az99-305:31584] Signal code:  (-6)
[fv-az99-305:31584] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fb62cf0f210]
[fv-az99-305:31584] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fb62cf0f18b]
[fv-az99-305:31584] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fb62ceee859]
[fv-az99-305:31584] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fb62d176951]
[fv-az99-305:31584] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fb62d18247c]
[fv-az99-305:31584] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fb62d1824e7]
[fv-az99-305:31584] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fb62d1827ed]
[fv-az99-305:31584] [ 7] plumed_master(+0xf568)[0x5607872f9568]
[fv-az99-305:31584] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fb62cef00b3]
[fv-az99-305:31584] [ 9] plumed_master(+0xf79e)[0x5607872f979e]
[fv-az99-305:31584] *** End of error message ***
</pre>
{% endraw %}
