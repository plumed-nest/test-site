**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  4_silicon/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: REFCV SPECIES=1-216 SIGMA=0.04 LATTICE_CONSTANTS=0.5431 CRYSTAL_STRUCTURE=DIAMOND LABEL=refcv MORE_THAN=RATIONAL R_0=0.5 NN=12 MM=24 MEAN
Maybe a missing space or a typo?
[fv-az99-305:36116] *** Process received signal ***
[fv-az99-305:36116] Signal: Aborted (6)
[fv-az99-305:36116] Signal code:  (-6)
[fv-az99-305:36116] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff385a97210]
[fv-az99-305:36116] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff385a9718b]
[fv-az99-305:36116] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff385a76859]
[fv-az99-305:36116] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff385cfe951]
[fv-az99-305:36116] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff385d0a47c]
[fv-az99-305:36116] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff385d0a4e7]
[fv-az99-305:36116] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7ff385d0a7ed]
[fv-az99-305:36116] [ 7] plumed_master(+0xf568)[0x55ae4d00c568]
[fv-az99-305:36116] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff385a780b3]
[fv-az99-305:36116] [ 9] plumed_master(+0xf79e)[0x55ae4d00c79e]
[fv-az99-305:36116] *** End of error message ***
</pre>
{% endraw %}
