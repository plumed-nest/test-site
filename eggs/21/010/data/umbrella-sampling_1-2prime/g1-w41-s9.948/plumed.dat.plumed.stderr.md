**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w41-s9.948/plumed.dat   
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
[fv-az99-305:09401] *** Process received signal ***
[fv-az99-305:09401] Signal: Aborted (6)
[fv-az99-305:09401] Signal code:  (-6)
[fv-az99-305:09401] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc693033210]
[fv-az99-305:09401] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc69303318b]
[fv-az99-305:09401] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc693012859]
[fv-az99-305:09401] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc69329a951]
[fv-az99-305:09401] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc6932a647c]
[fv-az99-305:09401] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc6932a64e7]
[fv-az99-305:09401] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc6932a6799]
[fv-az99-305:09401] [ 7] plumed(+0xf47d)[0x5640df55547d]
[fv-az99-305:09401] [ 8] plumed(+0x14004)[0x5640df55a004]
[fv-az99-305:09401] [ 9] plumed(+0xf698)[0x5640df555698]
[fv-az99-305:09401] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc6930140b3]
[fv-az99-305:09401] [11] plumed(+0xf76e)[0x5640df55576e]
[fv-az99-305:09401] *** End of error message ***
</pre>
{% endraw %}
