**Project ID:** [plumID:19.075]({{ '/' | absolute_url }}eggs/19/075/)  
Stderr for source:  regtest/pycv/rt-f1/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PYTHONFUNCTION LABEL=dAB2 ARG=dAB IMPORT=pythonfunction FUNCTION=square PERIODIC=NO
Maybe a missing space or a typo?
[fv-az659-178:71645] *** Process received signal ***
[fv-az659-178:71645] Signal: Aborted (6)
[fv-az659-178:71645] Signal code:  (-6)
[fv-az659-178:71645] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f32b2642520]
[fv-az659-178:71645] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f32b26969fc]
[fv-az659-178:71645] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f32b2642476]
[fv-az659-178:71645] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f32b26287f3]
[fv-az659-178:71645] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f32b2aa2b9e]
[fv-az659-178:71645] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f32b2aae20c]
[fv-az659-178:71645] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f32b2aae277]
[fv-az659-178:71645] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f32b2aae52b]
[fv-az659-178:71645] [ 8] plumed(+0x12f48)[0x561ef34caf48]
[fv-az659-178:71645] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f32b2629d90]
[fv-az659-178:71645] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f32b2629e40]
[fv-az659-178:71645] [11] plumed(+0x131e5)[0x561ef34cb1e5]
[fv-az659-178:71645] *** End of error message ***
</pre>
{% endraw %}
