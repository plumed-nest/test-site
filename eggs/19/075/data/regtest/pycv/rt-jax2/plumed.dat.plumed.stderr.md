**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax2/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4,3 IMPORT=jaxcv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az99-305:30447] *** Process received signal ***
[fv-az99-305:30447] Signal: Aborted (6)
[fv-az99-305:30447] Signal code:  (-6)
[fv-az99-305:30447] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f35d1354210]
[fv-az99-305:30447] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f35d135418b]
[fv-az99-305:30447] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f35d1333859]
[fv-az99-305:30447] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f35d15bb951]
[fv-az99-305:30447] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f35d15c747c]
[fv-az99-305:30447] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f35d15c74e7]
[fv-az99-305:30447] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f35d15c7799]
[fv-az99-305:30447] [ 7] plumed(+0xf47d)[0x5639b360a47d]
[fv-az99-305:30447] [ 8] plumed(+0x14004)[0x5639b360f004]
[fv-az99-305:30447] [ 9] plumed(+0xf698)[0x5639b360a698]
[fv-az99-305:30447] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f35d13350b3]
[fv-az99-305:30447] [11] plumed(+0xf76e)[0x5639b360a76e]
[fv-az99-305:30447] *** End of error message ***
</pre>
{% endraw %}
