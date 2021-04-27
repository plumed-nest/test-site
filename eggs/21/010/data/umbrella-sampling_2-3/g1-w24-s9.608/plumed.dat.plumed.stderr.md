**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g1-w24-s9.608/plumed.dat   
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
[fv-az99-305:10383] *** Process received signal ***
[fv-az99-305:10383] Signal: Aborted (6)
[fv-az99-305:10383] Signal code:  (-6)
[fv-az99-305:10383] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f3eea303210]
[fv-az99-305:10383] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f3eea30318b]
[fv-az99-305:10383] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f3eea2e2859]
[fv-az99-305:10383] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f3eea56a951]
[fv-az99-305:10383] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f3eea57647c]
[fv-az99-305:10383] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f3eea5764e7]
[fv-az99-305:10383] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f3eea576799]
[fv-az99-305:10383] [ 7] plumed(+0xf47d)[0x5625c28ad47d]
[fv-az99-305:10383] [ 8] plumed(+0x14004)[0x5625c28b2004]
[fv-az99-305:10383] [ 9] plumed(+0xf698)[0x5625c28ad698]
[fv-az99-305:10383] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f3eea2e40b3]
[fv-az99-305:10383] [11] plumed(+0xf76e)[0x5625c28ad76e]
[fv-az99-305:10383] *** End of error message ***
</pre>
{% endraw %}
