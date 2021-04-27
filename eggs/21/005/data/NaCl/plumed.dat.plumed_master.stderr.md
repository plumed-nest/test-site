**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  NaCl/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTORCH_MODEL LABEL=auto1 MODEL=nacl_sfNa_ct1.pt ARG=s1.Sk3_-3_-3,s1.Sk3_-3_3,s1.Sk3_3_-3,s1.Sk3_3_3,s1.Sk6_0_0,s1.Sk0_6_-6,s1.Sk0_6_6,s1.Sk6_-6_0,s1.Sk6_0_-6,s1.Sk6_0_6,s1.Sk6_6_0,s1.Sk9_-3_-3,s1.Sk9_-3_3,s1.Sk9_3_-3,s1.Sk9_3_3
Maybe a missing space or a typo?
[fv-az99-305:17705] *** Process received signal ***
[fv-az99-305:17705] Signal: Aborted (6)
[fv-az99-305:17705] Signal code:  (-6)
[fv-az99-305:17705] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7b03215210]
[fv-az99-305:17705] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7b0321518b]
[fv-az99-305:17705] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7b031f4859]
[fv-az99-305:17705] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7b0347c951]
[fv-az99-305:17705] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7b0348847c]
[fv-az99-305:17705] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7b034884e7]
[fv-az99-305:17705] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f7b034887ed]
[fv-az99-305:17705] [ 7] plumed_master(+0xf568)[0x561836b60568]
[fv-az99-305:17705] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7b031f60b3]
[fv-az99-305:17705] [ 9] plumed_master(+0xf79e)[0x561836b6079e]
[fv-az99-305:17705] *** End of error message ***
</pre>
{% endraw %}
