**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w22-s8.332/plumed.dat   
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
[fv-az99-305:12191] *** Process received signal ***
[fv-az99-305:12191] Signal: Aborted (6)
[fv-az99-305:12191] Signal code:  (-6)
[fv-az99-305:12191] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fcc2f42f210]
[fv-az99-305:12191] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fcc2f42f18b]
[fv-az99-305:12191] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fcc2f40e859]
[fv-az99-305:12191] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fcc2f696951]
[fv-az99-305:12191] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fcc2f6a247c]
[fv-az99-305:12191] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fcc2f6a24e7]
[fv-az99-305:12191] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fcc2f6a2799]
[fv-az99-305:12191] [ 7] plumed(+0xf47d)[0x555db424947d]
[fv-az99-305:12191] [ 8] plumed(+0x14004)[0x555db424e004]
[fv-az99-305:12191] [ 9] plumed(+0xf698)[0x555db4249698]
[fv-az99-305:12191] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fcc2f4100b3]
[fv-az99-305:12191] [11] plumed(+0xf76e)[0x555db424976e]
[fv-az99-305:12191] *** End of error message ***
</pre>
{% endraw %}
