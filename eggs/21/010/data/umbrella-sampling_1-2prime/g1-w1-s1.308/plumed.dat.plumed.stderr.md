**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w1-s1.308/plumed.dat   
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
[fv-az99-305:08541] *** Process received signal ***
[fv-az99-305:08541] Signal: Aborted (6)
[fv-az99-305:08541] Signal code:  (-6)
[fv-az99-305:08541] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f403aa50210]
[fv-az99-305:08541] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f403aa5018b]
[fv-az99-305:08541] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f403aa2f859]
[fv-az99-305:08541] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f403acb7951]
[fv-az99-305:08541] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f403acc347c]
[fv-az99-305:08541] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f403acc34e7]
[fv-az99-305:08541] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f403acc3799]
[fv-az99-305:08541] [ 7] plumed(+0xf47d)[0x55d24681147d]
[fv-az99-305:08541] [ 8] plumed(+0x14004)[0x55d246816004]
[fv-az99-305:08541] [ 9] plumed(+0xf698)[0x55d246811698]
[fv-az99-305:08541] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f403aa310b3]
[fv-az99-305:08541] [11] plumed(+0xf76e)[0x55d24681176e]
[fv-az99-305:08541] *** End of error message ***
</pre>
{% endraw %}
