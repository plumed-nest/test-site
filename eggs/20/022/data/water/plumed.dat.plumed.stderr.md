**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
Stderr for source:  water/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_LINEAR LABEL=ecv ARG=DeltaU TEMP=443
Maybe a missing space or a typo?
[fv-az99-305:22491] *** Process received signal ***
[fv-az99-305:22491] Signal: Aborted (6)
[fv-az99-305:22491] Signal code:  (-6)
[fv-az99-305:22491] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdcb1365210]
[fv-az99-305:22491] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdcb136518b]
[fv-az99-305:22491] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdcb1344859]
[fv-az99-305:22491] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdcb15cc951]
[fv-az99-305:22491] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdcb15d847c]
[fv-az99-305:22491] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdcb15d84e7]
[fv-az99-305:22491] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdcb15d8799]
[fv-az99-305:22491] [ 7] plumed(+0xf47d)[0x55806ffdb47d]
[fv-az99-305:22491] [ 8] plumed(+0x14004)[0x55806ffe0004]
[fv-az99-305:22491] [ 9] plumed(+0xf698)[0x55806ffdb698]
[fv-az99-305:22491] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdcb13460b3]
[fv-az99-305:22491] [11] plumed(+0xf76e)[0x55806ffdb76e]
[fv-az99-305:22491] *** End of error message ***
</pre>
{% endraw %}
