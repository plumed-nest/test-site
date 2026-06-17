**Project ID:** [plumID:23.004]({{ '/' | absolute_url }}eggs/23/004/)  
Stderr for source:  BiasedCoexistence/IceIII/1-distributions/3000bar-295K/CalculateOptimalSigma/Liquid/plumed-base.dat   
Download: [zipped raw stdout](plumed-base.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-base.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @77 : keyword ARG is compulsory for this action
[runnervm1li68:06115] *** Process received signal ***
[runnervm1li68:06115] Signal: Aborted (6)
[runnervm1li68:06115] Signal code:  (-6)
[runnervm1li68:06115] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc84d245330]
[runnervm1li68:06115] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc84d29eb2c]
[runnervm1li68:06115] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc84d24527e]
[runnervm1li68:06115] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc84d2288ff]
[runnervm1li68:06115] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc84d6a5ff5]
[runnervm1li68:06115] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc84d6bb0da]
[runnervm1li68:06115] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc84d6a5a55]
[runnervm1li68:06115] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc84d6a5a6f]
[runnervm1li68:06115] [ 8] plumed_master(+0x146dd)[0x55fda3db16dd]
[runnervm1li68:06115] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc84d22a1ca]
[runnervm1li68:06115] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc84d22a28b]
[runnervm1li68:06115] [11] plumed_master(+0x15365)[0x55fda3db2365]
[runnervm1li68:06115] *** End of error message ***
</pre>
{% endraw %}
