**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/8REP/plumed_8REP.dat   
(download [zipped raw stdout](plumed_8REP.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44057] *** Process received signal ***
[fv-az99-305:44057] Signal: Aborted (6)
[fv-az99-305:44057] Signal code:  (-6)
[fv-az99-305:44057] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fd532341210]
[fv-az99-305:44057] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fd53234118b]
[fv-az99-305:44057] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fd532320859]
[fv-az99-305:44057] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fd5325a8951]
[fv-az99-305:44057] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fd5325b447c]
[fv-az99-305:44057] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fd5325b44e7]
[fv-az99-305:44057] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fd5325b4799]
[fv-az99-305:44057] [ 7] plumed(+0xf47d)[0x565106fe147d]
[fv-az99-305:44057] [ 8] plumed(+0x14004)[0x565106fe6004]
[fv-az99-305:44057] [ 9] plumed(+0xf698)[0x565106fe1698]
[fv-az99-305:44057] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fd5323220b3]
[fv-az99-305:44057] [11] plumed(+0xf76e)[0x565106fe176e]
[fv-az99-305:44057] *** End of error message ***
</pre>
{% endraw %}
