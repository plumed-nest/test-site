**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w1-s1.625/plumed.dat   
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
[fv-az99-305:14377] *** Process received signal ***
[fv-az99-305:14377] Signal: Aborted (6)
[fv-az99-305:14377] Signal code:  (-6)
[fv-az99-305:14377] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3e6b08d210]
[fv-az99-305:14377] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3e6b08d18b]
[fv-az99-305:14377] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3e6b06c859]
[fv-az99-305:14377] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3e6b2f4951]
[fv-az99-305:14377] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3e6b30047c]
[fv-az99-305:14377] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3e6b3004e7]
[fv-az99-305:14377] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3e6b300799]
[fv-az99-305:14377] [ 7] plumed(+0xf47d)[0x55b2fcbab47d]
[fv-az99-305:14377] [ 8] plumed(+0x14004)[0x55b2fcbb0004]
[fv-az99-305:14377] [ 9] plumed(+0xf698)[0x55b2fcbab698]
[fv-az99-305:14377] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3e6b06e0b3]
[fv-az99-305:14377] [11] plumed(+0xf76e)[0x55b2fcbab76e]
[fv-az99-305:14377] *** End of error message ***
</pre>
{% endraw %}
