**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1mfy/01-BENX/2-Production/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SHADOW LABEL=rmsd ATOMS=rna NOPBC UPDATE=100
Maybe a missing space or a typo?
[fv-az1113-981:40202] *** Process received signal ***
[fv-az1113-981:40202] Signal: Aborted (6)
[fv-az1113-981:40202] Signal code:  (-6)
[fv-az1113-981:40202] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8c07642520]
[fv-az1113-981:40202] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8c076969fc]
[fv-az1113-981:40202] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8c07642476]
[fv-az1113-981:40202] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8c076287f3]
[fv-az1113-981:40202] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8c07aa2b9e]
[fv-az1113-981:40202] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8c07aae20c]
[fv-az1113-981:40202] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8c07aae277]
[fv-az1113-981:40202] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8c07aae52b]
[fv-az1113-981:40202] [ 8] plumed(+0x12f48)[0x55f2efb33f48]
[fv-az1113-981:40202] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8c07629d90]
[fv-az1113-981:40202] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8c07629e40]
[fv-az1113-981:40202] [11] plumed(+0x131e5)[0x55f2efb341e5]
[fv-az1113-981:40202] *** End of error message ***
</pre>
{% endraw %}
