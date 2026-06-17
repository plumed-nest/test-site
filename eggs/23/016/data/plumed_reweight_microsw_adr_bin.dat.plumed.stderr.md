**Project ID:** [plumID:23.016]({{ '/' | absolute_url }}eggs/23/016/)  
Stderr for source:  plumed_reweight_microsw_adr_bin.dat   
Download: [zipped raw stdout](plumed_reweight_microsw_adr_bin.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_microsw_adr_bin.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s17 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm7b5n9:07077] *** Process received signal ***
[runnervm7b5n9:07077] Signal: Aborted (6)
[runnervm7b5n9:07077] Signal code:  (-6)
[runnervm7b5n9:07077] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f052c245330]
[runnervm7b5n9:07077] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f052c29eb2c]
[runnervm7b5n9:07077] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f052c24527e]
[runnervm7b5n9:07077] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f052c2288ff]
[runnervm7b5n9:07077] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f052c6a5ff5]
[runnervm7b5n9:07077] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f052c6bb0da]
[runnervm7b5n9:07077] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f052c6a5a55]
[runnervm7b5n9:07077] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f052c6a5a6f]
[runnervm7b5n9:07077] [ 8] plumed(+0x146dd)[0x5565d02aa6dd]
[runnervm7b5n9:07077] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f052c22a1ca]
[runnervm7b5n9:07077] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f052c22a28b]
[runnervm7b5n9:07077] [11] plumed(+0x15365)[0x5565d02ab365]
[runnervm7b5n9:07077] *** End of error message ***
</pre>
{% endraw %}
