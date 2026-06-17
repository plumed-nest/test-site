**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  wild-type/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:151) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  461  97.1
[runnervm1li68:09970] *** Process received signal ***
[runnervm1li68:09970] Signal: Aborted (6)
[runnervm1li68:09970] Signal code:  (-6)
[runnervm1li68:09970] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdfe4e45330]
[runnervm1li68:09970] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdfe4e9eb2c]
[runnervm1li68:09970] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdfe4e4527e]
[runnervm1li68:09970] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdfe4e288ff]
[runnervm1li68:09970] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdfe52a5ff5]
[runnervm1li68:09970] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdfe52bb0da]
[runnervm1li68:09970] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdfe52a5a55]
[runnervm1li68:09970] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdfe52a5a6f]
[runnervm1li68:09970] [ 8] plumed(+0x146dd)[0x5615ca9ab6dd]
[runnervm1li68:09970] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdfe4e2a1ca]
[runnervm1li68:09970] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdfe4e2a28b]
[runnervm1li68:09970] [11] plumed(+0x15365)[0x5615ca9ac365]
[runnervm1li68:09970] *** End of error message ***
</pre>
{% endraw %}
