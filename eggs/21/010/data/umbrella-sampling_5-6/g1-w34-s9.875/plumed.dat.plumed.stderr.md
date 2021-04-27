**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w34-s9.875/plumed.dat   
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
[fv-az99-305:15037] *** Process received signal ***
[fv-az99-305:15037] Signal: Aborted (6)
[fv-az99-305:15037] Signal code:  (-6)
[fv-az99-305:15037] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f79846a2210]
[fv-az99-305:15037] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f79846a218b]
[fv-az99-305:15037] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7984681859]
[fv-az99-305:15037] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7984909951]
[fv-az99-305:15037] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f798491547c]
[fv-az99-305:15037] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f79849154e7]
[fv-az99-305:15037] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f7984915799]
[fv-az99-305:15037] [ 7] plumed(+0xf47d)[0x55b63de6647d]
[fv-az99-305:15037] [ 8] plumed(+0x14004)[0x55b63de6b004]
[fv-az99-305:15037] [ 9] plumed(+0xf698)[0x55b63de66698]
[fv-az99-305:15037] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f79846830b3]
[fv-az99-305:15037] [11] plumed(+0xf76e)[0x55b63de6676e]
[fv-az99-305:15037] *** End of error message ***
</pre>
{% endraw %}
