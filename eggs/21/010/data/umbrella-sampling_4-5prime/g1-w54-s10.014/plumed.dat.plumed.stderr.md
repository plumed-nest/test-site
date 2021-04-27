**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w54-s10.014/plumed.dat   
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
[fv-az99-305:13985] *** Process received signal ***
[fv-az99-305:13985] Signal: Aborted (6)
[fv-az99-305:13985] Signal code:  (-6)
[fv-az99-305:13985] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fea2c490210]
[fv-az99-305:13985] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fea2c49018b]
[fv-az99-305:13985] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fea2c46f859]
[fv-az99-305:13985] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fea2c6f7951]
[fv-az99-305:13985] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fea2c70347c]
[fv-az99-305:13985] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fea2c7034e7]
[fv-az99-305:13985] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fea2c703799]
[fv-az99-305:13985] [ 7] plumed(+0xf47d)[0x5577b935e47d]
[fv-az99-305:13985] [ 8] plumed(+0x14004)[0x5577b9363004]
[fv-az99-305:13985] [ 9] plumed(+0xf698)[0x5577b935e698]
[fv-az99-305:13985] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fea2c4710b3]
[fv-az99-305:13985] [11] plumed(+0xf76e)[0x5577b935e76e]
[fv-az99-305:13985] *** End of error message ***
</pre>
{% endraw %}
