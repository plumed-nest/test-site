**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5-6/g1-w13-s4.625/plumed.dat   
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
[fv-az99-305:14475] *** Process received signal ***
[fv-az99-305:14475] Signal: Aborted (6)
[fv-az99-305:14475] Signal code:  (-6)
[fv-az99-305:14475] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f26c5671210]
[fv-az99-305:14475] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f26c567118b]
[fv-az99-305:14475] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f26c5650859]
[fv-az99-305:14475] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f26c58d8951]
[fv-az99-305:14475] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f26c58e447c]
[fv-az99-305:14475] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f26c58e44e7]
[fv-az99-305:14475] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f26c58e4799]
[fv-az99-305:14475] [ 7] plumed(+0xf47d)[0x5575bd1ae47d]
[fv-az99-305:14475] [ 8] plumed(+0x14004)[0x5575bd1b3004]
[fv-az99-305:14475] [ 9] plumed(+0xf698)[0x5575bd1ae698]
[fv-az99-305:14475] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f26c56520b3]
[fv-az99-305:14475] [11] plumed(+0xf76e)[0x5575bd1ae76e]
[fv-az99-305:14475] *** End of error message ***
</pre>
{% endraw %}
