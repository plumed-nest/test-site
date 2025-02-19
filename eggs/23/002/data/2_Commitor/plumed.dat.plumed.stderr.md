**Project ID:** [plumID:23.002]({{ '/' | absolute_url }}eggs/23/002/)  
Stderr for source:  2_Commitor/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action PAIRENTROPY with label @s13 : keyword GRID_BIN is compulsory for this action
[fv-az1436-30:07803] *** Process received signal ***
[fv-az1436-30:07803] Signal: Aborted (6)
[fv-az1436-30:07803] Signal code:  (-6)
[fv-az1436-30:07803] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcb96a45330]
[fv-az1436-30:07803] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcb96a9eb2c]
[fv-az1436-30:07803] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcb96a4527e]
[fv-az1436-30:07803] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcb96a288ff]
[fv-az1436-30:07803] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcb96ea5ff5]
[fv-az1436-30:07803] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcb96ebb0da]
[fv-az1436-30:07803] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcb96ea5a55]
[fv-az1436-30:07803] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcb96ea5a6f]
[fv-az1436-30:07803] [ 8] plumed(+0x146dd)[0x55c734de96dd]
[fv-az1436-30:07803] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcb96a2a1ca]
[fv-az1436-30:07803] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcb96a2a28b]
[fv-az1436-30:07803] [11] plumed(+0x15365)[0x55c734dea365]
[fv-az1436-30:07803] *** End of error message ***
</pre>
{% endraw %}
