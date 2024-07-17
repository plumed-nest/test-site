**Project ID:** [plumID:23.043]({{ '/' | absolute_url }}eggs/23/043/)  
Stderr for source:  metad-example/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SPHERICAL_EXPANSION LABEL=SPEX_A SPECIES1=1-216 SPECIES2=217-432 SPECIES3=433-1080 HYPERPARAMS=     "max_radial": 6,     "max_angular": 1,     "compute_gradients": false,     "cutoff_function": {"type": "ShiftedCosine", "cutoff": {"value": 3.0, "unit": "AA"}, "smooth_width": {"value": 0.5, "unit": "AA"}},     "gaussian_density": {"type": "Constant", "gaussian_sigma": {"value": 0.5, "unit": "AA"}},     "radial_contribution": {"type": "GTO"}
Maybe a missing space or a typo?
[fv-az774-16:69541] *** Process received signal ***
[fv-az774-16:69541] Signal: Aborted (6)
[fv-az774-16:69541] Signal code:  (-6)
[fv-az774-16:69541] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3568642520]
[fv-az774-16:69541] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f35686969fc]
[fv-az774-16:69541] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3568642476]
[fv-az774-16:69541] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f35686287f3]
[fv-az774-16:69541] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3568aa2b9e]
[fv-az774-16:69541] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3568aae20c]
[fv-az774-16:69541] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3568aae277]
[fv-az774-16:69541] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3568aae52b]
[fv-az774-16:69541] [ 8] plumed(+0x12f48)[0x559d3d3acf48]
[fv-az774-16:69541] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3568629d90]
[fv-az774-16:69541] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3568629e40]
[fv-az774-16:69541] [11] plumed(+0x131e5)[0x559d3d3ad1e5]
[fv-az774-16:69541] *** End of error message ***
</pre>
{% endraw %}
