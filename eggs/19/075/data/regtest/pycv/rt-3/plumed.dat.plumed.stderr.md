**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az99-305:30349] *** Process received signal ***
[fv-az99-305:30349] Signal: Aborted (6)
[fv-az99-305:30349] Signal code:  (-6)
[fv-az99-305:30349] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1aa5dea210]
[fv-az99-305:30349] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f1aa5dea18b]
[fv-az99-305:30349] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1aa5dc9859]
[fv-az99-305:30349] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f1aa6051951]
[fv-az99-305:30349] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f1aa605d47c]
[fv-az99-305:30349] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f1aa605d4e7]
[fv-az99-305:30349] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f1aa605d799]
[fv-az99-305:30349] [ 7] plumed(+0xf47d)[0x562d8db2f47d]
[fv-az99-305:30349] [ 8] plumed(+0x14004)[0x562d8db34004]
[fv-az99-305:30349] [ 9] plumed(+0xf698)[0x562d8db2f698]
[fv-az99-305:30349] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f1aa5dcb0b3]
[fv-az99-305:30349] [11] plumed(+0xf76e)[0x562d8db2f76e]
[fv-az99-305:30349] *** End of error message ***
</pre>
{% endraw %}
