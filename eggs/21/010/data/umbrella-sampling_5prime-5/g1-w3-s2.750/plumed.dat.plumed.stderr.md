**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w3-s2.750/plumed.dat   
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
[fv-az99-305:16143] *** Process received signal ***
[fv-az99-305:16143] Signal: Aborted (6)
[fv-az99-305:16143] Signal code:  (-6)
[fv-az99-305:16143] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0482b8e210]
[fv-az99-305:16143] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0482b8e18b]
[fv-az99-305:16143] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0482b6d859]
[fv-az99-305:16143] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0482df5951]
[fv-az99-305:16143] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0482e0147c]
[fv-az99-305:16143] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0482e014e7]
[fv-az99-305:16143] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f0482e01799]
[fv-az99-305:16143] [ 7] plumed(+0xf47d)[0x55ed7258247d]
[fv-az99-305:16143] [ 8] plumed(+0x14004)[0x55ed72587004]
[fv-az99-305:16143] [ 9] plumed(+0xf698)[0x55ed72582698]
[fv-az99-305:16143] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0482b6f0b3]
[fv-az99-305:16143] [11] plumed(+0xf76e)[0x55ed7258276e]
[fv-az99-305:16143] *** End of error message ***
</pre>
{% endraw %}
