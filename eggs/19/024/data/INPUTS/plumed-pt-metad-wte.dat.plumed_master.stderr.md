**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
Stderr for source:  INPUTS/plumed-pt-metad-wte.dat   
Download: [zipped raw stdout](plumed-pt-metad-wte.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed-pt-metad-wte.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:564) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled @6.bias in in grid input
[fv-az695-903:09836] *** Process received signal ***
[fv-az695-903:09836] Signal: Aborted (6)
[fv-az695-903:09836] Signal code:  (-6)
[fv-az695-903:09836] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f84f8e42520]
[fv-az695-903:09836] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f84f8e969fc]
[fv-az695-903:09836] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f84f8e42476]
[fv-az695-903:09836] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f84f8e287f3]
[fv-az695-903:09836] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f84f92a4f26]
[fv-az695-903:09836] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f84f92b6d9c]
[fv-az695-903:09836] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f84f92b6e07]
[fv-az695-903:09836] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f84f92b70bb]
[fv-az695-903:09836] [ 8] plumed_master(+0x12ebf)[0x558546197ebf]
[fv-az695-903:09836] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f84f8e29d90]
[fv-az695-903:09836] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f84f8e29e40]
[fv-az695-903:09836] [11] plumed_master(+0x13155)[0x558546198155]
[fv-az695-903:09836] *** End of error message ***
</pre>
{% endraw %}
