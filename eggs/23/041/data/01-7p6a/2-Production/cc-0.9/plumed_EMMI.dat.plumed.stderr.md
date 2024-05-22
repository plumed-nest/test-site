**Project ID:** [plumID:23.041]({{ '/' | absolute_url }}eggs/23/041/)  
Stderr for source:  01-7p6a/2-Production/cc-0.9/plumed_EMMI.dat   
Download: [zipped raw stdout](plumed_EMMI.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: EMMIVOX LABEL=emmi TEMP=300.0 NL_STRIDE=50 NL_DIST_CUTOFF=1.0 NL_GAUSS_CUTOFF=3.0 ATOMS=system-map DATA_FILE=emd_plumed_aligned.dat NORM_DENSITY=687.556335 RESOLUTION=0.19 SIGMA_MIN=0.2 GPU STATUS_FILE=EMMIStatus WRITE_STRIDE=5000 BFACT_NOCHAIN DBFACT=0.05 MCBFACT_STRIDE=500 BFACT_SIGMA=0.1 SCALE=1.400000 CORRELATION
Maybe a missing space or a typo?
[fv-az1113-981:39729] *** Process received signal ***
[fv-az1113-981:39729] Signal: Aborted (6)
[fv-az1113-981:39729] Signal code:  (-6)
[fv-az1113-981:39729] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa476842520]
[fv-az1113-981:39729] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa4768969fc]
[fv-az1113-981:39729] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa476842476]
[fv-az1113-981:39729] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa4768287f3]
[fv-az1113-981:39729] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa476ca2b9e]
[fv-az1113-981:39729] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa476cae20c]
[fv-az1113-981:39729] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa476cae277]
[fv-az1113-981:39729] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa476cae52b]
[fv-az1113-981:39729] [ 8] plumed(+0x12f48)[0x558414d84f48]
[fv-az1113-981:39729] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa476829d90]
[fv-az1113-981:39729] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa476829e40]
[fv-az1113-981:39729] [11] plumed(+0x131e5)[0x558414d851e5]
[fv-az1113-981:39729] *** End of error message ***
</pre>
{% endraw %}
