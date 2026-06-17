**Project ID:** [plumID:23.027]({{ '/' | absolute_url }}eggs/23/027/)  
Stderr for source:  water-structure-driver.dat   
Download: [zipped raw stdout](water-structure-driver.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](water-structure-driver.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @150 : keyword ARG is compulsory for this action
[runnervm7b5n9:05734] *** Process received signal ***
[runnervm7b5n9:05734] Signal: Aborted (6)
[runnervm7b5n9:05734] Signal code:  (-6)
[runnervm7b5n9:05734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6a78a45330]
[runnervm7b5n9:05734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6a78a9eb2c]
[runnervm7b5n9:05734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6a78a4527e]
[runnervm7b5n9:05734] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6a78a288ff]
[runnervm7b5n9:05734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6a78ea5ff5]
[runnervm7b5n9:05734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6a78ebb0da]
[runnervm7b5n9:05734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6a78ea5a55]
[runnervm7b5n9:05734] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6a78ea5a6f]
[runnervm7b5n9:05734] [ 8] plumed_master(+0x146dd)[0x55fa35e936dd]
[runnervm7b5n9:05734] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6a78a2a1ca]
[runnervm7b5n9:05734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6a78a2a28b]
[runnervm7b5n9:05734] [11] plumed_master(+0x15365)[0x55fa35e94365]
[runnervm7b5n9:05734] *** End of error message ***
</pre>
{% endraw %}
