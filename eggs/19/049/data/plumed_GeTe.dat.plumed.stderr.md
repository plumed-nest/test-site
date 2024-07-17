**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_GeTe.dat   
Download: [zipped raw stdout](plumed_GeTe.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_GeTe.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: MORE_THAN LABEL=flq6 ARG=lq6 SWITCH=GAUSSIAN D_0=0.19 R_0=0.01 D_MAX=0.2
Maybe a missing space or a typo?
[fv-az774-16:73954] *** Process received signal ***
[fv-az774-16:73954] Signal: Aborted (6)
[fv-az774-16:73954] Signal code:  (-6)
[fv-az774-16:73954] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa80f042520]
[fv-az774-16:73954] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa80f0969fc]
[fv-az774-16:73954] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa80f042476]
[fv-az774-16:73954] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa80f0287f3]
[fv-az774-16:73954] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa80f4a2b9e]
[fv-az774-16:73954] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa80f4ae20c]
[fv-az774-16:73954] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa80f4ae277]
[fv-az774-16:73954] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa80f4ae52b]
[fv-az774-16:73954] [ 8] plumed(+0x12f48)[0x55be82d09f48]
[fv-az774-16:73954] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa80f029d90]
[fv-az774-16:73954] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa80f029e40]
[fv-az774-16:73954] [11] plumed(+0x131e5)[0x55be82d0a1e5]
[fv-az774-16:73954] *** End of error message ***
</pre>
{% endraw %}
