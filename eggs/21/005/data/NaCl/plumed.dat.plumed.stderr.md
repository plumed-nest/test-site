**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  NaCl/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTORCH_MODEL LABEL=auto1 MODEL=nacl_sfNa_ct1.pt ARG=s1.Sk3_-3_-3,s1.Sk3_-3_3,s1.Sk3_3_-3,s1.Sk3_3_3,s1.Sk6_0_0,s1.Sk0_6_-6,s1.Sk0_6_6,s1.Sk6_-6_0,s1.Sk6_0_-6,s1.Sk6_0_6,s1.Sk6_6_0,s1.Sk9_-3_-3,s1.Sk9_-3_3,s1.Sk9_3_-3,s1.Sk9_3_3
Maybe a missing space or a typo?
[fv-az99-305:17683] *** Process received signal ***
[fv-az99-305:17683] Signal: Aborted (6)
[fv-az99-305:17683] Signal code:  (-6)
[fv-az99-305:17683] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fad47fe8210]
[fv-az99-305:17683] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fad47fe818b]
[fv-az99-305:17683] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fad47fc7859]
[fv-az99-305:17683] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fad4824f951]
[fv-az99-305:17683] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fad4825b47c]
[fv-az99-305:17683] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fad4825b4e7]
[fv-az99-305:17683] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fad4825b799]
[fv-az99-305:17683] [ 7] plumed(+0xf47d)[0x555a18bea47d]
[fv-az99-305:17683] [ 8] plumed(+0x14004)[0x555a18bef004]
[fv-az99-305:17683] [ 9] plumed(+0xf698)[0x555a18bea698]
[fv-az99-305:17683] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fad47fc90b3]
[fv-az99-305:17683] [11] plumed(+0xf76e)[0x555a18bea76e]
[fv-az99-305:17683] *** End of error message ***
</pre>
{% endraw %}
