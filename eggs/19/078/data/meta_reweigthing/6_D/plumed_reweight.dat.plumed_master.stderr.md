**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/6_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=10
Maybe a missing space or a typo?
[fv-az532-512:10547] *** Process received signal ***
[fv-az532-512:10547] Signal: Aborted (6)
[fv-az532-512:10547] Signal code:  (-6)
[fv-az532-512:10547] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0c6c042520]
[fv-az532-512:10547] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0c6c0969fc]
[fv-az532-512:10547] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0c6c042476]
[fv-az532-512:10547] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0c6c0287f3]
[fv-az532-512:10547] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f0c6c4a4f26]
[fv-az532-512:10547] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f0c6c4b6d9c]
[fv-az532-512:10547] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f0c6c4b6e07]
[fv-az532-512:10547] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0c6c4b70bb]
[fv-az532-512:10547] [ 8] plumed_master(+0x12ebf)[0x55936feceebf]
[fv-az532-512:10547] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0c6c029d90]
[fv-az532-512:10547] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0c6c029e40]
[fv-az532-512:10547] [11] plumed_master(+0x13155)[0x55936fecf155]
[fv-az532-512:10547] *** End of error message ***
</pre>
{% endraw %}
