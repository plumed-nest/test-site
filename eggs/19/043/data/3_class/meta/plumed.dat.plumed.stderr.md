**Project ID:** [plumID:19.043]({{ '/' | absolute_url }}eggs/19/043/)  
Stderr for source:  3_class/meta/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : When using ADAPTIVE Gaussians on a grid SIGMA_MIN must be specified
[fv-az1672-644:08734] *** Process received signal ***
[fv-az1672-644:08734] Signal: Aborted (6)
[fv-az1672-644:08734] Signal code:  (-6)
[fv-az1672-644:08734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3512845330]
[fv-az1672-644:08734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f351289eb2c]
[fv-az1672-644:08734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f351284527e]
[fv-az1672-644:08734] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f35128288ff]
[fv-az1672-644:08734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3512ca5ff5]
[fv-az1672-644:08734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3512cbb0da]
[fv-az1672-644:08734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3512ca5a55]
[fv-az1672-644:08734] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3512ca5a6f]
[fv-az1672-644:08734] [ 8] plumed(+0x146dd)[0x564110a6c6dd]
[fv-az1672-644:08734] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f351282a1ca]
[fv-az1672-644:08734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f351282a28b]
[fv-az1672-644:08734] [11] plumed(+0x15365)[0x564110a6d365]
[fv-az1672-644:08734] *** End of error message ***
</pre>
{% endraw %}
