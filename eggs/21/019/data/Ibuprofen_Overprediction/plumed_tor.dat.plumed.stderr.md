**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATOMS141=9314,9319,9310,9313
Maybe a missing space or a typo?
[fv-az1113-981:44153] *** Process received signal ***
[fv-az1113-981:44153] Signal: Aborted (6)
[fv-az1113-981:44153] Signal code:  (-6)
[fv-az1113-981:44153] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2b47442520]
[fv-az1113-981:44153] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2b474969fc]
[fv-az1113-981:44153] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2b47442476]
[fv-az1113-981:44153] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2b474287f3]
[fv-az1113-981:44153] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2b478a2b9e]
[fv-az1113-981:44153] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2b478ae20c]
[fv-az1113-981:44153] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2b478ae277]
[fv-az1113-981:44153] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2b478ae52b]
[fv-az1113-981:44153] [ 8] plumed(+0x12f48)[0x55ddc99e7f48]
[fv-az1113-981:44153] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2b47429d90]
[fv-az1113-981:44153] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2b47429e40]
[fv-az1113-981:44153] [11] plumed(+0x131e5)[0x55ddc99e81e5]
[fv-az1113-981:44153] *** End of error message ***
</pre>
{% endraw %}
