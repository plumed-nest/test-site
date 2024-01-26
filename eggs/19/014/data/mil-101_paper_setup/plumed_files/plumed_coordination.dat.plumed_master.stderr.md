**Project ID:** [plumID:19.014]({{ '/' | absolute_url }}eggs/19/014/)  
Stderr for source:  mil-101_paper_setup/plumed_files/plumed_coordination.dat   
Download: [zipped raw stdout](plumed_coordination.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_coordination.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : restart file hills not found
[fv-az695-903:09903] *** Process received signal ***
[fv-az695-903:09903] Signal: Aborted (6)
[fv-az695-903:09903] Signal code:  (-6)
[fv-az695-903:09903] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f11e4842520]
[fv-az695-903:09903] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f11e48969fc]
[fv-az695-903:09903] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f11e4842476]
[fv-az695-903:09903] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f11e48287f3]
[fv-az695-903:09903] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f11e4ca4f26]
[fv-az695-903:09903] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f11e4cb6d9c]
[fv-az695-903:09903] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f11e4cb6e07]
[fv-az695-903:09903] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f11e4cb70bb]
[fv-az695-903:09903] [ 8] plumed_master(+0x12ebf)[0x562f61752ebf]
[fv-az695-903:09903] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f11e4829d90]
[fv-az695-903:09903] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f11e4829e40]
[fv-az695-903:09903] [11] plumed_master(+0x13155)[0x562f61753155]
[fv-az695-903:09903] *** End of error message ***
</pre>
{% endraw %}
