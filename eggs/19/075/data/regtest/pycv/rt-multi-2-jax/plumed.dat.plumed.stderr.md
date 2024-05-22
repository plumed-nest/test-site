**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-multi-2-jax/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,3,4 IMPORT=distcv FUNCTION=cv COMPONENTS=d12,d13
Maybe a missing space or a typo?
[fv-az1109-238:41571] *** Process received signal ***
[fv-az1109-238:41571] Signal: Aborted (6)
[fv-az1109-238:41571] Signal code:  (-6)
[fv-az1109-238:41571] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f977d042520]
[fv-az1109-238:41571] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f977d0969fc]
[fv-az1109-238:41571] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f977d042476]
[fv-az1109-238:41571] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f977d0287f3]
[fv-az1109-238:41571] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f977d4a2b9e]
[fv-az1109-238:41571] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f977d4ae20c]
[fv-az1109-238:41571] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f977d4ae277]
[fv-az1109-238:41571] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f977d4ae52b]
[fv-az1109-238:41571] [ 8] plumed(+0x12f48)[0x558fad9a8f48]
[fv-az1109-238:41571] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f977d029d90]
[fv-az1109-238:41571] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f977d029e40]
[fv-az1109-238:41571] [11] plumed(+0x131e5)[0x558fad9a91e5]
[fv-az1109-238:41571] *** End of error message ***
</pre>
{% endraw %}
