**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g3-w1-s6.3125/plumed.dat   
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
[fv-az99-305:16389] *** Process received signal ***
[fv-az99-305:16389] Signal: Aborted (6)
[fv-az99-305:16389] Signal code:  (-6)
[fv-az99-305:16389] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f9957167210]
[fv-az99-305:16389] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f995716718b]
[fv-az99-305:16389] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f9957146859]
[fv-az99-305:16389] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f99573ce951]
[fv-az99-305:16389] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f99573da47c]
[fv-az99-305:16389] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f99573da4e7]
[fv-az99-305:16389] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f99573da799]
[fv-az99-305:16389] [ 7] plumed(+0xf47d)[0x560b4f17047d]
[fv-az99-305:16389] [ 8] plumed(+0x14004)[0x560b4f175004]
[fv-az99-305:16389] [ 9] plumed(+0xf698)[0x560b4f170698]
[fv-az99-305:16389] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f99571480b3]
[fv-az99-305:16389] [11] plumed(+0xf76e)[0x560b4f17076e]
[fv-az99-305:16389] *** End of error message ***
</pre>
{% endraw %}
