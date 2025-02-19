**Project ID:** [plumID:21.016]({{ '/' | absolute_url }}eggs/21/016/)  
Stderr for source:  input_files/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label saxs : cannot understand the following words from the input line : SCALEINT=1
[fv-az1770-999:07948] *** Process received signal ***
[fv-az1770-999:07948] Signal: Aborted (6)
[fv-az1770-999:07948] Signal code:  (-6)
[fv-az1770-999:07948] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f15be445330]
[fv-az1770-999:07948] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f15be49eb2c]
[fv-az1770-999:07948] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f15be44527e]
[fv-az1770-999:07948] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f15be4288ff]
[fv-az1770-999:07948] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f15be8a5ff5]
[fv-az1770-999:07948] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f15be8bb0da]
[fv-az1770-999:07948] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f15be8a5a55]
[fv-az1770-999:07948] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f15be8a5a6f]
[fv-az1770-999:07948] [ 8] plumed(+0x146dd)[0x5641747556dd]
[fv-az1770-999:07948] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f15be42a1ca]
[fv-az1770-999:07948] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f15be42a28b]
[fv-az1770-999:07948] [11] plumed(+0x15365)[0x564174756365]
[fv-az1770-999:07948] *** End of error message ***
</pre>
{% endraw %}
