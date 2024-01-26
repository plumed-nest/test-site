**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ATOMS141=9314,9319,9310,9313
Maybe a missing space or a typo?
[fv-az532-512:09423] *** Process received signal ***
[fv-az532-512:09423] Signal: Aborted (6)
[fv-az532-512:09423] Signal code:  (-6)
[fv-az532-512:09423] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9540a42520]
[fv-az532-512:09423] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9540a969fc]
[fv-az532-512:09423] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9540a42476]
[fv-az532-512:09423] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9540a287f3]
[fv-az532-512:09423] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9540ea4f26]
[fv-az532-512:09423] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9540eb6d9c]
[fv-az532-512:09423] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9540eb6e07]
[fv-az532-512:09423] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9540eb70bb]
[fv-az532-512:09423] [ 8] plumed(+0x12f48)[0x56041d7bcf48]
[fv-az532-512:09423] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9540a29d90]
[fv-az532-512:09423] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9540a29e40]
[fv-az532-512:09423] [11] plumed(+0x131e5)[0x56041d7bd1e5]
[fv-az532-512:09423] *** End of error message ***
</pre>
{% endraw %}
