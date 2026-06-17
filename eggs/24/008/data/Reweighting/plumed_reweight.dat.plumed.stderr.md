**Project ID:** [plumID:24.008]({{ '/' | absolute_url }}eggs/24/008/)  
Stderr for source:  Reweighting/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label rho : could not find file named rtp_coord.dat
[runnervm1li68:06003] *** Process received signal ***
[runnervm1li68:06003] Signal: Aborted (6)
[runnervm1li68:06003] Signal code:  (-6)
[runnervm1li68:06003] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f54d3645330]
[runnervm1li68:06003] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f54d369eb2c]
[runnervm1li68:06003] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f54d364527e]
[runnervm1li68:06003] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f54d36288ff]
[runnervm1li68:06003] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f54d3aa5ff5]
[runnervm1li68:06003] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f54d3abb0da]
[runnervm1li68:06003] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f54d3aa5a55]
[runnervm1li68:06003] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f54d3aa5a6f]
[runnervm1li68:06003] [ 8] plumed(+0x146dd)[0x56177b4e36dd]
[runnervm1li68:06003] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f54d362a1ca]
[runnervm1li68:06003] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f54d362a28b]
[runnervm1li68:06003] [11] plumed(+0x15365)[0x56177b4e4365]
[runnervm1li68:06003] *** End of error message ***
</pre>
{% endraw %}
