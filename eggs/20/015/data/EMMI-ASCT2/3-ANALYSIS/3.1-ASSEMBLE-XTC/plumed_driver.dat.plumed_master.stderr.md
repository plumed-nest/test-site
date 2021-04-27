**Project ID:** [plumID:20.015]({{ '/' | absolute_url }}eggs/20/015/)  
Stderr for source:  EMMI-ASCT2/3-ANALYSIS/3.1-ASSEMBLE-XTC/plumed_driver.dat   
(download [zipped raw stdout](plumed_driver.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Action.cpp:243, function void PLMD::Action::error(const string&) const
+++ message follows +++
ERROR in input to action WHOLEMOLECULES with label @2 : cannot understand the following words from the input line : REF0=5.3607,4.5911,3.1497, REF1=3.2439,3.3684,6.0308
[fv-az99-305:23202] *** Process received signal ***
[fv-az99-305:23202] Signal: Aborted (6)
[fv-az99-305:23202] Signal code:  (-6)
[fv-az99-305:23202] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f384cca2210]
[fv-az99-305:23202] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f384cca218b]
[fv-az99-305:23202] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f384cc81859]
[fv-az99-305:23202] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f384cf09951]
[fv-az99-305:23202] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f384cf1547c]
[fv-az99-305:23202] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f384cf154e7]
[fv-az99-305:23202] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f384cf157ed]
[fv-az99-305:23202] [ 7] plumed_master(+0xf568)[0x557376f47568]
[fv-az99-305:23202] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f384cc830b3]
[fv-az99-305:23202] [ 9] plumed_master(+0xf79e)[0x557376f4779e]
[fv-az99-305:23202] *** End of error message ***
</pre>
{% endraw %}
