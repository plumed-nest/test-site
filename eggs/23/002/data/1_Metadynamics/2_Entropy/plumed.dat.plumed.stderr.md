**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  1_Metadynamics/2_Entropy/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[runnervm1li68:07674] *** Process received signal ***
[runnervm1li68:07674] Signal: Aborted (6)
[runnervm1li68:07674] Signal code:  (-6)
[runnervm1li68:07674] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f64a3445330]
[runnervm1li68:07674] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f64a349eb2c]
[runnervm1li68:07674] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f64a344527e]
[runnervm1li68:07674] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f64a34288ff]
[runnervm1li68:07674] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f64a38a5ff5]
[runnervm1li68:07674] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f64a38bb0da]
[runnervm1li68:07674] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f64a38a5a55]
[runnervm1li68:07674] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f64a38a5a6f]
[runnervm1li68:07674] [ 8] plumed(+0x146dd)[0x55ac32c6c6dd]
[runnervm1li68:07674] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f64a342a1ca]
[runnervm1li68:07674] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f64a342a28b]
[runnervm1li68:07674] [11] plumed(+0x15365)[0x55ac32c6d365]
[runnervm1li68:07674] *** End of error message ***
</pre>
{% endraw %}
