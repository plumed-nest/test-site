**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w42-s10.164/plumed.dat   
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
[fv-az99-305:09425] *** Process received signal ***
[fv-az99-305:09425] Signal: Aborted (6)
[fv-az99-305:09425] Signal code:  (-6)
[fv-az99-305:09425] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f616324f210]
[fv-az99-305:09425] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f616324f18b]
[fv-az99-305:09425] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f616322e859]
[fv-az99-305:09425] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f61634b6951]
[fv-az99-305:09425] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f61634c247c]
[fv-az99-305:09425] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f61634c24e7]
[fv-az99-305:09425] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f61634c2799]
[fv-az99-305:09425] [ 7] plumed(+0xf47d)[0x55f22690e47d]
[fv-az99-305:09425] [ 8] plumed(+0x14004)[0x55f226913004]
[fv-az99-305:09425] [ 9] plumed(+0xf698)[0x55f22690e698]
[fv-az99-305:09425] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f61632300b3]
[fv-az99-305:09425] [11] plumed(+0xf76e)[0x55f22690e76e]
[fv-az99-305:09425] *** End of error message ***
</pre>
{% endraw %}
