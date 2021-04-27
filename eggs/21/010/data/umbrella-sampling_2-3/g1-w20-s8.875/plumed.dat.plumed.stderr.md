**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w20-s8.875/plumed.dat   
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
[fv-az99-305:10286] *** Process received signal ***
[fv-az99-305:10286] Signal: Aborted (6)
[fv-az99-305:10286] Signal code:  (-6)
[fv-az99-305:10286] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4aad22a210]
[fv-az99-305:10286] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4aad22a18b]
[fv-az99-305:10286] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4aad209859]
[fv-az99-305:10286] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4aad491951]
[fv-az99-305:10286] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4aad49d47c]
[fv-az99-305:10286] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4aad49d4e7]
[fv-az99-305:10286] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4aad49d799]
[fv-az99-305:10286] [ 7] plumed(+0xf47d)[0x5631e73bd47d]
[fv-az99-305:10286] [ 8] plumed(+0x14004)[0x5631e73c2004]
[fv-az99-305:10286] [ 9] plumed(+0xf698)[0x5631e73bd698]
[fv-az99-305:10286] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4aad20b0b3]
[fv-az99-305:10286] [11] plumed(+0xf76e)[0x5631e73bd76e]
[fv-az99-305:10286] *** End of error message ***
</pre>
{% endraw %}
