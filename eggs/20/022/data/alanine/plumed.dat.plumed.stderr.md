**Project ID:** [plumID:20.022]({{ '/' | absolute_url }}eggs/20/022/)  
Stderr for source:  alanine/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: ECV_MULTITHERMAL LABEL=ecv ARG=ene MAX_TEMP=1000
Maybe a missing space or a typo?
[fv-az99-305:22398] *** Process received signal ***
[fv-az99-305:22398] Signal: Aborted (6)
[fv-az99-305:22398] Signal code:  (-6)
[fv-az99-305:22398] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6ef4ece210]
[fv-az99-305:22398] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6ef4ece18b]
[fv-az99-305:22398] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6ef4ead859]
[fv-az99-305:22398] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6ef5135951]
[fv-az99-305:22398] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6ef514147c]
[fv-az99-305:22398] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6ef51414e7]
[fv-az99-305:22398] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f6ef5141799]
[fv-az99-305:22398] [ 7] plumed(+0xf47d)[0x5558e9e6247d]
[fv-az99-305:22398] [ 8] plumed(+0x14004)[0x5558e9e67004]
[fv-az99-305:22398] [ 9] plumed(+0xf698)[0x5558e9e62698]
[fv-az99-305:22398] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6ef4eaf0b3]
[fv-az99-305:22398] [11] plumed(+0xf76e)[0x5558e9e6276e]
[fv-az99-305:22398] *** End of error message ***
</pre>
{% endraw %}
