**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_map_to_reference_map.dat   
Download: [zipped raw stdout](plumed_map_to_reference_map.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_map_to_reference_map.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: SKETCHMAP_PROJECTION LABEL=smap ARG=d1,d2,d3,d4,d5,d6,d7,d8,d9,d10,d11,d12,d13,d14,d15,d16,d17,d18,d19,d20,d21,d22,d23,d24,d25,d26,d27,d28,d29,d30,d31,d32,d33,d34,d35,d36,d37,d38,d39,d40,d41,d42,d43,d44,d45,d46,d47,d48,d49,d50,d51 REFERENCE=ref_data.pdb PROPERTY=smap_coord-1,smap_coord-2 WEIGHT=lwe HIGH_DIM_FUNCTION=SMAP R_0=1.5 A=2 B=2 LOW_DIM_FUNCTION=SMAP R_0=1.5 A=2 B=2 CGTOL=1E-3
Maybe a missing space or a typo?
[fv-az736-136:04592] *** Process received signal ***
[fv-az736-136:04592] Signal: Aborted (6)
[fv-az736-136:04592] Signal code:  (-6)
[fv-az736-136:04592] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7165642520]
[fv-az736-136:04592] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f71656969fc]
[fv-az736-136:04592] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7165642476]
[fv-az736-136:04592] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f71656287f3]
[fv-az736-136:04592] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7165aa4f26]
[fv-az736-136:04592] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7165ab6d9c]
[fv-az736-136:04592] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7165ab6e07]
[fv-az736-136:04592] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7165ab70bb]
[fv-az736-136:04592] [ 8] plumed_master(+0x12ebf)[0x56465ed28ebf]
[fv-az736-136:04592] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7165629d90]
[fv-az736-136:04592] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7165629e40]
[fv-az736-136:04592] [11] plumed_master(+0x13155)[0x56465ed29155]
[fv-az736-136:04592] *** End of error message ***
</pre>
{% endraw %}
