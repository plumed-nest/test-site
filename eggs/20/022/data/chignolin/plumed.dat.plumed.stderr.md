**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
Stderr for source:  chignolin/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL_MULTIBARIC LABEL=ecv ARG=ene,vol MIN_TEMP=270 MAX_TEMP=800 PRESSURE=0.06022140857*2000 MIN_PRESSURE=0.06022140857 MAX_PRESSURE=0.06022140857*4000 CUT_CORNER=500,0.06022140857,800,0.06022140857*1000
Maybe a missing space or a typo?
[fv-az99-305:22421] *** Process received signal ***
[fv-az99-305:22421] Signal: Aborted (6)
[fv-az99-305:22421] Signal code:  (-6)
[fv-az99-305:22421] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc1e6565210]
[fv-az99-305:22421] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc1e656518b]
[fv-az99-305:22421] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc1e6544859]
[fv-az99-305:22421] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc1e67cc951]
[fv-az99-305:22421] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc1e67d847c]
[fv-az99-305:22421] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc1e67d84e7]
[fv-az99-305:22421] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc1e67d8799]
[fv-az99-305:22421] [ 7] plumed(+0xf47d)[0x5558e2f8c47d]
[fv-az99-305:22421] [ 8] plumed(+0x14004)[0x5558e2f91004]
[fv-az99-305:22421] [ 9] plumed(+0xf698)[0x5558e2f8c698]
[fv-az99-305:22421] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc1e65460b3]
[fv-az99-305:22421] [11] plumed(+0xf76e)[0x5558e2f8c76e]
[fv-az99-305:22421] *** End of error message ***
</pre>
{% endraw %}
