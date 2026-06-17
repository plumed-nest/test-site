**Project ID:** [plumID:25.012]({{ '/' | absolute_url }}eggs/25/012/)  
Stderr for source:  OPES_Enhanced_Sampling_with_Committor/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/DLLoader.cpp:50) void* PLMD::DLLoader::load(const std::string&)
Could not load library ./pytorch_model_bias.so
libxpmem.so.0: cannot open shared object file: No such file or directory
[runnervm1li68:04197] *** Process received signal ***
[runnervm1li68:04197] Signal: Aborted (6)
[runnervm1li68:04197] Signal code:  (-6)
[runnervm1li68:04197] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1530245330]
[runnervm1li68:04197] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f153029eb2c]
[runnervm1li68:04197] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f153024527e]
[runnervm1li68:04197] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f15302288ff]
[runnervm1li68:04197] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f15306a5ff5]
[runnervm1li68:04197] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f15306bb0da]
[runnervm1li68:04197] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f15306a5a55]
[runnervm1li68:04197] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f15306a5a6f]
[runnervm1li68:04197] [ 8] plumed(+0x146dd)[0x55d307fc46dd]
[runnervm1li68:04197] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f153022a1ca]
[runnervm1li68:04197] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f153022a28b]
[runnervm1li68:04197] [11] plumed(+0x15365)[0x55d307fc5365]
[runnervm1li68:04197] *** End of error message ***
</pre>
{% endraw %}
