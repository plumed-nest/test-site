**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w19-s7.550/plumed.dat   
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
[fv-az99-305:15849] *** Process received signal ***
[fv-az99-305:15849] Signal: Aborted (6)
[fv-az99-305:15849] Signal code:  (-6)
[fv-az99-305:15849] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f711be46210]
[fv-az99-305:15849] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f711be4618b]
[fv-az99-305:15849] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f711be25859]
[fv-az99-305:15849] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f711c0ad951]
[fv-az99-305:15849] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f711c0b947c]
[fv-az99-305:15849] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f711c0b94e7]
[fv-az99-305:15849] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f711c0b9799]
[fv-az99-305:15849] [ 7] plumed(+0xf47d)[0x562fa3e9247d]
[fv-az99-305:15849] [ 8] plumed(+0x14004)[0x562fa3e97004]
[fv-az99-305:15849] [ 9] plumed(+0xf698)[0x562fa3e92698]
[fv-az99-305:15849] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f711be270b3]
[fv-az99-305:15849] [11] plumed(+0xf76e)[0x562fa3e9276e]
[fv-az99-305:15849] *** End of error message ***
</pre>
{% endraw %}
