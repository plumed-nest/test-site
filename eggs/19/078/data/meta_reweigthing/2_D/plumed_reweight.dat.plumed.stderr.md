**Project ID:** [plumID:19.078]({{ '/' | absolute_url }}eggs/19/078/)  
Stderr for source:  meta_reweigthing/2_D/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ITRE LABEL=it ARG=cc.logweights TEMP=1 MAXITER=20
Maybe a missing space or a typo?
[fv-az695-456:75560] *** Process received signal ***
[fv-az695-456:75560] Signal: Aborted (6)
[fv-az695-456:75560] Signal code:  (-6)
[fv-az695-456:75560] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6309842520]
[fv-az695-456:75560] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f63098969fc]
[fv-az695-456:75560] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6309842476]
[fv-az695-456:75560] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f63098287f3]
[fv-az695-456:75560] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6309ca2b9e]
[fv-az695-456:75560] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6309cae20c]
[fv-az695-456:75560] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6309cae277]
[fv-az695-456:75560] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6309cae52b]
[fv-az695-456:75560] [ 8] plumed(+0x12f48)[0x55579030df48]
[fv-az695-456:75560] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6309829d90]
[fv-az695-456:75560] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6309829e40]
[fv-az695-456:75560] [11] plumed(+0x131e5)[0x55579030e1e5]
[fv-az695-456:75560] *** End of error message ***
</pre>
{% endraw %}
