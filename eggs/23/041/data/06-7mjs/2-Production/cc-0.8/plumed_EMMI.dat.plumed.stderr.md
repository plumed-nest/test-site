**Project ID:** [plumID:23.041]({{ '/' | absolute_url }}eggs/23/041/)  
Stderr for source:  06-7mjs/2-Production/cc-0.8/plumed_EMMI.dat   
Download: [zipped raw stdout](plumed_EMMI.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_EMMI.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: EMMIVOX LABEL=emmi TEMP=300.0 NL_STRIDE=50 NL_DIST_CUTOFF=1.0 NL_GAUSS_CUTOFF=3.0 ATOMS=system-map DATA_FILE=emd_plumed_aligned.dat NORM_DENSITY=13433.030273 RESOLUTION=0.303 SIGMA_MIN=0.2 GPU STATUS_FILE=EMMIStatus WRITE_STRIDE=5000 DBFACT=0.05 MCBFACT_STRIDE=500 BFACT_SIGMA=0.1 SCALE=1.400000 CORRELATION
Maybe a missing space or a typo?
[fv-az695-456:69996] *** Process received signal ***
[fv-az695-456:69996] Signal: Aborted (6)
[fv-az695-456:69996] Signal code:  (-6)
[fv-az695-456:69996] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7eff62042520]
[fv-az695-456:69996] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7eff620969fc]
[fv-az695-456:69996] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7eff62042476]
[fv-az695-456:69996] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7eff620287f3]
[fv-az695-456:69996] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7eff624a2b9e]
[fv-az695-456:69996] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7eff624ae20c]
[fv-az695-456:69996] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7eff624ae277]
[fv-az695-456:69996] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7eff624ae52b]
[fv-az695-456:69996] [ 8] plumed(+0x12f48)[0x559ff6556f48]
[fv-az695-456:69996] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7eff62029d90]
[fv-az695-456:69996] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7eff62029e40]
[fv-az695-456:69996] [11] plumed(+0x131e5)[0x559ff65571e5]
[fv-az695-456:69996] *** End of error message ***
</pre>
{% endraw %}