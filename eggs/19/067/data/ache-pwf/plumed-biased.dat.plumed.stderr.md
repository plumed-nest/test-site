**Project ID:** [plumID:19.067]({{ '/' | absolute_url }}eggs/19/067/)  
Stderr for source:  ache-pwf/plumed-biased.dat   
Download: [zipped raw stdout](plumed-biased.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-biased.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label meta : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[runnervm1li68:10978] *** Process received signal ***
[runnervm1li68:10978] Signal: Aborted (6)
[runnervm1li68:10978] Signal code:  (-6)
[runnervm1li68:10978] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1fe0445330]
[runnervm1li68:10978] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1fe049eb2c]
[runnervm1li68:10978] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1fe044527e]
[runnervm1li68:10978] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1fe04288ff]
[runnervm1li68:10978] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1fe08a5ff5]
[runnervm1li68:10978] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1fe08bb0da]
[runnervm1li68:10978] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1fe08a5a55]
[runnervm1li68:10978] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1fe08a5a6f]
[runnervm1li68:10978] [ 8] plumed(+0x146dd)[0x561d746f86dd]
[runnervm1li68:10978] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1fe042a1ca]
[runnervm1li68:10978] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1fe042a28b]
[runnervm1li68:10978] [11] plumed(+0x15365)[0x561d746f9365]
[runnervm1li68:10978] *** End of error message ***
</pre>
{% endraw %}
