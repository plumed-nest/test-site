**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HBOND_COORD SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb
Maybe a missing space or a typo?
[fv-az99-305:40279] *** Process received signal ***
[fv-az99-305:40279] Signal: Aborted (6)
[fv-az99-305:40279] Signal code:  (-6)
[fv-az99-305:40279] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fed8d37d210]
[fv-az99-305:40279] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fed8d37d18b]
[fv-az99-305:40279] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fed8d35c859]
[fv-az99-305:40279] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fed8d5e4951]
[fv-az99-305:40279] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fed8d5f047c]
[fv-az99-305:40279] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fed8d5f04e7]
[fv-az99-305:40279] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fed8d5f07ed]
[fv-az99-305:40279] [ 7] plumed_master(+0xf568)[0x55db8dd67568]
[fv-az99-305:40279] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fed8d35e0b3]
[fv-az99-305:40279] [ 9] plumed_master(+0xf79e)[0x55db8dd6779e]
[fv-az99-305:40279] *** End of error message ***
</pre>
{% endraw %}
