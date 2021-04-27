**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w5-s2.583/plumed.dat   
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
[fv-az99-305:13862] *** Process received signal ***
[fv-az99-305:13862] Signal: Aborted (6)
[fv-az99-305:13862] Signal code:  (-6)
[fv-az99-305:13862] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1f98e70210]
[fv-az99-305:13862] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1f98e7018b]
[fv-az99-305:13862] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1f98e4f859]
[fv-az99-305:13862] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1f990d7951]
[fv-az99-305:13862] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1f990e347c]
[fv-az99-305:13862] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1f990e34e7]
[fv-az99-305:13862] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1f990e3799]
[fv-az99-305:13862] [ 7] plumed(+0xf47d)[0x55734fb1f47d]
[fv-az99-305:13862] [ 8] plumed(+0x14004)[0x55734fb24004]
[fv-az99-305:13862] [ 9] plumed(+0xf698)[0x55734fb1f698]
[fv-az99-305:13862] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1f98e510b3]
[fv-az99-305:13862] [11] plumed(+0xf76e)[0x55734fb1f76e]
[fv-az99-305:13862] *** End of error message ***
</pre>
{% endraw %}
