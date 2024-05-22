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
[fv-az2031-223:39077] *** Process received signal ***
[fv-az2031-223:39077] Signal: Aborted (6)
[fv-az2031-223:39077] Signal code:  (-6)
[fv-az2031-223:39077] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f906a642520]
[fv-az2031-223:39077] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f906a6969fc]
[fv-az2031-223:39077] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f906a642476]
[fv-az2031-223:39077] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f906a6287f3]
[fv-az2031-223:39077] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f906aaa2b9e]
[fv-az2031-223:39077] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f906aaae20c]
[fv-az2031-223:39077] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f906aaae277]
[fv-az2031-223:39077] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f906aaae52b]
[fv-az2031-223:39077] [ 8] plumed(+0x12f48)[0x5616f504ef48]
[fv-az2031-223:39077] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f906a629d90]
[fv-az2031-223:39077] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f906a629e40]
[fv-az2031-223:39077] [11] plumed(+0x131e5)[0x5616f504f1e5]
[fv-az2031-223:39077] *** End of error message ***
</pre>
{% endraw %}
