**Project ID:** [plumID:20.033]({{ '/' | absolute_url }}eggs/20/033/)  
Stderr for source:  ANALYSIS/plumed_histogram.dat   
Download: [zipped raw stdout](plumed_histogram.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_histogram.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @30 : keyword ARG is compulsory for this action
[fv-az1372-996:10071] *** Process received signal ***
[fv-az1372-996:10071] Signal: Aborted (6)
[fv-az1372-996:10071] Signal code:  (-6)
[fv-az1372-996:10071] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7faf2d245330]
[fv-az1372-996:10071] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7faf2d29eb2c]
[fv-az1372-996:10071] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7faf2d24527e]
[fv-az1372-996:10071] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7faf2d2288ff]
[fv-az1372-996:10071] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7faf2d6a5ff5]
[fv-az1372-996:10071] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7faf2d6bb0da]
[fv-az1372-996:10071] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7faf2d6a5a55]
[fv-az1372-996:10071] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7faf2d6a5a6f]
[fv-az1372-996:10071] [ 8] plumed_master(+0x146dd)[0x55eeb5b1e6dd]
[fv-az1372-996:10071] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7faf2d22a1ca]
[fv-az1372-996:10071] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7faf2d22a28b]
[fv-az1372-996:10071] [11] plumed_master(+0x15365)[0x55eeb5b1f365]
[fv-az1372-996:10071] *** End of error message ***
</pre>
{% endraw %}
