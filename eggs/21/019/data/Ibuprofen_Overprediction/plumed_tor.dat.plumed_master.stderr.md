**Project ID:** [plumID:21.019]({{ '/' | absolute_url }}eggs/21/019/)  
Stderr for source:  Ibuprofen_Overprediction/plumed_tor.dat   
Download: [zipped raw stdout](plumed_tor.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_tor.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:981) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: ATOMS141=9314,9319,9310,9313
Maybe a missing space or a typo?
[fv-az532-512:09431] *** Process received signal ***
[fv-az532-512:09431] Signal: Aborted (6)
[fv-az532-512:09431] Signal code:  (-6)
[fv-az532-512:09431] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5a68642520]
[fv-az532-512:09431] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5a686969fc]
[fv-az532-512:09431] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5a68642476]
[fv-az532-512:09431] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5a686287f3]
[fv-az532-512:09431] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f5a68aa4f26]
[fv-az532-512:09431] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f5a68ab6d9c]
[fv-az532-512:09431] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f5a68ab6e07]
[fv-az532-512:09431] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5a68ab70bb]
[fv-az532-512:09431] [ 8] plumed_master(+0x12ebf)[0x5575684e2ebf]
[fv-az532-512:09431] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5a68629d90]
[fv-az532-512:09431] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5a68629e40]
[fv-az532-512:09431] [11] plumed_master(+0x13155)[0x5575684e3155]
[fv-az532-512:09431] *** End of error message ***
</pre>
{% endraw %}
