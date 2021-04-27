**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
Stderr for source:  fun_metaD/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PROJECTION_ON_AXIS LABEL=pp AXIS_ATOMS=p1,p2_FS2 ATOM=lig
Maybe a missing space or a typo?
[fv-az99-305:23547] *** Process received signal ***
[fv-az99-305:23547] Signal: Aborted (6)
[fv-az99-305:23547] Signal code:  (-6)
[fv-az99-305:23547] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd4dd6c8210]
[fv-az99-305:23547] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd4dd6c818b]
[fv-az99-305:23547] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd4dd6a7859]
[fv-az99-305:23547] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd4dd92f951]
[fv-az99-305:23547] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd4dd93b47c]
[fv-az99-305:23547] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd4dd93b4e7]
[fv-az99-305:23547] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fd4dd93b7ed]
[fv-az99-305:23547] [ 7] plumed_master(+0xf568)[0x555e6b7c1568]
[fv-az99-305:23547] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd4dd6a90b3]
[fv-az99-305:23547] [ 9] plumed_master(+0xf79e)[0x555e6b7c179e]
[fv-az99-305:23547] *** End of error message ***
</pre>
{% endraw %}
