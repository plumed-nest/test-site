**Project ID:** [plumID:23.005]({{ '/' | absolute_url }}eggs/23/005/)  
Stderr for source:  apo-5HT1A/plumed_reweight_microsw_5ht1a_rec.dat   
Download: [zipped raw stdout](plumed_reweight_microsw_5ht1a_rec.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_microsw_5ht1a_rec.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s15 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm1li68:06214] *** Process received signal ***
[runnervm1li68:06214] Signal: Aborted (6)
[runnervm1li68:06214] Signal code:  (-6)
[runnervm1li68:06214] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f510e045330]
[runnervm1li68:06214] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f510e09eb2c]
[runnervm1li68:06214] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f510e04527e]
[runnervm1li68:06214] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f510e0288ff]
[runnervm1li68:06214] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f510e4a5ff5]
[runnervm1li68:06214] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f510e4bb0da]
[runnervm1li68:06214] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f510e4a5a55]
[runnervm1li68:06214] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f510e4a5a6f]
[runnervm1li68:06214] [ 8] plumed_master(+0x146dd)[0x55e03b13d6dd]
[runnervm1li68:06214] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f510e02a1ca]
[runnervm1li68:06214] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f510e02a28b]
[runnervm1li68:06214] [11] plumed_master(+0x15365)[0x55e03b13e365]
[runnervm1li68:06214] *** End of error message ***
</pre>
{% endraw %}
