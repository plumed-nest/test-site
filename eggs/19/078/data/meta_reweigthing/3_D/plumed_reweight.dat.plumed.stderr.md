**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/3_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=20
Maybe a missing space or a typo?
[fv-az532-512:10448] *** Process received signal ***
[fv-az532-512:10448] Signal: Aborted (6)
[fv-az532-512:10448] Signal code:  (-6)
[fv-az532-512:10448] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa6dd842520]
[fv-az532-512:10448] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa6dd8969fc]
[fv-az532-512:10448] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa6dd842476]
[fv-az532-512:10448] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa6dd8287f3]
[fv-az532-512:10448] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa6ddca4f26]
[fv-az532-512:10448] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa6ddcb6d9c]
[fv-az532-512:10448] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa6ddcb6e07]
[fv-az532-512:10448] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa6ddcb70bb]
[fv-az532-512:10448] [ 8] plumed(+0x12f48)[0x556ce0952f48]
[fv-az532-512:10448] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa6dd829d90]
[fv-az532-512:10448] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa6dd829e40]
[fv-az532-512:10448] [11] plumed(+0x131e5)[0x556ce09531e5]
[fv-az532-512:10448] *** End of error message ***
</pre>
{% endraw %}
