**Project ID:** [plumID:24.006]({{ '/' | absolute_url }}eggs/24/006/)  
Stderr for source:  clusterFormationFreeEnergy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action CLUSTER_PROPERTIES with label @s22 : keyword ARG is compulsory for this action
[fv-az1945-156:06914] *** Process received signal ***
[fv-az1945-156:06914] Signal: Aborted (6)
[fv-az1945-156:06914] Signal code:  (-6)
[fv-az1945-156:06914] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f46de445330]
[fv-az1945-156:06914] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f46de49eb2c]
[fv-az1945-156:06914] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f46de44527e]
[fv-az1945-156:06914] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f46de4288ff]
[fv-az1945-156:06914] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f46de8a5ff5]
[fv-az1945-156:06914] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f46de8bb0da]
[fv-az1945-156:06914] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f46de8a5a55]
[fv-az1945-156:06914] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f46de8a5a6f]
[fv-az1945-156:06914] [ 8] plumed(+0x146dd)[0x5615a305b6dd]
[fv-az1945-156:06914] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f46de42a1ca]
[fv-az1945-156:06914] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f46de42a28b]
[fv-az1945-156:06914] [11] plumed(+0x15365)[0x5615a305c365]
[fv-az1945-156:06914] *** End of error message ***
</pre>
{% endraw %}
