**Project ID:** [plumID:21.020]({{ '/' | absolute_url }}eggs/21/020/)  
Stderr for source:  hbr/fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @52 : keyword ARG is compulsory for this action
[fv-az1770-999:07734] *** Process received signal ***
[fv-az1770-999:07734] Signal: Aborted (6)
[fv-az1770-999:07734] Signal code:  (-6)
[fv-az1770-999:07734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa794c45330]
[fv-az1770-999:07734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa794c9eb2c]
[fv-az1770-999:07734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa794c4527e]
[fv-az1770-999:07734] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa794c288ff]
[fv-az1770-999:07734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa7950a5ff5]
[fv-az1770-999:07734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa7950bb0da]
[fv-az1770-999:07734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa7950a5a55]
[fv-az1770-999:07734] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa7950a5a6f]
[fv-az1770-999:07734] [ 8] plumed_master(+0x146dd)[0x5631d7d576dd]
[fv-az1770-999:07734] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa794c2a1ca]
[fv-az1770-999:07734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa794c2a28b]
[fv-az1770-999:07734] [11] plumed_master(+0x15365)[0x5631d7d58365]
[fv-az1770-999:07734] *** End of error message ***
</pre>
{% endraw %}
