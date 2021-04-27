**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w20-s7.813/plumed.dat   
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
[fv-az99-305:12143] *** Process received signal ***
[fv-az99-305:12143] Signal: Aborted (6)
[fv-az99-305:12143] Signal code:  (-6)
[fv-az99-305:12143] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7ad372d210]
[fv-az99-305:12143] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7ad372d18b]
[fv-az99-305:12143] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7ad370c859]
[fv-az99-305:12143] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7ad3994951]
[fv-az99-305:12143] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7ad39a047c]
[fv-az99-305:12143] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7ad39a04e7]
[fv-az99-305:12143] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7ad39a0799]
[fv-az99-305:12143] [ 7] plumed(+0xf47d)[0x557c64da347d]
[fv-az99-305:12143] [ 8] plumed(+0x14004)[0x557c64da8004]
[fv-az99-305:12143] [ 9] plumed(+0xf698)[0x557c64da3698]
[fv-az99-305:12143] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7ad370e0b3]
[fv-az99-305:12143] [11] plumed(+0xf76e)[0x557c64da376e]
[fv-az99-305:12143] *** End of error message ***
</pre>
{% endraw %}
