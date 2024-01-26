**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: SPHERICAL_EXPANSION LABEL=SPEX_A SPECIES1=1-216 SPECIES2=217-432 SPECIES3=433-1080 HYPERPARAMS=     "max_radial": 6,     "max_angular": 1,     "compute_gradients": false,     "cutoff_function": {"type": "ShiftedCosine", "cutoff": {"value": 3.0, "unit": "AA"}, "smooth_width": {"value": 0.5, "unit": "AA"}},     "gaussian_density": {"type": "Constant", "gaussian_sigma": {"value": 0.5, "unit": "AA"}},     "radial_contribution": {"type": "GTO"}
Maybe a missing space or a typo?
[fv-az529-343:04275] *** Process received signal ***
[fv-az529-343:04275] Signal: Aborted (6)
[fv-az529-343:04275] Signal code:  (-6)
[fv-az529-343:04275] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff2f8a42520]
[fv-az529-343:04275] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff2f8a969fc]
[fv-az529-343:04275] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff2f8a42476]
[fv-az529-343:04275] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff2f8a287f3]
[fv-az529-343:04275] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7ff2f8ea4f26]
[fv-az529-343:04275] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7ff2f8eb6d9c]
[fv-az529-343:04275] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7ff2f8eb6e07]
[fv-az529-343:04275] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff2f8eb70bb]
[fv-az529-343:04275] [ 8] plumed_master(+0x12ebf)[0x55aff51a8ebf]
[fv-az529-343:04275] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff2f8a29d90]
[fv-az529-343:04275] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff2f8a29e40]
[fv-az529-343:04275] [11] plumed_master(+0x13155)[0x55aff51a9155]
[fv-az529-343:04275] *** End of error message ***
</pre>
{% endraw %}
