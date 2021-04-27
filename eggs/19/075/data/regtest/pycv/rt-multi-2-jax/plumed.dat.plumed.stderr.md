**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-2-jax/plumed.dat   
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
[fv-az99-305:30522] *** Process received signal ***
[fv-az99-305:30522] Signal: Aborted (6)
[fv-az99-305:30522] Signal code:  (-6)
[fv-az99-305:30522] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4c6ff24210]
[fv-az99-305:30522] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4c6ff2418b]
[fv-az99-305:30522] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4c6ff03859]
[fv-az99-305:30522] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4c7018b951]
[fv-az99-305:30522] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4c7019747c]
[fv-az99-305:30522] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4c701974e7]
[fv-az99-305:30522] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4c70197799]
[fv-az99-305:30522] [ 7] plumed(+0xf47d)[0x564f95ddf47d]
[fv-az99-305:30522] [ 8] plumed(+0x14004)[0x564f95de4004]
[fv-az99-305:30522] [ 9] plumed(+0xf698)[0x564f95ddf698]
[fv-az99-305:30522] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4c6ff050b3]
[fv-az99-305:30522] [11] plumed(+0xf76e)[0x564f95ddf76e]
[fv-az99-305:30522] *** End of error message ***
</pre>
{% endraw %}
