**Project ID:** [plumID:20.028]({{ '/' | absolute_url }}eggs/20/028/)  
Stderr for source:  oncogenic/plumed-1.dat   
Download: [zipped raw stdout](plumed-1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Tools.h:151) static void PLMD::Tools::convert(const T&, U&) [with T = std::__cxx11::basic_string<char>; U = double]
+++ assertion failed: convertNoexcept(t,u)
Error converting  483  97.1
[fv-az1445-962:74377] *** Process received signal ***
[fv-az1445-962:74377] Signal: Aborted (6)
[fv-az1445-962:74377] Signal code:  (-6)
[fv-az1445-962:74377] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbad2042520]
[fv-az1445-962:74377] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbad20969fc]
[fv-az1445-962:74377] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbad2042476]
[fv-az1445-962:74377] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbad20287f3]
[fv-az1445-962:74377] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbad24a2b9e]
[fv-az1445-962:74377] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbad24ae20c]
[fv-az1445-962:74377] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbad24ae277]
[fv-az1445-962:74377] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbad24ae52b]
[fv-az1445-962:74377] [ 8] plumed_master(+0x14274)[0x557cbeb96274]
[fv-az1445-962:74377] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbad2029d90]
[fv-az1445-962:74377] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbad2029e40]
[fv-az1445-962:74377] [11] plumed_master(+0x14ed5)[0x557cbeb96ed5]
[fv-az1445-962:74377] *** End of error message ***
</pre>
{% endraw %}
