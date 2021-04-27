**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/16REP/plumed_16REP.dat   
(download [zipped raw stdout](plumed_16REP.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44016] *** Process received signal ***
[fv-az99-305:44016] Signal: Aborted (6)
[fv-az99-305:44016] Signal code:  (-6)
[fv-az99-305:44016] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f7a71f94210]
[fv-az99-305:44016] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f7a71f9418b]
[fv-az99-305:44016] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f7a71f73859]
[fv-az99-305:44016] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f7a721fb951]
[fv-az99-305:44016] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f7a7220747c]
[fv-az99-305:44016] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f7a722074e7]
[fv-az99-305:44016] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f7a722077ed]
[fv-az99-305:44016] [ 7] plumed_master(+0xf568)[0x556a9f645568]
[fv-az99-305:44016] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f7a71f750b3]
[fv-az99-305:44016] [ 9] plumed_master(+0xf79e)[0x556a9f64579e]
[fv-az99-305:44016] *** End of error message ***
</pre>
{% endraw %}
