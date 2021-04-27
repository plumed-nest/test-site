**Project ID:** [plumID:19.012]({{ '/' | absolute_url }}eggs/19/012/)  
Stderr for source:  ./Protein-DNA/plumed-main.dat   
(download [zipped raw stdout](plumed-main.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (saxsdata\.biasDer)
[fv-az99-305:43524] *** Process received signal ***
[fv-az99-305:43524] Signal: Aborted (6)
[fv-az99-305:43524] Signal code:  (-6)
[fv-az99-305:43524] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f4cb21d7210]
[fv-az99-305:43524] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f4cb21d718b]
[fv-az99-305:43524] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f4cb21b6859]
[fv-az99-305:43524] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f4cb243e951]
[fv-az99-305:43524] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f4cb244a47c]
[fv-az99-305:43524] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f4cb244a4e7]
[fv-az99-305:43524] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f4cb244a799]
[fv-az99-305:43524] [ 7] plumed(+0xf47d)[0x55c12598d47d]
[fv-az99-305:43524] [ 8] plumed(+0x14004)[0x55c125992004]
[fv-az99-305:43524] [ 9] plumed(+0xf698)[0x55c12598d698]
[fv-az99-305:43524] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f4cb21b80b3]
[fv-az99-305:43524] [11] plumed(+0xf76e)[0x55c12598d76e]
[fv-az99-305:43524] *** End of error message ***
</pre>
{% endraw %}
