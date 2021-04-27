**Project ID:** [plumID:19.060]({{ '/' | absolute_url }}eggs/19/060/)  
Stderr for source:  4_silicon/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: REFCV SPECIES=1-216 SIGMA=0.04 LATTICE_CONSTANTS=0.5431 CRYSTAL_STRUCTURE=DIAMOND LABEL=refcv MORE_THAN=RATIONAL R_0=0.5 NN=12 MM=24 MEAN
Maybe a missing space or a typo?
[fv-az99-305:36108] *** Process received signal ***
[fv-az99-305:36108] Signal: Aborted (6)
[fv-az99-305:36108] Signal code:  (-6)
[fv-az99-305:36108] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ff13d0d7210]
[fv-az99-305:36108] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ff13d0d718b]
[fv-az99-305:36108] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ff13d0b6859]
[fv-az99-305:36108] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ff13d33e951]
[fv-az99-305:36108] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ff13d34a47c]
[fv-az99-305:36108] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ff13d34a4e7]
[fv-az99-305:36108] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ff13d34a799]
[fv-az99-305:36108] [ 7] plumed(+0xf47d)[0x555a9882c47d]
[fv-az99-305:36108] [ 8] plumed(+0x14004)[0x555a98831004]
[fv-az99-305:36108] [ 9] plumed(+0xf698)[0x555a9882c698]
[fv-az99-305:36108] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ff13d0b80b3]
[fv-az99-305:36108] [11] plumed(+0xf76e)[0x555a9882c76e]
[fv-az99-305:36108] *** End of error message ***
</pre>
{% endraw %}
