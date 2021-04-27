**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w3-s11.617/plumed.dat   
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
[fv-az99-305:10407] *** Process received signal ***
[fv-az99-305:10407] Signal: Aborted (6)
[fv-az99-305:10407] Signal code:  (-6)
[fv-az99-305:10407] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4bb0dcb210]
[fv-az99-305:10407] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4bb0dcb18b]
[fv-az99-305:10407] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4bb0daa859]
[fv-az99-305:10407] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4bb1032951]
[fv-az99-305:10407] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4bb103e47c]
[fv-az99-305:10407] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4bb103e4e7]
[fv-az99-305:10407] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4bb103e799]
[fv-az99-305:10407] [ 7] plumed(+0xf47d)[0x558055a3447d]
[fv-az99-305:10407] [ 8] plumed(+0x14004)[0x558055a39004]
[fv-az99-305:10407] [ 9] plumed(+0xf698)[0x558055a34698]
[fv-az99-305:10407] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4bb0dac0b3]
[fv-az99-305:10407] [11] plumed(+0xf76e)[0x558055a3476e]
[fv-az99-305:10407] *** End of error message ***
</pre>
{% endraw %}
