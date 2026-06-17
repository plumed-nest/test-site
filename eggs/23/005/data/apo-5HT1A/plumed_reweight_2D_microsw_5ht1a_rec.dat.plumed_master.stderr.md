**Project ID:** [plumID:23.005]({{ '/' | absolute_url }}eggs/23/005/)  
Stderr for source:  apo-5HT1A/plumed_reweight_2D_microsw_5ht1a_rec.dat   
Download: [zipped raw stdout](plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_2D_microsw_5ht1a_rec.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s15 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:06162] *** Process received signal ***
[runnervm1li68:06162] Signal: Aborted (6)
[runnervm1li68:06162] Signal code:  (-6)
[runnervm1li68:06162] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9fe0e45330]
[runnervm1li68:06162] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9fe0e9eb2c]
[runnervm1li68:06162] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9fe0e4527e]
[runnervm1li68:06162] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9fe0e288ff]
[runnervm1li68:06162] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9fe12a5ff5]
[runnervm1li68:06162] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9fe12bb0da]
[runnervm1li68:06162] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9fe12a5a55]
[runnervm1li68:06162] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9fe12a5a6f]
[runnervm1li68:06162] [ 8] plumed_master(+0x146dd)[0x560f3a88b6dd]
[runnervm1li68:06162] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9fe0e2a1ca]
[runnervm1li68:06162] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9fe0e2a28b]
[runnervm1li68:06162] [11] plumed_master(+0x15365)[0x560f3a88c365]
[runnervm1li68:06162] *** End of error message ***
</pre>
{% endraw %}
