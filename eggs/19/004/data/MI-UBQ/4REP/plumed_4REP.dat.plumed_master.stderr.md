**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/4REP/plumed_4REP.dat   
(download [zipped raw stdout](plumed_4REP.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44040] *** Process received signal ***
[fv-az99-305:44040] Signal: Aborted (6)
[fv-az99-305:44040] Signal code:  (-6)
[fv-az99-305:44040] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f13eb84d210]
[fv-az99-305:44040] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f13eb84d18b]
[fv-az99-305:44040] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f13eb82c859]
[fv-az99-305:44040] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f13ebab4951]
[fv-az99-305:44040] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f13ebac047c]
[fv-az99-305:44040] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f13ebac04e7]
[fv-az99-305:44040] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f13ebac07ed]
[fv-az99-305:44040] [ 7] plumed_master(+0xf568)[0x564ae61bb568]
[fv-az99-305:44040] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f13eb82e0b3]
[fv-az99-305:44040] [ 9] plumed_master(+0xf79e)[0x564ae61bb79e]
[fv-az99-305:44040] *** End of error message ***
</pre>
{% endraw %}
