**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
Stderr for source:  mil-101_paper_setup/plumed_files/plumed_distances.dat   
Download: [zipped raw stdout](plumed_distances.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_distances.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file hills not found
[fv-az695-903:09934] *** Process received signal ***
[fv-az695-903:09934] Signal: Aborted (6)
[fv-az695-903:09934] Signal code:  (-6)
[fv-az695-903:09934] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6327a42520]
[fv-az695-903:09934] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6327a969fc]
[fv-az695-903:09934] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6327a42476]
[fv-az695-903:09934] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6327a287f3]
[fv-az695-903:09934] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f6327ea4f26]
[fv-az695-903:09934] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f6327eb6d9c]
[fv-az695-903:09934] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f6327eb6e07]
[fv-az695-903:09934] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6327eb70bb]
[fv-az695-903:09934] [ 8] plumed_master(+0x12ebf)[0x55a171974ebf]
[fv-az695-903:09934] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6327a29d90]
[fv-az695-903:09934] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6327a29e40]
[fv-az695-903:09934] [11] plumed_master(+0x13155)[0x55a171975155]
[fv-az695-903:09934] *** End of error message ***
</pre>
{% endraw %}
