**Project ID:** [plumID:23.031]({{ '/' | absolute_url }}eggs/23/031/)  
Stderr for source:  1mfy/02-BETH/2-Production/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: SHADOW LABEL=rmsd ATOMS=rna NOPBC UPDATE=100
Maybe a missing space or a typo?
[fv-az695-456:70754] *** Process received signal ***
[fv-az695-456:70754] Signal: Aborted (6)
[fv-az695-456:70754] Signal code:  (-6)
[fv-az695-456:70754] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb647442520]
[fv-az695-456:70754] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb6474969fc]
[fv-az695-456:70754] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb647442476]
[fv-az695-456:70754] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb6474287f3]
[fv-az695-456:70754] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb6478a2b9e]
[fv-az695-456:70754] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb6478ae20c]
[fv-az695-456:70754] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb6478ae277]
[fv-az695-456:70754] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb6478ae52b]
[fv-az695-456:70754] [ 8] plumed(+0x12f48)[0x55ea3cda6f48]
[fv-az695-456:70754] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb647429d90]
[fv-az695-456:70754] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb647429e40]
[fv-az695-456:70754] [11] plumed(+0x131e5)[0x55ea3cda71e5]
[fv-az695-456:70754] *** End of error message ***
</pre>
{% endraw %}
