**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_for_reference_map.dat   
Download: [zipped raw stdout](plumed_for_reference_map.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_for_reference_map.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action VSTACK with label mat : keyword ARG is compulsory for this action
[runnervm7b5n9:05958] *** Process received signal ***
[runnervm7b5n9:05958] Signal: Aborted (6)
[runnervm7b5n9:05958] Signal code:  (-6)
[runnervm7b5n9:05958] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb2ac245330]
[runnervm7b5n9:05958] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb2ac29eb2c]
[runnervm7b5n9:05958] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb2ac24527e]
[runnervm7b5n9:05958] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb2ac2288ff]
[runnervm7b5n9:05958] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb2ac6a5ff5]
[runnervm7b5n9:05958] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb2ac6bb0da]
[runnervm7b5n9:05958] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb2ac6a5a55]
[runnervm7b5n9:05958] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb2ac6a5a6f]
[runnervm7b5n9:05958] [ 8] plumed_master(+0x146dd)[0x563689a5a6dd]
[runnervm7b5n9:05958] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb2ac22a1ca]
[runnervm7b5n9:05958] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb2ac22a28b]
[runnervm7b5n9:05958] [11] plumed_master(+0x15365)[0x563689a5b365]
[runnervm7b5n9:05958] *** End of error message ***
</pre>
{% endraw %}
