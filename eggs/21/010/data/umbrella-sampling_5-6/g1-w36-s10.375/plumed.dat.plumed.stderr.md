**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w36-s10.375/plumed.dat   
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
[fv-az99-305:15087] *** Process received signal ***
[fv-az99-305:15087] Signal: Aborted (6)
[fv-az99-305:15087] Signal code:  (-6)
[fv-az99-305:15087] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f41bbb25210]
[fv-az99-305:15087] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f41bbb2518b]
[fv-az99-305:15087] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f41bbb04859]
[fv-az99-305:15087] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f41bbd8c951]
[fv-az99-305:15087] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f41bbd9847c]
[fv-az99-305:15087] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f41bbd984e7]
[fv-az99-305:15087] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f41bbd98799]
[fv-az99-305:15087] [ 7] plumed(+0xf47d)[0x5585f529247d]
[fv-az99-305:15087] [ 8] plumed(+0x14004)[0x5585f5297004]
[fv-az99-305:15087] [ 9] plumed(+0xf698)[0x5585f5292698]
[fv-az99-305:15087] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f41bbb060b3]
[fv-az99-305:15087] [11] plumed(+0xf76e)[0x5585f529276e]
[fv-az99-305:15087] *** End of error message ***
</pre>
{% endraw %}
