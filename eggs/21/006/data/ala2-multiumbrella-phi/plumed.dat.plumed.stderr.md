**Project ID:** [plumID:21.006]({{ '/' | absolute_url }}eggs/21/006/)  
Stderr for source:  ala2-multiumbrella-phi/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_UMBRELLAS_LINE LABEL=ecv ARG=phi MIN_CV=-pi MAX_CV=pi SIGMA=0.15 BARRIER=50
Maybe a missing space or a typo?
[fv-az99-305:17587] *** Process received signal ***
[fv-az99-305:17587] Signal: Aborted (6)
[fv-az99-305:17587] Signal code:  (-6)
[fv-az99-305:17587] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f27eb1f3210]
[fv-az99-305:17587] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f27eb1f318b]
[fv-az99-305:17587] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f27eb1d2859]
[fv-az99-305:17587] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f27eb45a951]
[fv-az99-305:17587] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f27eb46647c]
[fv-az99-305:17587] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f27eb4664e7]
[fv-az99-305:17587] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f27eb466799]
[fv-az99-305:17587] [ 7] plumed(+0xf47d)[0x56418e75f47d]
[fv-az99-305:17587] [ 8] plumed(+0x14004)[0x56418e764004]
[fv-az99-305:17587] [ 9] plumed(+0xf698)[0x56418e75f698]
[fv-az99-305:17587] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f27eb1d40b3]
[fv-az99-305:17587] [11] plumed(+0xf76e)[0x56418e75f76e]
[fv-az99-305:17587] *** End of error message ***
</pre>
{% endraw %}
