**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/4REP/plumed_4REP.dat   
(download [zipped raw stdout](plumed_4REP.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44032] *** Process received signal ***
[fv-az99-305:44032] Signal: Aborted (6)
[fv-az99-305:44032] Signal code:  (-6)
[fv-az99-305:44032] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc8ecc9c210]
[fv-az99-305:44032] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc8ecc9c18b]
[fv-az99-305:44032] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc8ecc7b859]
[fv-az99-305:44032] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc8ecf03951]
[fv-az99-305:44032] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc8ecf0f47c]
[fv-az99-305:44032] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc8ecf0f4e7]
[fv-az99-305:44032] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc8ecf0f799]
[fv-az99-305:44032] [ 7] plumed(+0xf47d)[0x55875a8b747d]
[fv-az99-305:44032] [ 8] plumed(+0x14004)[0x55875a8bc004]
[fv-az99-305:44032] [ 9] plumed(+0xf698)[0x55875a8b7698]
[fv-az99-305:44032] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc8ecc7d0b3]
[fv-az99-305:44032] [11] plumed(+0xf76e)[0x55875a8b776e]
[fv-az99-305:44032] *** End of error message ***
</pre>
{% endraw %}
