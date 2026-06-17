**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[runnervm7b5n9:09520] *** Process received signal ***
[runnervm7b5n9:09520] Signal: Aborted (6)
[runnervm7b5n9:09520] Signal code:  (-6)
[runnervm7b5n9:09520] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe213c45330]
[runnervm7b5n9:09520] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe213c9eb2c]
[runnervm7b5n9:09520] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe213c4527e]
[runnervm7b5n9:09520] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe213c288ff]
[runnervm7b5n9:09520] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe2140a5ff5]
[runnervm7b5n9:09520] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe2140bb0da]
[runnervm7b5n9:09520] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe2140a5a55]
[runnervm7b5n9:09520] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe2140a5a6f]
[runnervm7b5n9:09520] [ 8] plumed(+0x146dd)[0x55f6e45af6dd]
[runnervm7b5n9:09520] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe213c2a1ca]
[runnervm7b5n9:09520] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe213c2a28b]
[runnervm7b5n9:09520] [11] plumed(+0x15365)[0x55f6e45b0365]
[runnervm7b5n9:09520] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT=1680
[runnervm7b5n9:09519] *** Process received signal ***
[runnervm7b5n9:09519] Signal: Aborted (6)
[runnervm7b5n9:09519] Signal code:  (-6)
[runnervm7b5n9:09519] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fdce6c45330]
[runnervm7b5n9:09519] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fdce6c9eb2c]
[runnervm7b5n9:09519] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fdce6c4527e]
[runnervm7b5n9:09519] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fdce6c288ff]
[runnervm7b5n9:09519] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fdce70a5ff5]
[runnervm7b5n9:09519] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fdce70bb0da]
[runnervm7b5n9:09519] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fdce70a5a55]
[runnervm7b5n9:09519] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fdce70a5a6f]
[runnervm7b5n9:09519] [ 8] plumed(+0x146dd)[0x559563f126dd]
[runnervm7b5n9:09519] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fdce6c2a1ca]
[runnervm7b5n9:09519] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fdce6c2a28b]
[runnervm7b5n9:09519] [11] plumed(+0x15365)[0x559563f13365]
[runnervm7b5n9:09519] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node runnervm7b5n9 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
