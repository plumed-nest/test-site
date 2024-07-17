**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_sketchmap.dat   
Download: [zipped raw stdout](plumed_sketchmap.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_sketchmap.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: VSTACK LABEL=mat ARG1=a.d1 ARG2=a.d2 ARG3=a.d3 ARG4=a.d4 ARG5=a.d5 ARG6=a.d6 ARG7=a.d7 ARG8=a.d8 ARG9=a.d9 ARG10=a.d10 ARG11=a.d11 ARG12=a.d12 ARG13=a.d13 ARG14=a.d14 ARG15=a.d15 ARG16=a.d16 ARG17=a.d17 ARG18=a.d18 ARG19=a.d19 ARG20=a.d20 ARG21=a.d21 ARG22=a.d22 ARG23=a.d23 ARG24=a.d24 ARG25=a.d25 ARG26=a.d26 ARG27=a.d27 ARG28=a.d28 ARG29=a.d29 ARG30=a.d30 ARG31=a.d31 ARG32=a.d32 ARG33=a.d33 ARG34=a.d34 ARG35=a.d35 ARG36=a.d36 ARG37=a.d37 ARG38=a.d38 ARG39=a.d39 ARG40=a.d40 ARG41=a.d41 ARG42=a.d42 ARG43=a.d43 ARG44=a.d44 ARG45=a.d45 ARG46=a.d46 ARG47=a.d47 ARG48=a.d48 ARG49=a.d49 ARG50=a.d50 ARG51=a.d51
Maybe a missing space or a typo?
[fv-az975-63:70187] *** Process received signal ***
[fv-az975-63:70187] Signal: Aborted (6)
[fv-az975-63:70187] Signal code:  (-6)
[fv-az975-63:70187] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f48bde42520]
[fv-az975-63:70187] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f48bde969fc]
[fv-az975-63:70187] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f48bde42476]
[fv-az975-63:70187] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f48bde287f3]
[fv-az975-63:70187] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f48be2a2b9e]
[fv-az975-63:70187] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f48be2ae20c]
[fv-az975-63:70187] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f48be2ae277]
[fv-az975-63:70187] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f48be2ae52b]
[fv-az975-63:70187] [ 8] plumed(+0x12f48)[0x55c4a0fc0f48]
[fv-az975-63:70187] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f48bde29d90]
[fv-az975-63:70187] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f48bde29e40]
[fv-az975-63:70187] [11] plumed(+0x131e5)[0x55c4a0fc11e5]
[fv-az975-63:70187] *** End of error message ***
</pre>
{% endraw %}
