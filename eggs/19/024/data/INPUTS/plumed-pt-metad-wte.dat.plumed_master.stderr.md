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
[fv-az659-568:45081] *** Process received signal ***
[fv-az659-568:45081] Signal: Aborted (6)
[fv-az659-568:45081] Signal code:  (-6)
[fv-az659-568:45081] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f34c0842520]
[fv-az659-568:45081] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f34c08969fc]
[fv-az659-568:45081] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f34c0842476]
[fv-az659-568:45081] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f34c08287f3]
[fv-az659-568:45081] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f34c0ca2b9e]
[fv-az659-568:45081] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f34c0cae20c]
[fv-az659-568:45081] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f34c0cae277]
[fv-az659-568:45081] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f34c0cae52b]
[fv-az659-568:45081] [ 8] plumed_master(+0x14274)[0x55f023ea0274]
[fv-az659-568:45081] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f34c0829d90]
[fv-az659-568:45081] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f34c0829e40]
[fv-az659-568:45081] [11] plumed_master(+0x14ed5)[0x55f023ea0ed5]
[fv-az659-568:45081] *** End of error message ***
</pre>
{% endraw %}
