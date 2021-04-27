**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/2_D/plumed_reweight.dat   
(download [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=20
Maybe a missing space or a typo?
[fv-az99-305:26801] *** Process received signal ***
[fv-az99-305:26801] Signal: Aborted (6)
[fv-az99-305:26801] Signal code:  (-6)
[fv-az99-305:26801] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f056a52c210]
[fv-az99-305:26801] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f056a52c18b]
[fv-az99-305:26801] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f056a50b859]
[fv-az99-305:26801] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f056a793951]
[fv-az99-305:26801] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f056a79f47c]
[fv-az99-305:26801] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f056a79f4e7]
[fv-az99-305:26801] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f056a79f799]
[fv-az99-305:26801] [ 7] plumed(+0xf47d)[0x55a903a1347d]
[fv-az99-305:26801] [ 8] plumed(+0x14004)[0x55a903a18004]
[fv-az99-305:26801] [ 9] plumed(+0xf698)[0x55a903a13698]
[fv-az99-305:26801] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f056a50d0b3]
[fv-az99-305:26801] [11] plumed(+0xf76e)[0x55a903a1376e]
[fv-az99-305:26801] *** End of error message ***
</pre>
{% endraw %}
