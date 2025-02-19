**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  hbr/ves/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @52 : keyword ARG is compulsory for this action
[fv-az1770-999:07866] *** Process received signal ***
[fv-az1770-999:07866] Signal: Aborted (6)
[fv-az1770-999:07866] Signal code:  (-6)
[fv-az1770-999:07866] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f99a5a45330]
[fv-az1770-999:07866] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f99a5a9eb2c]
[fv-az1770-999:07866] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f99a5a4527e]
[fv-az1770-999:07866] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f99a5a288ff]
[fv-az1770-999:07866] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f99a5ea5ff5]
[fv-az1770-999:07866] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f99a5ebb0da]
[fv-az1770-999:07866] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f99a5ea5a55]
[fv-az1770-999:07866] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f99a5ea5a6f]
[fv-az1770-999:07866] [ 8] plumed_master(+0x146dd)[0x561e0c2546dd]
[fv-az1770-999:07866] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f99a5a2a1ca]
[fv-az1770-999:07866] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f99a5a2a28b]
[fv-az1770-999:07866] [11] plumed_master(+0x15365)[0x561e0c255365]
[fv-az1770-999:07866] *** End of error message ***
</pre>
{% endraw %}
