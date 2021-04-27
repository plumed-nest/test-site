**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/6_D/plumed_reweight.dat   
(download [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=10
Maybe a missing space or a typo?
[fv-az99-305:26940] *** Process received signal ***
[fv-az99-305:26940] Signal: Aborted (6)
[fv-az99-305:26940] Signal code:  (-6)
[fv-az99-305:26940] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f259549d210]
[fv-az99-305:26940] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f259549d18b]
[fv-az99-305:26940] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f259547c859]
[fv-az99-305:26940] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f2595704951]
[fv-az99-305:26940] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f259571047c]
[fv-az99-305:26940] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f25957104e7]
[fv-az99-305:26940] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f2595710799]
[fv-az99-305:26940] [ 7] plumed(+0xf47d)[0x55bcef52e47d]
[fv-az99-305:26940] [ 8] plumed(+0x14004)[0x55bcef533004]
[fv-az99-305:26940] [ 9] plumed(+0xf698)[0x55bcef52e698]
[fv-az99-305:26940] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f259547e0b3]
[fv-az99-305:26940] [11] plumed(+0xf76e)[0x55bcef52e76e]
[fv-az99-305:26940] *** End of error message ***
</pre>
{% endraw %}
