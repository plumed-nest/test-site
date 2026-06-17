**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pws/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[runnervm1li68:11071] *** Process received signal ***
[runnervm1li68:11071] Signal: Aborted (6)
[runnervm1li68:11071] Signal code:  (-6)
[runnervm1li68:11071] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f30df045330]
[runnervm1li68:11071] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f30df09eb2c]
[runnervm1li68:11071] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f30df04527e]
[runnervm1li68:11071] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f30df0288ff]
[runnervm1li68:11071] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f30df4a5ff5]
[runnervm1li68:11071] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f30df4bb0da]
[runnervm1li68:11071] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f30df4a5a55]
[runnervm1li68:11071] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f30df4a5a6f]
[runnervm1li68:11071] [ 8] plumed_master(+0x146dd)[0x5560207b26dd]
[runnervm1li68:11071] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f30df02a1ca]
[runnervm1li68:11071] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f30df02a28b]
[runnervm1li68:11071] [11] plumed_master(+0x15365)[0x5560207b3365]
[runnervm1li68:11071] *** End of error message ***
</pre>
{% endraw %}
