**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_5prime-5/g1-w6-s3.650/plumed.dat   
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
[fv-az99-305:16242] *** Process received signal ***
[fv-az99-305:16242] Signal: Aborted (6)
[fv-az99-305:16242] Signal code:  (-6)
[fv-az99-305:16242] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc45860c210]
[fv-az99-305:16242] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc45860c18b]
[fv-az99-305:16242] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc4585eb859]
[fv-az99-305:16242] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc458873951]
[fv-az99-305:16242] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc45887f47c]
[fv-az99-305:16242] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc45887f4e7]
[fv-az99-305:16242] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc45887f799]
[fv-az99-305:16242] [ 7] plumed(+0xf47d)[0x556d0e33747d]
[fv-az99-305:16242] [ 8] plumed(+0x14004)[0x556d0e33c004]
[fv-az99-305:16242] [ 9] plumed(+0xf698)[0x556d0e337698]
[fv-az99-305:16242] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc4585ed0b3]
[fv-az99-305:16242] [11] plumed(+0xf76e)[0x556d0e33776e]
[fv-az99-305:16242] *** End of error message ***
</pre>
{% endraw %}
