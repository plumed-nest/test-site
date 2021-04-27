**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/6_D/plumed_reweight.dat   
(download [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=10
Maybe a missing space or a typo?
[fv-az99-305:26948] *** Process received signal ***
[fv-az99-305:26948] Signal: Aborted (6)
[fv-az99-305:26948] Signal code:  (-6)
[fv-az99-305:26948] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f0ddd31e210]
[fv-az99-305:26948] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0ddd31e18b]
[fv-az99-305:26948] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0ddd2fd859]
[fv-az99-305:26948] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f0ddd585951]
[fv-az99-305:26948] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f0ddd59147c]
[fv-az99-305:26948] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f0ddd5914e7]
[fv-az99-305:26948] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f0ddd5917ed]
[fv-az99-305:26948] [ 7] plumed_master(+0xf568)[0x5605c8613568]
[fv-az99-305:26948] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0ddd2ff0b3]
[fv-az99-305:26948] [ 9] plumed_master(+0xf79e)[0x5605c861379e]
[fv-az99-305:26948] *** End of error message ***
</pre>
{% endraw %}
