**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w2-s3.139/plumed.dat   
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
[fv-az99-305:12119] *** Process received signal ***
[fv-az99-305:12119] Signal: Aborted (6)
[fv-az99-305:12119] Signal code:  (-6)
[fv-az99-305:12119] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f171fbf0210]
[fv-az99-305:12119] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f171fbf018b]
[fv-az99-305:12119] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f171fbcf859]
[fv-az99-305:12119] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f171fe57951]
[fv-az99-305:12119] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f171fe6347c]
[fv-az99-305:12119] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f171fe634e7]
[fv-az99-305:12119] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f171fe63799]
[fv-az99-305:12119] [ 7] plumed(+0xf47d)[0x560da592047d]
[fv-az99-305:12119] [ 8] plumed(+0x14004)[0x560da5925004]
[fv-az99-305:12119] [ 9] plumed(+0xf698)[0x560da5920698]
[fv-az99-305:12119] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f171fbd10b3]
[fv-az99-305:12119] [11] plumed(+0xf76e)[0x560da592076e]
[fv-az99-305:12119] *** End of error message ***
</pre>
{% endraw %}
