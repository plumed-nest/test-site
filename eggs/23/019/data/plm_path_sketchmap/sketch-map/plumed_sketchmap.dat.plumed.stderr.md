**Project ID:** [plumID:23.019]({{ '/' | absolute_url }}eggs/23/019/)  
Stderr for source:  plm_path_sketchmap/sketch-map/plumed_sketchmap.dat   
Download: [zipped raw stdout](plumed_sketchmap.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_sketchmap.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action VSTACK with label mat : no arguments were specificed
[runnervm7b5n9:06018] *** Process received signal ***
[runnervm7b5n9:06018] Signal: Aborted (6)
[runnervm7b5n9:06018] Signal code:  (-6)
[runnervm7b5n9:06018] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7efca2e45330]
[runnervm7b5n9:06018] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7efca2e9eb2c]
[runnervm7b5n9:06018] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7efca2e4527e]
[runnervm7b5n9:06018] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7efca2e288ff]
[runnervm7b5n9:06018] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7efca32a5ff5]
[runnervm7b5n9:06018] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7efca32bb0da]
[runnervm7b5n9:06018] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7efca32a5a55]
[runnervm7b5n9:06018] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7efca32a5a6f]
[runnervm7b5n9:06018] [ 8] plumed(+0x146dd)[0x55ca4f0046dd]
[runnervm7b5n9:06018] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7efca2e2a1ca]
[runnervm7b5n9:06018] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7efca2e2a28b]
[runnervm7b5n9:06018] [11] plumed(+0x15365)[0x55ca4f005365]
[runnervm7b5n9:06018] *** End of error message ***
</pre>
{% endraw %}
