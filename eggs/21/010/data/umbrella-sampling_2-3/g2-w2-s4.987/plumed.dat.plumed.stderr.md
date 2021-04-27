**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_2-3/g2-w2-s4.987/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: HILLS RESTART HEIGHT 0.000 W_STRIDE 50
Maybe a missing space or a typo?
[fv-az99-305:10677] *** Process received signal ***
[fv-az99-305:10677] Signal: Aborted (6)
[fv-az99-305:10677] Signal code:  (-6)
[fv-az99-305:10677] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f6becdba210]
[fv-az99-305:10677] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f6becdba18b]
[fv-az99-305:10677] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f6becd99859]
[fv-az99-305:10677] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f6bed021951]
[fv-az99-305:10677] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f6bed02d47c]
[fv-az99-305:10677] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f6bed02d4e7]
[fv-az99-305:10677] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f6bed02d799]
[fv-az99-305:10677] [ 7] plumed(+0xf47d)[0x556c3b4cd47d]
[fv-az99-305:10677] [ 8] plumed(+0x14004)[0x556c3b4d2004]
[fv-az99-305:10677] [ 9] plumed(+0xf698)[0x556c3b4cd698]
[fv-az99-305:10677] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f6becd9b0b3]
[fv-az99-305:10677] [11] plumed(+0xf76e)[0x556c3b4cd76e]
[fv-az99-305:10677] *** End of error message ***
</pre>
{% endraw %}
