**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w10-s3.252/plumed.dat   
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
[fv-az99-305:08565] *** Process received signal ***
[fv-az99-305:08565] Signal: Aborted (6)
[fv-az99-305:08565] Signal code:  (-6)
[fv-az99-305:08565] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fad0b834210]
[fv-az99-305:08565] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fad0b83418b]
[fv-az99-305:08565] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fad0b813859]
[fv-az99-305:08565] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fad0ba9b951]
[fv-az99-305:08565] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fad0baa747c]
[fv-az99-305:08565] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fad0baa74e7]
[fv-az99-305:08565] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fad0baa7799]
[fv-az99-305:08565] [ 7] plumed(+0xf47d)[0x56074f11f47d]
[fv-az99-305:08565] [ 8] plumed(+0x14004)[0x56074f124004]
[fv-az99-305:08565] [ 9] plumed(+0xf698)[0x56074f11f698]
[fv-az99-305:08565] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fad0b8150b3]
[fv-az99-305:08565] [11] plumed(+0xf76e)[0x56074f11f76e]
[fv-az99-305:08565] *** End of error message ***
</pre>
{% endraw %}
