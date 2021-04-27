**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w35-s8.652/plumed.dat   
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
[fv-az99-305:09229] *** Process received signal ***
[fv-az99-305:09229] Signal: Aborted (6)
[fv-az99-305:09229] Signal code:  (-6)
[fv-az99-305:09229] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f2f4940c210]
[fv-az99-305:09229] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f2f4940c18b]
[fv-az99-305:09229] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f2f493eb859]
[fv-az99-305:09229] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2f49673951]
[fv-az99-305:09229] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f2f4967f47c]
[fv-az99-305:09229] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f2f4967f4e7]
[fv-az99-305:09229] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2f4967f799]
[fv-az99-305:09229] [ 7] plumed(+0xf47d)[0x561e16df647d]
[fv-az99-305:09229] [ 8] plumed(+0x14004)[0x561e16dfb004]
[fv-az99-305:09229] [ 9] plumed(+0xf698)[0x561e16df6698]
[fv-az99-305:09229] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f2f493ed0b3]
[fv-az99-305:09229] [11] plumed(+0xf76e)[0x561e16df676e]
[fv-az99-305:09229] *** End of error message ***
</pre>
{% endraw %}
