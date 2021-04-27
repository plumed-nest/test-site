**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w11-s5.150/plumed.dat   
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
[fv-az99-305:15651] *** Process received signal ***
[fv-az99-305:15651] Signal: Aborted (6)
[fv-az99-305:15651] Signal code:  (-6)
[fv-az99-305:15651] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa1da965210]
[fv-az99-305:15651] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa1da96518b]
[fv-az99-305:15651] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa1da944859]
[fv-az99-305:15651] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa1dabcc951]
[fv-az99-305:15651] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa1dabd847c]
[fv-az99-305:15651] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa1dabd84e7]
[fv-az99-305:15651] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa1dabd8799]
[fv-az99-305:15651] [ 7] plumed(+0xf47d)[0x559aefde447d]
[fv-az99-305:15651] [ 8] plumed(+0x14004)[0x559aefde9004]
[fv-az99-305:15651] [ 9] plumed(+0xf698)[0x559aefde4698]
[fv-az99-305:15651] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa1da9460b3]
[fv-az99-305:15651] [11] plumed(+0xf76e)[0x559aefde476e]
[fv-az99-305:15651] *** End of error message ***
</pre>
{% endraw %}
