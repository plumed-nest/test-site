**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w12-s3.684/plumed.dat   
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
[fv-az99-305:08614] *** Process received signal ***
[fv-az99-305:08614] Signal: Aborted (6)
[fv-az99-305:08614] Signal code:  (-6)
[fv-az99-305:08614] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f140b40e210]
[fv-az99-305:08614] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f140b40e18b]
[fv-az99-305:08614] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f140b3ed859]
[fv-az99-305:08614] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f140b675951]
[fv-az99-305:08614] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f140b68147c]
[fv-az99-305:08614] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f140b6814e7]
[fv-az99-305:08614] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f140b681799]
[fv-az99-305:08614] [ 7] plumed(+0xf47d)[0x558a7821e47d]
[fv-az99-305:08614] [ 8] plumed(+0x14004)[0x558a78223004]
[fv-az99-305:08614] [ 9] plumed(+0xf698)[0x558a7821e698]
[fv-az99-305:08614] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f140b3ef0b3]
[fv-az99-305:08614] [11] plumed(+0xf76e)[0x558a7821e76e]
[fv-az99-305:08614] *** End of error message ***
</pre>
{% endraw %}
