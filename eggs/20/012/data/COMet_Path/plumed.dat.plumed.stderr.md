**Project ID:** [plumID:20.012]({{ '/' | absolute_url }}eggs/20/012/)  
Stderr for source:  COMet_Path/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: PROJECTION_ON_AXIS LABEL=pp AXIS_ATOMS=p1,p2_FS2 ATOM=lig
Maybe a missing space or a typo?
[fv-az99-305:23382] *** Process received signal ***
[fv-az99-305:23382] Signal: Aborted (6)
[fv-az99-305:23382] Signal code:  (-6)
[fv-az99-305:23382] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fae8008a210]
[fv-az99-305:23382] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fae8008a18b]
[fv-az99-305:23382] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fae80069859]
[fv-az99-305:23382] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fae802f1951]
[fv-az99-305:23382] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fae802fd47c]
[fv-az99-305:23382] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fae802fd4e7]
[fv-az99-305:23382] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fae802fd799]
[fv-az99-305:23382] [ 7] plumed(+0xf47d)[0x5649e218647d]
[fv-az99-305:23382] [ 8] plumed(+0x14004)[0x5649e218b004]
[fv-az99-305:23382] [ 9] plumed(+0xf698)[0x5649e2186698]
[fv-az99-305:23382] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fae8006b0b3]
[fv-az99-305:23382] [11] plumed(+0xf76e)[0x5649e218676e]
[fv-az99-305:23382] *** End of error message ***
</pre>
{% endraw %}
