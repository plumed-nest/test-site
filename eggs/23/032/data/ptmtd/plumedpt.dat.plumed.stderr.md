**Project ID:** [plumID:23.032]({{ '/' | absolute_url }}eggs/23/032/)  
Stderr for source:  ptmtd/plumedpt.dat   
Download: [zipped raw stdout](plumedpt.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumedpt.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTORCH_MODEL_CV LABEL=ptm FILE=plumedpt.pt ATOMS=1,5,13,14,7,10,11,12,15,17,23,24,19,25,27,44,45,29,32,33,42,35,40,37,38,46,48,54,55,50,56,58,71,72,60,63,66,67,68,73,75,95,96,77,80,81,94,83,85,92,86,90,88,97,99,114,115,101,104,106,110,116,118,124,125,120,126,128,136,137,130,133,134,135,138,140,143,144,145,147,150,151,152,162,164,165,159,156,153,166,168,175,176,170,173,177,179,186,187,181,184,188,190,193,194,195,197,217,218,199,202,205,208,210,211,214,219,229,231,232,226,223,220,233,243,245,246,240,237,234,247,257,259,260,254,251,248,261,263,270,271,265,268,272
Maybe a missing space or a typo?
[fv-az774-16:69677] *** Process received signal ***
[fv-az774-16:69677] Signal: Aborted (6)
[fv-az774-16:69677] Signal code:  (-6)
[fv-az774-16:69677] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fec9b042520]
[fv-az774-16:69677] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fec9b0969fc]
[fv-az774-16:69677] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fec9b042476]
[fv-az774-16:69677] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fec9b0287f3]
[fv-az774-16:69677] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fec9b4a2b9e]
[fv-az774-16:69677] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fec9b4ae20c]
[fv-az774-16:69677] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fec9b4ae277]
[fv-az774-16:69677] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fec9b4ae52b]
[fv-az774-16:69677] [ 8] plumed(+0x12f48)[0x55a51ef81f48]
[fv-az774-16:69677] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fec9b029d90]
[fv-az774-16:69677] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fec9b029e40]
[fv-az774-16:69677] [11] plumed(+0x131e5)[0x55a51ef821e5]
[fv-az774-16:69677] *** End of error message ***
</pre>
{% endraw %}
