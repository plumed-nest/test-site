**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w3-s2.125/plumed.dat   
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
[fv-az99-305:14915] *** Process received signal ***
[fv-az99-305:14915] Signal: Aborted (6)
[fv-az99-305:14915] Signal code:  (-6)
[fv-az99-305:14915] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdc1db18210]
[fv-az99-305:14915] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdc1db1818b]
[fv-az99-305:14915] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdc1daf7859]
[fv-az99-305:14915] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdc1dd7f951]
[fv-az99-305:14915] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdc1dd8b47c]
[fv-az99-305:14915] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdc1dd8b4e7]
[fv-az99-305:14915] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdc1dd8b799]
[fv-az99-305:14915] [ 7] plumed(+0xf47d)[0x559954a3b47d]
[fv-az99-305:14915] [ 8] plumed(+0x14004)[0x559954a40004]
[fv-az99-305:14915] [ 9] plumed(+0xf698)[0x559954a3b698]
[fv-az99-305:14915] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdc1daf90b3]
[fv-az99-305:14915] [11] plumed(+0xf76e)[0x559954a3b76e]
[fv-az99-305:14915] *** End of error message ***
</pre>
{% endraw %}
