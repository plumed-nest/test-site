**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-jax1/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=jaxcv FUNCTION=cv1
Maybe a missing space or a typo?
[fv-az99-305:30423] *** Process received signal ***
[fv-az99-305:30423] Signal: Aborted (6)
[fv-az99-305:30423] Signal code:  (-6)
[fv-az99-305:30423] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7283145210]
[fv-az99-305:30423] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f728314518b]
[fv-az99-305:30423] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7283124859]
[fv-az99-305:30423] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f72833ac951]
[fv-az99-305:30423] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f72833b847c]
[fv-az99-305:30423] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f72833b84e7]
[fv-az99-305:30423] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f72833b8799]
[fv-az99-305:30423] [ 7] plumed(+0xf47d)[0x5557b9ed047d]
[fv-az99-305:30423] [ 8] plumed(+0x14004)[0x5557b9ed5004]
[fv-az99-305:30423] [ 9] plumed(+0xf698)[0x5557b9ed0698]
[fv-az99-305:30423] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f72831260b3]
[fv-az99-305:30423] [11] plumed(+0xf76e)[0x5557b9ed076e]
[fv-az99-305:30423] *** End of error message ***
</pre>
{% endraw %}
