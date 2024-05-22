**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
Download: [zipped raw stdout](plumed_FB_rewe.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FB_rewe.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:547) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[fv-az1435-553:43966] *** Process received signal ***
[fv-az1435-553:43966] Signal: Aborted (6)
[fv-az1435-553:43966] Signal code:  (-6)
[fv-az1435-553:43966] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2b6bc42520]
[fv-az1435-553:43966] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2b6bc969fc]
[fv-az1435-553:43966] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2b6bc42476]
[fv-az1435-553:43966] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2b6bc287f3]
[fv-az1435-553:43966] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2b6c0a2b9e]
[fv-az1435-553:43966] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2b6c0ae20c]
[fv-az1435-553:43966] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2b6c0ae277]
[fv-az1435-553:43966] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2b6c0ae52b]
[fv-az1435-553:43966] [ 8] plumed_master(+0x14274)[0x55579129b274]
[fv-az1435-553:43966] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2b6bc29d90]
[fv-az1435-553:43966] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2b6bc29e40]
[fv-az1435-553:43966] [11] plumed_master(+0x14ed5)[0x55579129bed5]
[fv-az1435-553:43966] *** End of error message ***
</pre>
{% endraw %}
