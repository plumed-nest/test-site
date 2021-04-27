**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g7-w1-s7.9425/plumed.dat   
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
[fv-az99-305:12734] *** Process received signal ***
[fv-az99-305:12734] Signal: Aborted (6)
[fv-az99-305:12734] Signal code:  (-6)
[fv-az99-305:12734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7feb9b923210]
[fv-az99-305:12734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7feb9b92318b]
[fv-az99-305:12734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7feb9b902859]
[fv-az99-305:12734] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7feb9bb8a951]
[fv-az99-305:12734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7feb9bb9647c]
[fv-az99-305:12734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7feb9bb964e7]
[fv-az99-305:12734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7feb9bb96799]
[fv-az99-305:12734] [ 7] plumed(+0xf47d)[0x55610fd1847d]
[fv-az99-305:12734] [ 8] plumed(+0x14004)[0x55610fd1d004]
[fv-az99-305:12734] [ 9] plumed(+0xf698)[0x55610fd18698]
[fv-az99-305:12734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7feb9b9040b3]
[fv-az99-305:12734] [11] plumed(+0xf76e)[0x55610fd1876e]
[fv-az99-305:12734] *** End of error message ***
</pre>
{% endraw %}
