**Project ID:** [plumID:24.016]({{ '/' | absolute_url }}eggs/24/016/)  
Stderr for source:  3-ensemble-refinement/plumed_EMMI_norst.dat   
Download: [zipped raw stdout](plumed_EMMI_norst.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI_norst.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: EMMIVOX LABEL=emmi TEMP=300.0 NL_STRIDE=50 NL_DIST_CUTOFF=1.0 NL_GAUSS_CUTOFF=3.0 ATOMS=system-map DATA_FILE=../2-ss-refinement/emd_plumed_aligned.dat NORM_DENSITY=6846.255371 RESOLUTION=0.36 SIGMA_MIN=0.2 GPU STATUS_FILE=EMMIStatus WRITE_STRIDE=5000 BFACT_READ SCALE=1.250000 CORRELATION
Maybe a missing space or a typo?
[fv-az774-16:69436] *** Process received signal ***
[fv-az774-16:69436] Signal: Aborted (6)
[fv-az774-16:69436] Signal code:  (-6)
[fv-az774-16:69436] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7961642520]
[fv-az774-16:69436] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f79616969fc]
[fv-az774-16:69436] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7961642476]
[fv-az774-16:69436] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f79616287f3]
[fv-az774-16:69436] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7961aa2b9e]
[fv-az774-16:69436] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7961aae20c]
[fv-az774-16:69436] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7961aae277]
[fv-az774-16:69436] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7961aae52b]
[fv-az774-16:69436] [ 8] plumed(+0x12f48)[0x55f9c8a7ff48]
[fv-az774-16:69436] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7961629d90]
[fv-az774-16:69436] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7961629e40]
[fv-az774-16:69436] [11] plumed(+0x131e5)[0x55f9c8a801e5]
[fv-az774-16:69436] *** End of error message ***
</pre>
{% endraw %}
