**Project ID:** [plumID:23.041]({{ '/' | absolute_url }}eggs/23/041/)  
Stderr for source:  01-7p6a/2-Production/cc-0.7/plumed_EMMI.dat   
Download: [zipped raw stdout](plumed_EMMI.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: EMMIVOX LABEL=emmi TEMP=300.0 NL_STRIDE=50 NL_DIST_CUTOFF=1.0 NL_GAUSS_CUTOFF=3.0 ATOMS=system-map DATA_FILE=emd_plumed_aligned.dat NORM_DENSITY=687.556335 RESOLUTION=0.19 SIGMA_MIN=0.2 GPU STATUS_FILE=EMMIStatus WRITE_STRIDE=5000 BFACT_NOCHAIN DBFACT=0.05 MCBFACT_STRIDE=500 BFACT_SIGMA=0.1 SCALE=1.400000 CORRELATION
Maybe a missing space or a typo?
[fv-az532-512:04858] *** Process received signal ***
[fv-az532-512:04858] Signal: Aborted (6)
[fv-az532-512:04858] Signal code:  (-6)
[fv-az532-512:04858] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7e16442520]
[fv-az532-512:04858] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7e164969fc]
[fv-az532-512:04858] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7e16442476]
[fv-az532-512:04858] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7e164287f3]
[fv-az532-512:04858] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f7e168a4f26]
[fv-az532-512:04858] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f7e168b6d9c]
[fv-az532-512:04858] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f7e168b6e07]
[fv-az532-512:04858] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7e168b70bb]
[fv-az532-512:04858] [ 8] plumed(+0x12f48)[0x55ba787f8f48]
[fv-az532-512:04858] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7e16429d90]
[fv-az532-512:04858] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7e16429e40]
[fv-az532-512:04858] [11] plumed(+0x131e5)[0x55ba787f91e5]
[fv-az532-512:04858] *** End of error message ***
</pre>
{% endraw %}
