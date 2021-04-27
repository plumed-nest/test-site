**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w17-s7.034/plumed.dat   
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
[fv-az99-305:12046] *** Process received signal ***
[fv-az99-305:12046] Signal: Aborted (6)
[fv-az99-305:12046] Signal code:  (-6)
[fv-az99-305:12046] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f02407ef210]
[fv-az99-305:12046] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f02407ef18b]
[fv-az99-305:12046] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f02407ce859]
[fv-az99-305:12046] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0240a56951]
[fv-az99-305:12046] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0240a6247c]
[fv-az99-305:12046] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0240a624e7]
[fv-az99-305:12046] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f0240a62799]
[fv-az99-305:12046] [ 7] plumed(+0xf47d)[0x564fd151b47d]
[fv-az99-305:12046] [ 8] plumed(+0x14004)[0x564fd1520004]
[fv-az99-305:12046] [ 9] plumed(+0xf698)[0x564fd151b698]
[fv-az99-305:12046] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f02407d00b3]
[fv-az99-305:12046] [11] plumed(+0xf76e)[0x564fd151b76e]
[fv-az99-305:12046] *** End of error message ***
</pre>
{% endraw %}
