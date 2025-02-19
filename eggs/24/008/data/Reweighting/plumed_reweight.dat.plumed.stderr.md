**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1945-156:06782] *** Process received signal ***
[fv-az1945-156:06782] Signal: Aborted (6)
[fv-az1945-156:06782] Signal code:  (-6)
[fv-az1945-156:06782] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fac9e245330]
[fv-az1945-156:06782] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fac9e29eb2c]
[fv-az1945-156:06782] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fac9e24527e]
[fv-az1945-156:06782] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fac9e2288ff]
[fv-az1945-156:06782] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fac9e6a5ff5]
[fv-az1945-156:06782] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fac9e6bb0da]
[fv-az1945-156:06782] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fac9e6a5a55]
[fv-az1945-156:06782] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fac9e6a5a6f]
[fv-az1945-156:06782] [ 8] plumed(+0x146dd)[0x558f9b7c76dd]
[fv-az1945-156:06782] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fac9e22a1ca]
[fv-az1945-156:06782] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fac9e22a28b]
[fv-az1945-156:06782] [11] plumed(+0x15365)[0x558f9b7c8365]
[fv-az1945-156:06782] *** End of error message ***
</pre>
{% endraw %}
