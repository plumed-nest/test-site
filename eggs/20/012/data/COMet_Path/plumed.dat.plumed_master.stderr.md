**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
Stderr for source:  COMet_Path/plumed.dat   
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
[fv-az99-305:23427] *** Process received signal ***
[fv-az99-305:23427] Signal: Aborted (6)
[fv-az99-305:23427] Signal code:  (-6)
[fv-az99-305:23427] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f1712472210]
[fv-az99-305:23427] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f171247218b]
[fv-az99-305:23427] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f1712451859]
[fv-az99-305:23427] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f17126d9951]
[fv-az99-305:23427] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f17126e547c]
[fv-az99-305:23427] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f17126e54e7]
[fv-az99-305:23427] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f17126e57ed]
[fv-az99-305:23427] [ 7] plumed_master(+0xf568)[0x562329239568]
[fv-az99-305:23427] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f17124530b3]
[fv-az99-305:23427] [ 9] plumed_master(+0xf79e)[0x56232923979e]
[fv-az99-305:23427] *** End of error message ***
</pre>
{% endraw %}
