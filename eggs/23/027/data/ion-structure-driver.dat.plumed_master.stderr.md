**Project ID:** [plumID:23.027]({{ '/' | absolute_url }}eggs/23/027/)  
Stderr for source:  ion-structure-driver.dat   
Download: [zipped raw stdout](ion-structure-driver.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](ion-structure-driver.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DFSCLUSTERING with label dfs0l : keyword ARG is compulsory for this action
[runnervm7b5n9:05773] *** Process received signal ***
[runnervm7b5n9:05773] Signal: Aborted (6)
[runnervm7b5n9:05773] Signal code:  (-6)
[runnervm7b5n9:05773] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f48ade45330]
[runnervm7b5n9:05773] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f48ade9eb2c]
[runnervm7b5n9:05773] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f48ade4527e]
[runnervm7b5n9:05773] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f48ade288ff]
[runnervm7b5n9:05773] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f48ae2a5ff5]
[runnervm7b5n9:05773] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f48ae2bb0da]
[runnervm7b5n9:05773] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f48ae2a5a55]
[runnervm7b5n9:05773] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f48ae2a5a6f]
[runnervm7b5n9:05773] [ 8] plumed_master(+0x146dd)[0x55f8d336d6dd]
[runnervm7b5n9:05773] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f48ade2a1ca]
[runnervm7b5n9:05773] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f48ade2a28b]
[runnervm7b5n9:05773] [11] plumed_master(+0x15365)[0x55f8d336e365]
[runnervm7b5n9:05773] *** End of error message ***
</pre>
{% endraw %}
