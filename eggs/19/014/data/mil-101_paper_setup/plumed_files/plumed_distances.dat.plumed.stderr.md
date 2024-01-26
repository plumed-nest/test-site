**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
Stderr for source:  mil-101_paper_setup/plumed_files/plumed_distances.dat   
Download: [zipped raw stdout](plumed_distances.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_distances.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file hills not found
[fv-az695-903:09926] *** Process received signal ***
[fv-az695-903:09926] Signal: Aborted (6)
[fv-az695-903:09926] Signal code:  (-6)
[fv-az695-903:09926] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f791de42520]
[fv-az695-903:09926] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f791de969fc]
[fv-az695-903:09926] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f791de42476]
[fv-az695-903:09926] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f791de287f3]
[fv-az695-903:09926] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f791e2a4f26]
[fv-az695-903:09926] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f791e2b6d9c]
[fv-az695-903:09926] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f791e2b6e07]
[fv-az695-903:09926] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f791e2b70bb]
[fv-az695-903:09926] [ 8] plumed(+0x12f48)[0x55cca5192f48]
[fv-az695-903:09926] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f791de29d90]
[fv-az695-903:09926] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f791de29e40]
[fv-az695-903:09926] [11] plumed(+0x131e5)[0x55cca51931e5]
[fv-az695-903:09926] *** End of error message ***
</pre>
{% endraw %}
