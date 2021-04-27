**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w12-s5.736/plumed.dat   
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
[fv-az99-305:11923] *** Process received signal ***
[fv-az99-305:11923] Signal: Aborted (6)
[fv-az99-305:11923] Signal code:  (-6)
[fv-az99-305:11923] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1b086bd210]
[fv-az99-305:11923] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1b086bd18b]
[fv-az99-305:11923] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1b0869c859]
[fv-az99-305:11923] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1b08924951]
[fv-az99-305:11923] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1b0893047c]
[fv-az99-305:11923] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1b089304e7]
[fv-az99-305:11923] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1b08930799]
[fv-az99-305:11923] [ 7] plumed(+0xf47d)[0x55e1d28bf47d]
[fv-az99-305:11923] [ 8] plumed(+0x14004)[0x55e1d28c4004]
[fv-az99-305:11923] [ 9] plumed(+0xf698)[0x55e1d28bf698]
[fv-az99-305:11923] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1b0869e0b3]
[fv-az99-305:11923] [11] plumed(+0xf76e)[0x55e1d28bf76e]
[fv-az99-305:11923] *** End of error message ***
</pre>
{% endraw %}
