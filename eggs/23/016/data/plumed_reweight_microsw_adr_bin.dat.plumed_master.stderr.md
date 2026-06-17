**Project ID:** [plumID:23.016]({{ '/' | absolute_url }}eggs/23/016/)  
Stderr for source:  plumed_reweight_microsw_adr_bin.dat   
Download: [zipped raw stdout](plumed_reweight_microsw_adr_bin.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_microsw_adr_bin.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s17 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm7b5n9:07094] *** Process received signal ***
[runnervm7b5n9:07094] Signal: Aborted (6)
[runnervm7b5n9:07094] Signal code:  (-6)
[runnervm7b5n9:07094] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fddde445330]
[runnervm7b5n9:07094] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fddde49eb2c]
[runnervm7b5n9:07094] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fddde44527e]
[runnervm7b5n9:07094] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fddde4288ff]
[runnervm7b5n9:07094] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fddde8a5ff5]
[runnervm7b5n9:07094] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fddde8bb0da]
[runnervm7b5n9:07094] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fddde8a5a55]
[runnervm7b5n9:07094] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fddde8a5a6f]
[runnervm7b5n9:07094] [ 8] plumed_master(+0x146dd)[0x559e025fc6dd]
[runnervm7b5n9:07094] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fddde42a1ca]
[runnervm7b5n9:07094] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fddde42a28b]
[runnervm7b5n9:07094] [11] plumed_master(+0x15365)[0x559e025fd365]
[runnervm7b5n9:07094] *** End of error message ***
</pre>
{% endraw %}
