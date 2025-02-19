**Project ID:** [plumID:24.006]({{ '/' | absolute_url }}eggs/24/006/)  
Stderr for source:  clusterFormationFreeEnergy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DFSCLUSTERING with label dfs : keyword ARG is compulsory for this action
[fv-az1945-156:06930] *** Process received signal ***
[fv-az1945-156:06930] Signal: Aborted (6)
[fv-az1945-156:06930] Signal code:  (-6)
[fv-az1945-156:06930] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbb06c45330]
[fv-az1945-156:06930] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbb06c9eb2c]
[fv-az1945-156:06930] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbb06c4527e]
[fv-az1945-156:06930] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbb06c288ff]
[fv-az1945-156:06930] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbb070a5ff5]
[fv-az1945-156:06930] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbb070bb0da]
[fv-az1945-156:06930] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbb070a5a55]
[fv-az1945-156:06930] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbb070a5a6f]
[fv-az1945-156:06930] [ 8] plumed_master(+0x146dd)[0x55d3f60406dd]
[fv-az1945-156:06930] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbb06c2a1ca]
[fv-az1945-156:06930] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbb06c2a28b]
[fv-az1945-156:06930] [11] plumed_master(+0x15365)[0x55d3f6041365]
[fv-az1945-156:06930] *** End of error message ***
</pre>
{% endraw %}
