**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_map_to_reference_map.dat   
Download: [zipped raw stdout](plumed_map_to_reference_map.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_map_to_reference_map.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SKETCHMAP_PROJECTION LABEL=smap ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29,d30,d31,d32,d33,d34,d35,d36,d37,d38,d39,d40,d41,d42,d43,d44,d45,d46,d47,d48,d49,d50,d51 REFERENCE=ref_data.pdb PROPERTY=smap_coord-1,smap_coord-2 WEIGHT=lwe HIGH_DIM_FUNCTION=SMAP R_0=1.5 A=2 B=2 LOW_DIM_FUNCTION=SMAP R_0=1.5 A=2 B=2 CGTOL=1E-3
Maybe a missing space or a typo?
[fv-az1106-239:39612] *** Process received signal ***
[fv-az1106-239:39612] Signal: Aborted (6)
[fv-az1106-239:39612] Signal code:  (-6)
[fv-az1106-239:39612] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f29b0642520]
[fv-az1106-239:39612] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f29b06969fc]
[fv-az1106-239:39612] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f29b0642476]
[fv-az1106-239:39612] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f29b06287f3]
[fv-az1106-239:39612] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f29b0aa2b9e]
[fv-az1106-239:39612] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f29b0aae20c]
[fv-az1106-239:39612] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f29b0aae277]
[fv-az1106-239:39612] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f29b0aae52b]
[fv-az1106-239:39612] [ 8] plumed(+0x12f48)[0x55e7f2782f48]
[fv-az1106-239:39612] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f29b0629d90]
[fv-az1106-239:39612] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f29b0629e40]
[fv-az1106-239:39612] [11] plumed(+0x131e5)[0x55e7f27831e5]
[fv-az1106-239:39612] *** End of error message ***
</pre>
{% endraw %}
