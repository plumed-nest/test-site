**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g4-w1-s9.438/plumed.dat   
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
[fv-az99-305:15406] *** Process received signal ***
[fv-az99-305:15406] Signal: Aborted (6)
[fv-az99-305:15406] Signal code:  (-6)
[fv-az99-305:15406] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7ffb819cc210]
[fv-az99-305:15406] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7ffb819cc18b]
[fv-az99-305:15406] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7ffb819ab859]
[fv-az99-305:15406] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7ffb81c33951]
[fv-az99-305:15406] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7ffb81c3f47c]
[fv-az99-305:15406] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7ffb81c3f4e7]
[fv-az99-305:15406] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7ffb81c3f799]
[fv-az99-305:15406] [ 7] plumed(+0xf47d)[0x560b2abff47d]
[fv-az99-305:15406] [ 8] plumed(+0x14004)[0x560b2ac04004]
[fv-az99-305:15406] [ 9] plumed(+0xf698)[0x560b2abff698]
[fv-az99-305:15406] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7ffb819ad0b3]
[fv-az99-305:15406] [11] plumed(+0xf76e)[0x560b2abff76e]
[fv-az99-305:15406] *** End of error message ***
</pre>
{% endraw %}
