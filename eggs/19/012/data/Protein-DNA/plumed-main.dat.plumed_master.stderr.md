**Project ID:** [plumID:19.012]({{ '/' | absolute_url }}eggs/19/012/)  
Stderr for source:  ./Protein-DNA/plumed-main.dat   
(download [zipped raw stdout](plumed-main.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:128, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (saxsdata\.biasDer)
[fv-az99-305:43536] *** Process received signal ***
[fv-az99-305:43536] Signal: Aborted (6)
[fv-az99-305:43536] Signal code:  (-6)
[fv-az99-305:43536] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fe84cd64210]
[fv-az99-305:43536] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fe84cd6418b]
[fv-az99-305:43536] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fe84cd43859]
[fv-az99-305:43536] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fe84cfcb951]
[fv-az99-305:43536] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fe84cfd747c]
[fv-az99-305:43536] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fe84cfd74e7]
[fv-az99-305:43536] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fe84cfd77ed]
[fv-az99-305:43536] [ 7] plumed_master(+0xf568)[0x56139f8b4568]
[fv-az99-305:43536] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fe84cd450b3]
[fv-az99-305:43536] [ 9] plumed_master(+0xf79e)[0x56139f8b479e]
[fv-az99-305:43536] *** End of error message ***
</pre>
{% endraw %}
