**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-2/plumed.dat   
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
[fv-az99-305:30325] *** Process received signal ***
[fv-az99-305:30325] Signal: Aborted (6)
[fv-az99-305:30325] Signal code:  (-6)
[fv-az99-305:30325] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fee23825210]
[fv-az99-305:30325] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fee2382518b]
[fv-az99-305:30325] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fee23804859]
[fv-az99-305:30325] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fee23a8c951]
[fv-az99-305:30325] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fee23a9847c]
[fv-az99-305:30325] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fee23a984e7]
[fv-az99-305:30325] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fee23a98799]
[fv-az99-305:30325] [ 7] plumed(+0xf47d)[0x55edbe73a47d]
[fv-az99-305:30325] [ 8] plumed(+0x14004)[0x55edbe73f004]
[fv-az99-305:30325] [ 9] plumed(+0xf698)[0x55edbe73a698]
[fv-az99-305:30325] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fee238060b3]
[fv-az99-305:30325] [11] plumed(+0xf76e)[0x55edbe73a76e]
[fv-az99-305:30325] *** End of error message ***
</pre>
{% endraw %}
