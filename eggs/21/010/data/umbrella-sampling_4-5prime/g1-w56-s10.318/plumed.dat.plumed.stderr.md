**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w56-s10.318/plumed.dat   
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
[fv-az99-305:14034] *** Process received signal ***
[fv-az99-305:14034] Signal: Aborted (6)
[fv-az99-305:14034] Signal code:  (-6)
[fv-az99-305:14034] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd4f41c4210]
[fv-az99-305:14034] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd4f41c418b]
[fv-az99-305:14034] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd4f41a3859]
[fv-az99-305:14034] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd4f442b951]
[fv-az99-305:14034] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd4f443747c]
[fv-az99-305:14034] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd4f44374e7]
[fv-az99-305:14034] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd4f4437799]
[fv-az99-305:14034] [ 7] plumed(+0xf47d)[0x55620e00947d]
[fv-az99-305:14034] [ 8] plumed(+0x14004)[0x55620e00e004]
[fv-az99-305:14034] [ 9] plumed(+0xf698)[0x55620e009698]
[fv-az99-305:14034] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd4f41a50b3]
[fv-az99-305:14034] [11] plumed(+0xf76e)[0x55620e00976e]
[fv-az99-305:14034] *** End of error message ***
</pre>
{% endraw %}
