**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g5-w2-s6.250/plumed.dat   
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
[fv-az99-305:15478] *** Process received signal ***
[fv-az99-305:15478] Signal: Aborted (6)
[fv-az99-305:15478] Signal code:  (-6)
[fv-az99-305:15478] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa64f0a1210]
[fv-az99-305:15478] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa64f0a118b]
[fv-az99-305:15478] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa64f080859]
[fv-az99-305:15478] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa64f308951]
[fv-az99-305:15478] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa64f31447c]
[fv-az99-305:15478] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa64f3144e7]
[fv-az99-305:15478] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa64f314799]
[fv-az99-305:15478] [ 7] plumed(+0xf47d)[0x5637274bb47d]
[fv-az99-305:15478] [ 8] plumed(+0x14004)[0x5637274c0004]
[fv-az99-305:15478] [ 9] plumed(+0xf698)[0x5637274bb698]
[fv-az99-305:15478] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa64f0820b3]
[fv-az99-305:15478] [11] plumed(+0xf76e)[0x5637274bb76e]
[fv-az99-305:15478] *** End of error message ***
</pre>
{% endraw %}
