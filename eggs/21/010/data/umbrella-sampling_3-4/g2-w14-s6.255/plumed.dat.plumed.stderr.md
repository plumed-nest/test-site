**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w14-s6.255/plumed.dat   
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
[fv-az99-305:11972] *** Process received signal ***
[fv-az99-305:11972] Signal: Aborted (6)
[fv-az99-305:11972] Signal code:  (-6)
[fv-az99-305:11972] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fce84272210]
[fv-az99-305:11972] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fce8427218b]
[fv-az99-305:11972] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fce84251859]
[fv-az99-305:11972] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fce844d9951]
[fv-az99-305:11972] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fce844e547c]
[fv-az99-305:11972] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fce844e54e7]
[fv-az99-305:11972] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fce844e5799]
[fv-az99-305:11972] [ 7] plumed(+0xf47d)[0x55b9adee847d]
[fv-az99-305:11972] [ 8] plumed(+0x14004)[0x55b9adeed004]
[fv-az99-305:11972] [ 9] plumed(+0xf698)[0x55b9adee8698]
[fv-az99-305:11972] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fce842530b3]
[fv-az99-305:11972] [11] plumed(+0xf76e)[0x55b9adee876e]
[fv-az99-305:11972] *** End of error message ***
</pre>
{% endraw %}
