**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w25-s7.625/plumed.dat   
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
[fv-az99-305:14794] *** Process received signal ***
[fv-az99-305:14794] Signal: Aborted (6)
[fv-az99-305:14794] Signal code:  (-6)
[fv-az99-305:14794] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f441600c210]
[fv-az99-305:14794] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f441600c18b]
[fv-az99-305:14794] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4415feb859]
[fv-az99-305:14794] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4416273951]
[fv-az99-305:14794] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f441627f47c]
[fv-az99-305:14794] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f441627f4e7]
[fv-az99-305:14794] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f441627f799]
[fv-az99-305:14794] [ 7] plumed(+0xf47d)[0x5602bd9eb47d]
[fv-az99-305:14794] [ 8] plumed(+0x14004)[0x5602bd9f0004]
[fv-az99-305:14794] [ 9] plumed(+0xf698)[0x5602bd9eb698]
[fv-az99-305:14794] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4415fed0b3]
[fv-az99-305:14794] [11] plumed(+0xf76e)[0x5602bd9eb76e]
[fv-az99-305:14794] *** End of error message ***
</pre>
{% endraw %}
