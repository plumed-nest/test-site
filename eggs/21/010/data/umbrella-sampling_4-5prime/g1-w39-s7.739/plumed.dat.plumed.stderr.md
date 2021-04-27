**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_4-5prime/g1-w39-s7.739/plumed.dat   
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
[fv-az99-305:13569] *** Process received signal ***
[fv-az99-305:13569] Signal: Aborted (6)
[fv-az99-305:13569] Signal code:  (-6)
[fv-az99-305:13569] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd54994c210]
[fv-az99-305:13569] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd54994c18b]
[fv-az99-305:13569] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd54992b859]
[fv-az99-305:13569] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd549bb3951]
[fv-az99-305:13569] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd549bbf47c]
[fv-az99-305:13569] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd549bbf4e7]
[fv-az99-305:13569] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd549bbf799]
[fv-az99-305:13569] [ 7] plumed(+0xf47d)[0x55e71225d47d]
[fv-az99-305:13569] [ 8] plumed(+0x14004)[0x55e712262004]
[fv-az99-305:13569] [ 9] plumed(+0xf698)[0x55e71225d698]
[fv-az99-305:13569] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd54992d0b3]
[fv-az99-305:13569] [11] plumed(+0xf76e)[0x55e71225d76e]
[fv-az99-305:13569] *** End of error message ***
</pre>
{% endraw %}
