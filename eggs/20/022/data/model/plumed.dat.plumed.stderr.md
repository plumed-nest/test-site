**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
Stderr for source:  model/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_UMBRELLAS_LINE LABEL=ecv ARG=p.x MIN_CV=-2.5 MAX_CV=2.5 SIGMA=0.185815
Maybe a missing space or a typo?
[fv-az99-305:22444] *** Process received signal ***
[fv-az99-305:22444] Signal: Aborted (6)
[fv-az99-305:22444] Signal code:  (-6)
[fv-az99-305:22444] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f59dee9f210]
[fv-az99-305:22444] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f59dee9f18b]
[fv-az99-305:22444] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f59dee7e859]
[fv-az99-305:22444] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f59df106951]
[fv-az99-305:22444] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f59df11247c]
[fv-az99-305:22444] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f59df1124e7]
[fv-az99-305:22444] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f59df112799]
[fv-az99-305:22444] [ 7] plumed(+0xf47d)[0x560e54b7147d]
[fv-az99-305:22444] [ 8] plumed(+0x14004)[0x560e54b76004]
[fv-az99-305:22444] [ 9] plumed(+0xf698)[0x560e54b71698]
[fv-az99-305:22444] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f59dee800b3]
[fv-az99-305:22444] [11] plumed(+0xf76e)[0x560e54b7176e]
[fv-az99-305:22444] *** End of error message ***
</pre>
{% endraw %}
