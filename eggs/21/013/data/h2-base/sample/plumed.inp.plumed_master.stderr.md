**Project ID:** [plumID:21.013]({{ '/' | absolute_url }}eggs/21/013/)  
Stderr for source:  h2-base/sample/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @29 : keyword ARG is compulsory for this action
[fv-az1947-39:12255] *** Process received signal ***
[fv-az1947-39:12255] Signal: Aborted (6)
[fv-az1947-39:12255] Signal code:  (-6)
[fv-az1947-39:12255] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1650445330]
[fv-az1947-39:12255] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f165049eb2c]
[fv-az1947-39:12255] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f165044527e]
[fv-az1947-39:12255] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f16504288ff]
[fv-az1947-39:12255] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f16508a5ff5]
[fv-az1947-39:12255] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f16508bb0da]
[fv-az1947-39:12255] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f16508a5a55]
[fv-az1947-39:12255] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f16508a5a6f]
[fv-az1947-39:12255] [ 8] plumed_master(+0x146dd)[0x5561de1f96dd]
[fv-az1947-39:12255] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f165042a1ca]
[fv-az1947-39:12255] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f165042a28b]
[fv-az1947-39:12255] [11] plumed_master(+0x15365)[0x5561de1fa365]
[fv-az1947-39:12255] *** End of error message ***
</pre>
{% endraw %}
