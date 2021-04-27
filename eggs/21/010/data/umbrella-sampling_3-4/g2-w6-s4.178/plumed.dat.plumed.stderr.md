**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w6-s4.178/plumed.dat   
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
[fv-az99-305:12388] *** Process received signal ***
[fv-az99-305:12388] Signal: Aborted (6)
[fv-az99-305:12388] Signal code:  (-6)
[fv-az99-305:12388] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f26219a0210]
[fv-az99-305:12388] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f26219a018b]
[fv-az99-305:12388] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f262197f859]
[fv-az99-305:12388] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2621c07951]
[fv-az99-305:12388] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2621c1347c]
[fv-az99-305:12388] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2621c134e7]
[fv-az99-305:12388] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2621c13799]
[fv-az99-305:12388] [ 7] plumed(+0xf47d)[0x558a60ffa47d]
[fv-az99-305:12388] [ 8] plumed(+0x14004)[0x558a60fff004]
[fv-az99-305:12388] [ 9] plumed(+0xf698)[0x558a60ffa698]
[fv-az99-305:12388] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f26219810b3]
[fv-az99-305:12388] [11] plumed(+0xf76e)[0x558a60ffa76e]
[fv-az99-305:12388] *** End of error message ***
</pre>
{% endraw %}
