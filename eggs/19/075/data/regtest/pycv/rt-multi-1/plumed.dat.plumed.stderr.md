**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az99-305:30497] *** Process received signal ***
[fv-az99-305:30497] Signal: Aborted (6)
[fv-az99-305:30497] Signal code:  (-6)
[fv-az99-305:30497] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f938835f210]
[fv-az99-305:30497] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f938835f18b]
[fv-az99-305:30497] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f938833e859]
[fv-az99-305:30497] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f93885c6951]
[fv-az99-305:30497] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f93885d247c]
[fv-az99-305:30497] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f93885d24e7]
[fv-az99-305:30497] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f93885d2799]
[fv-az99-305:30497] [ 7] plumed(+0xf47d)[0x556c7d03a47d]
[fv-az99-305:30497] [ 8] plumed(+0x14004)[0x556c7d03f004]
[fv-az99-305:30497] [ 9] plumed(+0xf698)[0x556c7d03a698]
[fv-az99-305:30497] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f93883400b3]
[fv-az99-305:30497] [11] plumed(+0xf76e)[0x556c7d03a76e]
[fv-az99-305:30497] *** End of error message ***
</pre>
{% endraw %}
