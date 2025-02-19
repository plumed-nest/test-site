**Project ID:** [plumID:22.006]({{ '/' | absolute_url }}eggs/22/006/)  
Stderr for source:  analysis/contacts.plumed   
Download: [zipped raw stdout](contacts.plumed.plumed_master.stdout.txt.zip) - [zipped raw stderr](contacts.plumed.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @92 : keyword ARG is compulsory for this action
[fv-az2027-338:06734] *** Process received signal ***
[fv-az2027-338:06734] Signal: Aborted (6)
[fv-az2027-338:06734] Signal code:  (-6)
[fv-az2027-338:06734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f292e045330]
[fv-az2027-338:06734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f292e09eb2c]
[fv-az2027-338:06734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f292e04527e]
[fv-az2027-338:06734] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f292e0288ff]
[fv-az2027-338:06734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f292e4a5ff5]
[fv-az2027-338:06734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f292e4bb0da]
[fv-az2027-338:06734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f292e4a5a55]
[fv-az2027-338:06734] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f292e4a5a6f]
[fv-az2027-338:06734] [ 8] plumed_master(+0x146dd)[0x556fd42646dd]
[fv-az2027-338:06734] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f292e02a1ca]
[fv-az2027-338:06734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f292e02a28b]
[fv-az2027-338:06734] [11] plumed_master(+0x15365)[0x556fd4265365]
[fv-az2027-338:06734] *** End of error message ***
</pre>
{% endraw %}
