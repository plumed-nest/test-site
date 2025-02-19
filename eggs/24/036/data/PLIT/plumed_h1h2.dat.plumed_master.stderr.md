**Project ID:** [plumID:24.036]({{ '/' | absolute_url }}eggs/24/036/)  
Stderr for source:  PLIT/plumed_h1h2.dat   
Download: [zipped raw stdout](plumed_h1h2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_h1h2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @49 : keyword ARG is compulsory for this action
[fv-az2027-338:05515] *** Process received signal ***
[fv-az2027-338:05515] Signal: Aborted (6)
[fv-az2027-338:05515] Signal code:  (-6)
[fv-az2027-338:05515] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0b1f645330]
[fv-az2027-338:05515] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0b1f69eb2c]
[fv-az2027-338:05515] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0b1f64527e]
[fv-az2027-338:05515] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0b1f6288ff]
[fv-az2027-338:05515] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0b1faa5ff5]
[fv-az2027-338:05515] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0b1fabb0da]
[fv-az2027-338:05515] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0b1faa5a55]
[fv-az2027-338:05515] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0b1faa5a6f]
[fv-az2027-338:05515] [ 8] plumed_master(+0x146dd)[0x55a4fd4206dd]
[fv-az2027-338:05515] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0b1f62a1ca]
[fv-az2027-338:05515] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0b1f62a28b]
[fv-az2027-338:05515] [11] plumed_master(+0x15365)[0x55a4fd421365]
[fv-az2027-338:05515] *** End of error message ***
</pre>
{% endraw %}
