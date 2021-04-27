**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w26-s9.370/plumed.dat   
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
[fv-az99-305:12290] *** Process received signal ***
[fv-az99-305:12290] Signal: Aborted (6)
[fv-az99-305:12290] Signal code:  (-6)
[fv-az99-305:12290] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7efd55314210]
[fv-az99-305:12290] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7efd5531418b]
[fv-az99-305:12290] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7efd552f3859]
[fv-az99-305:12290] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7efd5557b951]
[fv-az99-305:12290] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7efd5558747c]
[fv-az99-305:12290] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7efd555874e7]
[fv-az99-305:12290] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7efd55587799]
[fv-az99-305:12290] [ 7] plumed(+0xf47d)[0x55d8ea27e47d]
[fv-az99-305:12290] [ 8] plumed(+0x14004)[0x55d8ea283004]
[fv-az99-305:12290] [ 9] plumed(+0xf698)[0x55d8ea27e698]
[fv-az99-305:12290] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7efd552f50b3]
[fv-az99-305:12290] [11] plumed(+0xf76e)[0x55d8ea27e76e]
[fv-az99-305:12290] *** End of error message ***
</pre>
{% endraw %}
