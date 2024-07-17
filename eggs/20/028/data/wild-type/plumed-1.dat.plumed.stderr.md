**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  wild-type/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:137) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  461  97.1
[fv-az1445-962:74338] *** Process received signal ***
[fv-az1445-962:74338] Signal: Aborted (6)
[fv-az1445-962:74338] Signal code:  (-6)
[fv-az1445-962:74338] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7bc1442520]
[fv-az1445-962:74338] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7bc14969fc]
[fv-az1445-962:74338] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7bc1442476]
[fv-az1445-962:74338] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7bc14287f3]
[fv-az1445-962:74338] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7bc18a2b9e]
[fv-az1445-962:74338] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7bc18ae20c]
[fv-az1445-962:74338] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7bc18ae277]
[fv-az1445-962:74338] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7bc18ae52b]
[fv-az1445-962:74338] [ 8] plumed(+0x12f48)[0x55afe0574f48]
[fv-az1445-962:74338] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7bc1429d90]
[fv-az1445-962:74338] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7bc1429e40]
[fv-az1445-962:74338] [11] plumed(+0x131e5)[0x55afe05751e5]
[fv-az1445-962:74338] *** End of error message ***
</pre>
{% endraw %}
