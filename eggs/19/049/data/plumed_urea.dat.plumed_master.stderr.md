**Project ID:** [plumID:19.049]({{ '/' | absolute_url }}eggs/19/049/)  
Stderr for source:  plumed_urea.dat   
Download: [zipped raw stdout](plumed_urea.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_urea.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CONTACT_MATRIX with label @s41 : missing SWITCH11 keyword
[fv-az1947-39:14213] *** Process received signal ***
[fv-az1947-39:14213] Signal: Aborted (6)
[fv-az1947-39:14213] Signal code:  (-6)
[fv-az1947-39:14213] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2a31a45330]
[fv-az1947-39:14213] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2a31a9eb2c]
[fv-az1947-39:14213] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2a31a4527e]
[fv-az1947-39:14213] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2a31a288ff]
[fv-az1947-39:14213] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2a31ea5ff5]
[fv-az1947-39:14213] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2a31ebb0da]
[fv-az1947-39:14213] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2a31ea5a55]
[fv-az1947-39:14213] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2a31ea5a6f]
[fv-az1947-39:14213] [ 8] plumed_master(+0x146dd)[0x56357c8496dd]
[fv-az1947-39:14213] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2a31a2a1ca]
[fv-az1947-39:14213] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2a31a2a28b]
[fv-az1947-39:14213] [11] plumed_master(+0x15365)[0x56357c84a365]
[fv-az1947-39:14213] *** End of error message ***
</pre>
{% endraw %}
