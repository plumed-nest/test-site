**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w14-s4.875/plumed.dat   
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
[fv-az99-305:14499] *** Process received signal ***
[fv-az99-305:14499] Signal: Aborted (6)
[fv-az99-305:14499] Signal code:  (-6)
[fv-az99-305:14499] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1407777210]
[fv-az99-305:14499] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f140777718b]
[fv-az99-305:14499] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1407756859]
[fv-az99-305:14499] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f14079de951]
[fv-az99-305:14499] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f14079ea47c]
[fv-az99-305:14499] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f14079ea4e7]
[fv-az99-305:14499] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f14079ea799]
[fv-az99-305:14499] [ 7] plumed(+0xf47d)[0x55b224f6347d]
[fv-az99-305:14499] [ 8] plumed(+0x14004)[0x55b224f68004]
[fv-az99-305:14499] [ 9] plumed(+0xf698)[0x55b224f63698]
[fv-az99-305:14499] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f14077580b3]
[fv-az99-305:14499] [11] plumed(+0xf76e)[0x55b224f6376e]
[fv-az99-305:14499] *** End of error message ***
</pre>
{% endraw %}
