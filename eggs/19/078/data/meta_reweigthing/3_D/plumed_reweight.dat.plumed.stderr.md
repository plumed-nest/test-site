**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/3_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=20
Maybe a missing space or a typo?
[fv-az1113-981:45150] *** Process received signal ***
[fv-az1113-981:45150] Signal: Aborted (6)
[fv-az1113-981:45150] Signal code:  (-6)
[fv-az1113-981:45150] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f25ebc42520]
[fv-az1113-981:45150] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f25ebc969fc]
[fv-az1113-981:45150] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f25ebc42476]
[fv-az1113-981:45150] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f25ebc287f3]
[fv-az1113-981:45150] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f25ec0a2b9e]
[fv-az1113-981:45150] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f25ec0ae20c]
[fv-az1113-981:45150] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f25ec0ae277]
[fv-az1113-981:45150] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f25ec0ae52b]
[fv-az1113-981:45150] [ 8] plumed(+0x12f48)[0x55bf474b0f48]
[fv-az1113-981:45150] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f25ebc29d90]
[fv-az1113-981:45150] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f25ebc29e40]
[fv-az1113-981:45150] [11] plumed(+0x131e5)[0x55bf474b11e5]
[fv-az1113-981:45150] *** End of error message ***
</pre>
{% endraw %}
