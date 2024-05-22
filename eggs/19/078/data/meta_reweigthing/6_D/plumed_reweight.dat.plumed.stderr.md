**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/6_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=10
Maybe a missing space or a typo?
[fv-az1113-981:45241] *** Process received signal ***
[fv-az1113-981:45241] Signal: Aborted (6)
[fv-az1113-981:45241] Signal code:  (-6)
[fv-az1113-981:45241] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f49b2a42520]
[fv-az1113-981:45241] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f49b2a969fc]
[fv-az1113-981:45241] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f49b2a42476]
[fv-az1113-981:45241] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f49b2a287f3]
[fv-az1113-981:45241] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f49b2ea2b9e]
[fv-az1113-981:45241] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f49b2eae20c]
[fv-az1113-981:45241] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f49b2eae277]
[fv-az1113-981:45241] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f49b2eae52b]
[fv-az1113-981:45241] [ 8] plumed(+0x12f48)[0x55634dc91f48]
[fv-az1113-981:45241] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f49b2a29d90]
[fv-az1113-981:45241] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f49b2a29e40]
[fv-az1113-981:45241] [11] plumed(+0x131e5)[0x55634dc921e5]
[fv-az1113-981:45241] *** End of error message ***
</pre>
{% endraw %}
