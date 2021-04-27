**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax3/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=r ATOMS=1,2,3 IMPORT=curvature FUNCTION=r
Maybe a missing space or a typo?
[fv-az99-305:30472] *** Process received signal ***
[fv-az99-305:30472] Signal: Aborted (6)
[fv-az99-305:30472] Signal code:  (-6)
[fv-az99-305:30472] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4c3168a210]
[fv-az99-305:30472] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4c3168a18b]
[fv-az99-305:30472] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4c31669859]
[fv-az99-305:30472] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4c318f1951]
[fv-az99-305:30472] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4c318fd47c]
[fv-az99-305:30472] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4c318fd4e7]
[fv-az99-305:30472] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4c318fd799]
[fv-az99-305:30472] [ 7] plumed(+0xf47d)[0x55d22880547d]
[fv-az99-305:30472] [ 8] plumed(+0x14004)[0x55d22880a004]
[fv-az99-305:30472] [ 9] plumed(+0xf698)[0x55d228805698]
[fv-az99-305:30472] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4c3166b0b3]
[fv-az99-305:30472] [11] plumed(+0xf76e)[0x55d22880576e]
[fv-az99-305:30472] *** End of error message ***
</pre>
{% endraw %}
