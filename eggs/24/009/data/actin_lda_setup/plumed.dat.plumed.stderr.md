**Project ID:** [plumID:24.009]({{ '/' | absolute_url }}eggs/24/009/)  
Stderr for source:  actin_lda_setup/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: LDA_PROJ LABEL=ld1 REFERENCE=global_avg.txt PRECISION=global_prec.txt VECTOR=ld1_scalings.txt GROUP=ga_list
Maybe a missing space or a typo?
[fv-az1445-962:69401] *** Process received signal ***
[fv-az1445-962:69401] Signal: Aborted (6)
[fv-az1445-962:69401] Signal code:  (-6)
[fv-az1445-962:69401] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2eff842520]
[fv-az1445-962:69401] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2eff8969fc]
[fv-az1445-962:69401] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2eff842476]
[fv-az1445-962:69401] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2eff8287f3]
[fv-az1445-962:69401] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2effca2b9e]
[fv-az1445-962:69401] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2effcae20c]
[fv-az1445-962:69401] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2effcae277]
[fv-az1445-962:69401] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2effcae52b]
[fv-az1445-962:69401] [ 8] plumed(+0x12f48)[0x564f20842f48]
[fv-az1445-962:69401] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2eff829d90]
[fv-az1445-962:69401] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2eff829e40]
[fv-az1445-962:69401] [11] plumed(+0x131e5)[0x564f208431e5]
[fv-az1445-962:69401] *** End of error message ***
</pre>
{% endraw %}
