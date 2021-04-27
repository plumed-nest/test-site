**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_3-4/g2-w10-s5.216/plumed.dat   
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
[fv-az99-305:11873] *** Process received signal ***
[fv-az99-305:11873] Signal: Aborted (6)
[fv-az99-305:11873] Signal code:  (-6)
[fv-az99-305:11873] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fbbc7e45210]
[fv-az99-305:11873] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fbbc7e4518b]
[fv-az99-305:11873] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fbbc7e24859]
[fv-az99-305:11873] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fbbc80ac951]
[fv-az99-305:11873] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fbbc80b847c]
[fv-az99-305:11873] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fbbc80b84e7]
[fv-az99-305:11873] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fbbc80b8799]
[fv-az99-305:11873] [ 7] plumed(+0xf47d)[0x563e3b08447d]
[fv-az99-305:11873] [ 8] plumed(+0x14004)[0x563e3b089004]
[fv-az99-305:11873] [ 9] plumed(+0xf698)[0x563e3b084698]
[fv-az99-305:11873] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fbbc7e260b3]
[fv-az99-305:11873] [11] plumed(+0xf76e)[0x563e3b08476e]
[fv-az99-305:11873] *** End of error message ***
</pre>
{% endraw %}
