**Project ID:** [plumID:19.050]({{ '/' | absolute_url }}eggs/19/050/)  
Stderr for source:  plumed_histogram.dat   
Download: [zipped raw stdout](plumed_histogram.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_histogram.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @33 : keyword ARG is compulsory for this action
[fv-az1372-996:12280] *** Process received signal ***
[fv-az1372-996:12280] Signal: Aborted (6)
[fv-az1372-996:12280] Signal code:  (-6)
[fv-az1372-996:12280] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1179c45330]
[fv-az1372-996:12280] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1179c9eb2c]
[fv-az1372-996:12280] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1179c4527e]
[fv-az1372-996:12280] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1179c288ff]
[fv-az1372-996:12280] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f117a0a5ff5]
[fv-az1372-996:12280] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f117a0bb0da]
[fv-az1372-996:12280] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f117a0a5a55]
[fv-az1372-996:12280] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f117a0a5a6f]
[fv-az1372-996:12280] [ 8] plumed_master(+0x146dd)[0x55e6d2a616dd]
[fv-az1372-996:12280] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1179c2a1ca]
[fv-az1372-996:12280] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1179c2a28b]
[fv-az1372-996:12280] [11] plumed_master(+0x15365)[0x55e6d2a62365]
[fv-az1372-996:12280] *** End of error message ***
</pre>
{% endraw %}
