**Project ID:** [plumID:21.003]({{ '/' | absolute_url }}eggs/21/003/)  
Stderr for source:  metainf_input/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT
[runnervm7b5n9:09555] *** Process received signal ***
[runnervm7b5n9:09555] Signal: Aborted (6)
[runnervm7b5n9:09555] Signal code:  (-6)
[runnervm7b5n9:09555] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1478245330]
[runnervm7b5n9:09555] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f147829eb2c]
[runnervm7b5n9:09555] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f147824527e]
[runnervm7b5n9:09555] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f14782288ff]
[runnervm7b5n9:09555] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f14786a5ff5]
[runnervm7b5n9:09555] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f14786bb0da]
[runnervm7b5n9:09555] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f14786a5a55]
[runnervm7b5n9:09555] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f14786a5a6f]
[runnervm7b5n9:09555] [ 8] plumed_master(+0x146dd)[0x55b5c615b6dd]
[runnervm7b5n9:09555] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f147822a1ca]
[runnervm7b5n9:09555] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f147822a28b]
[runnervm7b5n9:09555] [11] plumed_master(+0x15365)[0x55b5c615c365]
[runnervm7b5n9:09555] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action SAXS with label test2 : cannot understand the following words from the input line : SCALEINT
[runnervm7b5n9:09554] *** Process received signal ***
[runnervm7b5n9:09554] Signal: Aborted (6)
[runnervm7b5n9:09554] Signal code:  (-6)
[runnervm7b5n9:09554] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5251a45330]
[runnervm7b5n9:09554] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5251a9eb2c]
[runnervm7b5n9:09554] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5251a4527e]
[runnervm7b5n9:09554] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5251a288ff]
[runnervm7b5n9:09554] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f5251ea5ff5]
[runnervm7b5n9:09554] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f5251ebb0da]
[runnervm7b5n9:09554] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f5251ea5a55]
[runnervm7b5n9:09554] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f5251ea5a6f]
[runnervm7b5n9:09554] [ 8] plumed_master(+0x146dd)[0x55f8113bb6dd]
[runnervm7b5n9:09554] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5251a2a1ca]
[runnervm7b5n9:09554] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5251a2a28b]
[runnervm7b5n9:09554] [11] plumed_master(+0x15365)[0x55f8113bc365]
[runnervm7b5n9:09554] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node runnervm7b5n9 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}
