**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/8REP/plumed_8REP.dat   
(download [zipped raw stdout](plumed_8REP.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44065] *** Process received signal ***
[fv-az99-305:44065] Signal: Aborted (6)
[fv-az99-305:44065] Signal code:  (-6)
[fv-az99-305:44065] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f88bd7b8210]
[fv-az99-305:44065] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f88bd7b818b]
[fv-az99-305:44065] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f88bd797859]
[fv-az99-305:44065] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f88bda1f951]
[fv-az99-305:44065] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f88bda2b47c]
[fv-az99-305:44065] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f88bda2b4e7]
[fv-az99-305:44065] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f88bda2b7ed]
[fv-az99-305:44065] [ 7] plumed_master(+0xf568)[0x55b184033568]
[fv-az99-305:44065] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f88bd7990b3]
[fv-az99-305:44065] [ 9] plumed_master(+0xf79e)[0x55b18403379e]
[fv-az99-305:44065] *** End of error message ***
</pre>
{% endraw %}
