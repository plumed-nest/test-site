**Project ID:** [plumID:21.010]({{ '/' | absolute_url }}eggs/21/010/)  
Stderr for source:  umbrella-sampling_1-2prime/g1-w39-s9.516/plumed.dat   
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
[fv-az99-305:09326] *** Process received signal ***
[fv-az99-305:09326] Signal: Aborted (6)
[fv-az99-305:09326] Signal code:  (-6)
[fv-az99-305:09326] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fdb285a4210]
[fv-az99-305:09326] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fdb285a418b]
[fv-az99-305:09326] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fdb28583859]
[fv-az99-305:09326] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fdb2880b951]
[fv-az99-305:09326] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fdb2881747c]
[fv-az99-305:09326] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fdb288174e7]
[fv-az99-305:09326] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fdb28817799]
[fv-az99-305:09326] [ 7] plumed(+0xf47d)[0x55c34a9e047d]
[fv-az99-305:09326] [ 8] plumed(+0x14004)[0x55c34a9e5004]
[fv-az99-305:09326] [ 9] plumed(+0xf698)[0x55c34a9e0698]
[fv-az99-305:09326] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fdb285850b3]
[fv-az99-305:09326] [11] plumed(+0xf76e)[0x55c34a9e076e]
[fv-az99-305:09326] *** End of error message ***
</pre>
{% endraw %}
