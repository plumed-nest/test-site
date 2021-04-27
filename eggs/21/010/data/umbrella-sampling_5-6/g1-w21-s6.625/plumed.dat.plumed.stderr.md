**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w21-s6.625/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:14696] *** Process received signal ***
[fv-az99-305:14696] Signal: Aborted (6)
[fv-az99-305:14696] Signal code:  (-6)
[fv-az99-305:14696] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f5e3b590210]
[fv-az99-305:14696] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5e3b59018b]
[fv-az99-305:14696] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5e3b56f859]
[fv-az99-305:14696] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f5e3b7f7951]
[fv-az99-305:14696] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f5e3b80347c]
[fv-az99-305:14696] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f5e3b8034e7]
[fv-az99-305:14696] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f5e3b803799]
[fv-az99-305:14696] [ 7] plumed(+0xf47d)[0x5622f1a7547d]
[fv-az99-305:14696] [ 8] plumed(+0x14004)[0x5622f1a7a004]
[fv-az99-305:14696] [ 9] plumed(+0xf698)[0x5622f1a75698]
[fv-az99-305:14696] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5e3b5710b3]
[fv-az99-305:14696] [11] plumed(+0xf76e)[0x5622f1a7576e]
[fv-az99-305:14696] *** End of error message ***
</pre>
{% endraw %}
