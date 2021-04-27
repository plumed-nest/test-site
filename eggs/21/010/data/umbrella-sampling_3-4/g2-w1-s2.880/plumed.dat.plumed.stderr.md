**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w1-s2.880/plumed.dat   
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
[fv-az99-305:11849] *** Process received signal ***
[fv-az99-305:11849] Signal: Aborted (6)
[fv-az99-305:11849] Signal code:  (-6)
[fv-az99-305:11849] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd5c454e210]
[fv-az99-305:11849] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd5c454e18b]
[fv-az99-305:11849] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd5c452d859]
[fv-az99-305:11849] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd5c47b5951]
[fv-az99-305:11849] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd5c47c147c]
[fv-az99-305:11849] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd5c47c14e7]
[fv-az99-305:11849] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd5c47c1799]
[fv-az99-305:11849] [ 7] plumed(+0xf47d)[0x5611ad56747d]
[fv-az99-305:11849] [ 8] plumed(+0x14004)[0x5611ad56c004]
[fv-az99-305:11849] [ 9] plumed(+0xf698)[0x5611ad567698]
[fv-az99-305:11849] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd5c452f0b3]
[fv-az99-305:11849] [11] plumed(+0xf76e)[0x5611ad56776e]
[fv-az99-305:11849] *** End of error message ***
</pre>
{% endraw %}
