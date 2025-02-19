**Project ID:** [plumID:21.001]({{ '/' | absolute_url }}eggs/21/001/)  
Stderr for source:  HS6ST/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @48 : keyword ARG is compulsory for this action
[fv-az1436-30:10675] *** Process received signal ***
[fv-az1436-30:10675] Signal: Aborted (6)
[fv-az1436-30:10675] Signal code:  (-6)
[fv-az1436-30:10675] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe84f045330]
[fv-az1436-30:10675] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe84f09eb2c]
[fv-az1436-30:10675] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe84f04527e]
[fv-az1436-30:10675] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe84f0288ff]
[fv-az1436-30:10675] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe84f4a5ff5]
[fv-az1436-30:10675] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe84f4bb0da]
[fv-az1436-30:10675] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe84f4a5a55]
[fv-az1436-30:10675] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe84f4a5a6f]
[fv-az1436-30:10675] [ 8] plumed_master(+0x146dd)[0x5629d87006dd]
[fv-az1436-30:10675] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe84f02a1ca]
[fv-az1436-30:10675] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe84f02a28b]
[fv-az1436-30:10675] [11] plumed_master(+0x15365)[0x5629d8701365]
[fv-az1436-30:10675] *** End of error message ***
</pre>
{% endraw %}
