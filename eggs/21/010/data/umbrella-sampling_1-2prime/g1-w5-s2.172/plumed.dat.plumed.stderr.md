**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w5-s2.172/plumed.dat   
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
[fv-az99-305:09621] *** Process received signal ***
[fv-az99-305:09621] Signal: Aborted (6)
[fv-az99-305:09621] Signal code:  (-6)
[fv-az99-305:09621] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f30ac38a210]
[fv-az99-305:09621] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f30ac38a18b]
[fv-az99-305:09621] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f30ac369859]
[fv-az99-305:09621] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f30ac5f1951]
[fv-az99-305:09621] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f30ac5fd47c]
[fv-az99-305:09621] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f30ac5fd4e7]
[fv-az99-305:09621] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f30ac5fd799]
[fv-az99-305:09621] [ 7] plumed(+0xf47d)[0x55c22accf47d]
[fv-az99-305:09621] [ 8] plumed(+0x14004)[0x55c22acd4004]
[fv-az99-305:09621] [ 9] plumed(+0xf698)[0x55c22accf698]
[fv-az99-305:09621] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f30ac36b0b3]
[fv-az99-305:09621] [11] plumed(+0xf76e)[0x55c22accf76e]
[fv-az99-305:09621] *** End of error message ***
</pre>
{% endraw %}
