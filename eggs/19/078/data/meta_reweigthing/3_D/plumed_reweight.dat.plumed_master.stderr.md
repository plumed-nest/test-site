**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/3_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=20
Maybe a missing space or a typo?
[fv-az532-512:10456] *** Process received signal ***
[fv-az532-512:10456] Signal: Aborted (6)
[fv-az532-512:10456] Signal code:  (-6)
[fv-az532-512:10456] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2ee0042520]
[fv-az532-512:10456] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2ee00969fc]
[fv-az532-512:10456] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2ee0042476]
[fv-az532-512:10456] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2ee00287f3]
[fv-az532-512:10456] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f2ee04a4f26]
[fv-az532-512:10456] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f2ee04b6d9c]
[fv-az532-512:10456] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f2ee04b6e07]
[fv-az532-512:10456] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2ee04b70bb]
[fv-az532-512:10456] [ 8] plumed_master(+0x12ebf)[0x561e649d8ebf]
[fv-az532-512:10456] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2ee0029d90]
[fv-az532-512:10456] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2ee0029e40]
[fv-az532-512:10456] [11] plumed_master(+0x13155)[0x561e649d9155]
[fv-az532-512:10456] *** End of error message ***
</pre>
{% endraw %}
