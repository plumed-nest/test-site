**Project ID:** [plumID:21.005]({{ '/' | absolute_url }}eggs/21/005/)  
Stderr for source:  CO2/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PYTORCH_MODEL LABEL=auto1 MODEL=co2_333_sfO_tc1.pt ARG=so.Sk3_-3_-3,so.Sk3_-3_3,so.Sk3_3_-3,so.Sk3_3_3,so.Sk0_3_-6,so.Sk0_3_6,so.Sk0_6_-3,so.Sk0_6_3,so.Sk3_-6_0,so.Sk3_0_-6,so.Sk3_0_6,so.Sk3_6_0,so.Sk6_-3_0,so.Sk6_0_-3,so.Sk6_0_3,so.Sk6_3_0,so.Sk3_-6_-3,so.Sk3_-6_3,so.Sk3_-3_-6,so.Sk3_-3_6,so.Sk3_3_-6,so.Sk3_3_6,so.Sk3_6_-3,so.Sk3_6_3,so.Sk6_-3_-3,so.Sk6_-3_3,so.Sk6_3_-3,so.Sk6_3_3,so.Sk0_6_-9,so.Sk0_6_9,so.Sk0_9_-6,so.Sk0_9_6,so.Sk6_-9_0,so.Sk6_0_-9,so.Sk6_0_9,so.Sk6_9_0,so.Sk9_-6_0,so.Sk9_0_-6,so.Sk9_0_6,so.Sk9_6_0,so.Sk3_-9_-6,so.Sk3_-9_6,so.Sk3_-6_-9,so.Sk3_-6_9,so.Sk3_6_-9,so.Sk3_6_9,so.Sk3_9_-6,so.Sk3_9_6,so.Sk6_-9_-3,so.Sk6_-9_3,so.Sk6_-3_-9,so.Sk6_-3_9,so.Sk6_3_-9,so.Sk6_3_9,so.Sk6_9_-3,so.Sk6_9_3,so.Sk9_-6_-3,so.Sk9_-6_3,so.Sk9_-3_-6,so.Sk9_-3_6,so.Sk9_3_-6,so.Sk9_3_6,so.Sk9_6_-3,so.Sk9_6_3,so.Sk0_0_12,so.Sk0_12_0,so.Sk12_0_0
Maybe a missing space or a typo?
[fv-az99-305:17655] *** Process received signal ***
[fv-az99-305:17655] Signal: Aborted (6)
[fv-az99-305:17655] Signal code:  (-6)
[fv-az99-305:17655] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4354d96210]
[fv-az99-305:17655] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4354d9618b]
[fv-az99-305:17655] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4354d75859]
[fv-az99-305:17655] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4354ffd951]
[fv-az99-305:17655] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f435500947c]
[fv-az99-305:17655] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f43550094e7]
[fv-az99-305:17655] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f43550097ed]
[fv-az99-305:17655] [ 7] plumed_master(+0xf568)[0x55d48f608568]
[fv-az99-305:17655] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4354d770b3]
[fv-az99-305:17655] [ 9] plumed_master(+0xf79e)[0x55d48f60879e]
[fv-az99-305:17655] *** End of error message ***
</pre>
{% endraw %}
