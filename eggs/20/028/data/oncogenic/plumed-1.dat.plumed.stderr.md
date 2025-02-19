**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  oncogenic/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:151) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  483  97.1
[fv-az1326-415:12473] *** Process received signal ***
[fv-az1326-415:12473] Signal: Aborted (6)
[fv-az1326-415:12473] Signal code:  (-6)
[fv-az1326-415:12473] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f172b045330]
[fv-az1326-415:12473] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f172b09eb2c]
[fv-az1326-415:12473] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f172b04527e]
[fv-az1326-415:12473] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f172b0288ff]
[fv-az1326-415:12473] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f172b4a5ff5]
[fv-az1326-415:12473] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f172b4bb0da]
[fv-az1326-415:12473] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f172b4a5a55]
[fv-az1326-415:12473] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f172b4a5a6f]
[fv-az1326-415:12473] [ 8] plumed(+0x146dd)[0x55ad0dcdc6dd]
[fv-az1326-415:12473] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f172b02a1ca]
[fv-az1326-415:12473] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f172b02a28b]
[fv-az1326-415:12473] [11] plumed(+0x15365)[0x55ad0dcdd365]
[fv-az1326-415:12473] *** End of error message ***
</pre>
{% endraw %}
