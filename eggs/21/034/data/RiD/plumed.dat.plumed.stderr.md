**Project ID:** [plumID:21.034]({{ '/' | absolute_url }}eggs/21/034/)  
Stderr for source:  RiD/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: DEEPFE LABEL=dpfe TRUST_LVL_1=1.0 TRUST_LVL_2=2.0 MODEL=graph.pb ARG=dih-000-01,dih-001-00,dih-001-01,dih-002-00,dih-002-01,dih-003-00,dih-003-01,dih-004-00,dih-004-01,dih-005-00,dih-005-01,dih-006-00,dih-006-01,dih-007-00,dih-007-01,dih-008-00,dih-008-01,dih-009-00
Maybe a missing space or a typo?
[fv-az659-568:41690] *** Process received signal ***
[fv-az659-568:41690] Signal: Aborted (6)
[fv-az659-568:41690] Signal code:  (-6)
[fv-az659-568:41690] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0bbd842520]
[fv-az659-568:41690] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0bbd8969fc]
[fv-az659-568:41690] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0bbd842476]
[fv-az659-568:41690] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0bbd8287f3]
[fv-az659-568:41690] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0bbdca2b9e]
[fv-az659-568:41690] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0bbdcae20c]
[fv-az659-568:41690] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0bbdcae277]
[fv-az659-568:41690] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0bbdcae52b]
[fv-az659-568:41690] [ 8] plumed(+0x12f48)[0x5604325cdf48]
[fv-az659-568:41690] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0bbd829d90]
[fv-az659-568:41690] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0bbd829e40]
[fv-az659-568:41690] [11] plumed(+0x131e5)[0x5604325ce1e5]
[fv-az659-568:41690] *** End of error message ***
</pre>
{% endraw %}
