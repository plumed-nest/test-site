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
(tools/Grid.cpp:547) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled @6.bias in in grid input
[fv-az1108-41:75479] *** Process received signal ***
[fv-az1108-41:75479] Signal: Aborted (6)
[fv-az1108-41:75479] Signal code:  (-6)
[fv-az1108-41:75479] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8e9c442520]
[fv-az1108-41:75479] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8e9c4969fc]
[fv-az1108-41:75479] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8e9c442476]
[fv-az1108-41:75479] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8e9c4287f3]
[fv-az1108-41:75479] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8e9c8a2b9e]
[fv-az1108-41:75479] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8e9c8ae20c]
[fv-az1108-41:75479] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8e9c8ae277]
[fv-az1108-41:75479] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8e9c8ae52b]
[fv-az1108-41:75479] [ 8] plumed_master(+0x14274)[0x56293f1ca274]
[fv-az1108-41:75479] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8e9c429d90]
[fv-az1108-41:75479] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8e9c429e40]
[fv-az1108-41:75479] [11] plumed_master(+0x14ed5)[0x56293f1caed5]
[fv-az1108-41:75479] *** End of error message ***
</pre>
{% endraw %}