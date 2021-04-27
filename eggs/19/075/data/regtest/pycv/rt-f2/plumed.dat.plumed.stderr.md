**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f2/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=cc1 ARG=t1,t2,t3 IMPORT=pythonfunction FUNCTION=cc1 PERIODIC=NO
Maybe a missing space or a typo?
[fv-az99-305:30398] *** Process received signal ***
[fv-az99-305:30398] Signal: Aborted (6)
[fv-az99-305:30398] Signal code:  (-6)
[fv-az99-305:30398] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0a60179210]
[fv-az99-305:30398] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0a6017918b]
[fv-az99-305:30398] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0a60158859]
[fv-az99-305:30398] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0a603e0951]
[fv-az99-305:30398] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0a603ec47c]
[fv-az99-305:30398] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0a603ec4e7]
[fv-az99-305:30398] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f0a603ec799]
[fv-az99-305:30398] [ 7] plumed(+0xf47d)[0x5570d34ff47d]
[fv-az99-305:30398] [ 8] plumed(+0x14004)[0x5570d3504004]
[fv-az99-305:30398] [ 9] plumed(+0xf698)[0x5570d34ff698]
[fv-az99-305:30398] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0a6015a0b3]
[fv-az99-305:30398] [11] plumed(+0xf76e)[0x5570d34ff76e]
[fv-az99-305:30398] *** End of error message ***
</pre>
{% endraw %}
