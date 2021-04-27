**Project ID:** [plumID:19.004]({{ '/' | absolute_url }}eggs/19/004/)  
Stderr for source:  MI-UBQ/16REP/plumed_16REP.dat   
(download [zipped raw stdout](plumed_16REP.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at ActionWithArguments.cpp:129, function void PLMD::ActionWithArguments::interpretArgumentList(const std::vector<std::__cxx11::basic_string<char> >&, std::vector<PLMD::Value*>&)
+++ message follows +++
There isn't any action matching your regex (cs\.cb-.*)
[fv-az99-305:44008] *** Process received signal ***
[fv-az99-305:44008] Signal: Aborted (6)
[fv-az99-305:44008] Signal code:  (-6)
[fv-az99-305:44008] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7faf0698c210]
[fv-az99-305:44008] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7faf0698c18b]
[fv-az99-305:44008] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7faf0696b859]
[fv-az99-305:44008] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7faf06bf3951]
[fv-az99-305:44008] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7faf06bff47c]
[fv-az99-305:44008] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7faf06bff4e7]
[fv-az99-305:44008] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7faf06bff799]
[fv-az99-305:44008] [ 7] plumed(+0xf47d)[0x559f4c5e447d]
[fv-az99-305:44008] [ 8] plumed(+0x14004)[0x559f4c5e9004]
[fv-az99-305:44008] [ 9] plumed(+0xf698)[0x559f4c5e4698]
[fv-az99-305:44008] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7faf0696d0b3]
[fv-az99-305:44008] [11] plumed(+0xf76e)[0x559f4c5e476e]
[fv-az99-305:44008] *** End of error message ***
</pre>
{% endraw %}
