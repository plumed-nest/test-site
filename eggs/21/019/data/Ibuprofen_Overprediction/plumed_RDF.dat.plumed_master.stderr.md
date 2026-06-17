**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_RDF.dat   
Download: [zipped raw stdout](plumed_RDF.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_RDF.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action COM with label RDF_c284 : it was not possible to interpret atom name ...
[runnervm1li68:11191] *** Process received signal ***
[runnervm1li68:11191] Signal: Aborted (6)
[runnervm1li68:11191] Signal code:  (-6)
[runnervm1li68:11191] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9e68845330]
[runnervm1li68:11191] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9e6889eb2c]
[runnervm1li68:11191] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9e6884527e]
[runnervm1li68:11191] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9e688288ff]
[runnervm1li68:11191] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9e68ca5ff5]
[runnervm1li68:11191] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9e68cbb0da]
[runnervm1li68:11191] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9e68ca5a55]
[runnervm1li68:11191] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9e68ca5a6f]
[runnervm1li68:11191] [ 8] plumed_master(+0x146dd)[0x559d30d026dd]
[runnervm1li68:11191] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9e6882a1ca]
[runnervm1li68:11191] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9e6882a28b]
[runnervm1li68:11191] [11] plumed_master(+0x15365)[0x559d30d03365]
[runnervm1li68:11191] *** End of error message ***
</pre>
{% endraw %}
