**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-3/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONCV LABEL=cv1 ATOMS=1,4 IMPORT=distcv FUNCTION=cv
Maybe a missing space or a typo?
[fv-az659-178:71614] *** Process received signal ***
[fv-az659-178:71614] Signal: Aborted (6)
[fv-az659-178:71614] Signal code:  (-6)
[fv-az659-178:71614] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc27c842520]
[fv-az659-178:71614] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc27c8969fc]
[fv-az659-178:71614] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc27c842476]
[fv-az659-178:71614] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc27c8287f3]
[fv-az659-178:71614] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc27cca2b9e]
[fv-az659-178:71614] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc27ccae20c]
[fv-az659-178:71614] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc27ccae277]
[fv-az659-178:71614] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc27ccae52b]
[fv-az659-178:71614] [ 8] plumed(+0x12f48)[0x55b4c3bd4f48]
[fv-az659-178:71614] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc27c829d90]
[fv-az659-178:71614] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc27c829e40]
[fv-az659-178:71614] [11] plumed(+0x131e5)[0x55b4c3bd51e5]
[fv-az659-178:71614] *** End of error message ***
</pre>
{% endraw %}
