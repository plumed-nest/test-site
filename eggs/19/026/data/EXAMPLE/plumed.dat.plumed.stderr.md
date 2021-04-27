**Project ID:** [plumID:19.026]({{ '/' | absolute_url }}eggs/19/026/)  
Stderr for source:  EXAMPLE/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HBOND_COORD SPECIES=2665-10353:4 HYDROGENS=2666-10354:4,2667-10355:4 RCUTOO=0.324 RCUTOH=0.25 ACUT=0.20pi LABEL=hb
Maybe a missing space or a typo?
[fv-az99-305:40271] *** Process received signal ***
[fv-az99-305:40271] Signal: Aborted (6)
[fv-az99-305:40271] Signal code:  (-6)
[fv-az99-305:40271] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4f1ad00210]
[fv-az99-305:40271] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4f1ad0018b]
[fv-az99-305:40271] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4f1acdf859]
[fv-az99-305:40271] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4f1af67951]
[fv-az99-305:40271] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4f1af7347c]
[fv-az99-305:40271] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4f1af734e7]
[fv-az99-305:40271] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4f1af73799]
[fv-az99-305:40271] [ 7] plumed(+0xf47d)[0x564896aca47d]
[fv-az99-305:40271] [ 8] plumed(+0x14004)[0x564896acf004]
[fv-az99-305:40271] [ 9] plumed(+0xf698)[0x564896aca698]
[fv-az99-305:40271] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4f1ace10b3]
[fv-az99-305:40271] [11] plumed(+0xf76e)[0x564896aca76e]
[fv-az99-305:40271] *** End of error message ***
</pre>
{% endraw %}
