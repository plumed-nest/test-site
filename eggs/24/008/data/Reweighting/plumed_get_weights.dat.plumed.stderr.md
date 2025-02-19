**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_get_weights.dat   
Download: [zipped raw stdout](plumed_get_weights.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_get_weights.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[fv-az1945-156:06729] *** Process received signal ***
[fv-az1945-156:06729] Signal: Aborted (6)
[fv-az1945-156:06729] Signal code:  (-6)
[fv-az1945-156:06729] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9ecaa45330]
[fv-az1945-156:06729] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9ecaa9eb2c]
[fv-az1945-156:06729] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9ecaa4527e]
[fv-az1945-156:06729] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9ecaa288ff]
[fv-az1945-156:06729] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9ecaea5ff5]
[fv-az1945-156:06729] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9ecaebb0da]
[fv-az1945-156:06729] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9ecaea5a55]
[fv-az1945-156:06729] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9ecaea5a6f]
[fv-az1945-156:06729] [ 8] plumed(+0x146dd)[0x557c370146dd]
[fv-az1945-156:06729] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9ecaa2a1ca]
[fv-az1945-156:06729] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9ecaa2a28b]
[fv-az1945-156:06729] [11] plumed(+0x15365)[0x557c37015365]
[fv-az1945-156:06729] *** End of error message ***
</pre>
{% endraw %}
