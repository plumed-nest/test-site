**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w47-s8.953/plumed.dat   
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
[fv-az99-305:13789] *** Process received signal ***
[fv-az99-305:13789] Signal: Aborted (6)
[fv-az99-305:13789] Signal code:  (-6)
[fv-az99-305:13789] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd6f1392210]
[fv-az99-305:13789] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd6f139218b]
[fv-az99-305:13789] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd6f1371859]
[fv-az99-305:13789] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd6f15f9951]
[fv-az99-305:13789] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd6f160547c]
[fv-az99-305:13789] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd6f16054e7]
[fv-az99-305:13789] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd6f1605799]
[fv-az99-305:13789] [ 7] plumed(+0xf47d)[0x55663820a47d]
[fv-az99-305:13789] [ 8] plumed(+0x14004)[0x55663820f004]
[fv-az99-305:13789] [ 9] plumed(+0xf698)[0x55663820a698]
[fv-az99-305:13789] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd6f13730b3]
[fv-az99-305:13789] [11] plumed(+0xf76e)[0x55663820a76e]
[fv-az99-305:13789] *** End of error message ***
</pre>
{% endraw %}
