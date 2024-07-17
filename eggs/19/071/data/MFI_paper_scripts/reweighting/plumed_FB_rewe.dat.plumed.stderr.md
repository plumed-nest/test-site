**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
Download: [zipped raw stdout](plumed_FB_rewe.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_FB_rewe.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:564) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[fv-az1110-714:74185] *** Process received signal ***
[fv-az1110-714:74185] Signal: Aborted (6)
[fv-az1110-714:74185] Signal code:  (-6)
[fv-az1110-714:74185] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0635e42520]
[fv-az1110-714:74185] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0635e969fc]
[fv-az1110-714:74185] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0635e42476]
[fv-az1110-714:74185] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0635e287f3]
[fv-az1110-714:74185] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f06362a2b9e]
[fv-az1110-714:74185] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f06362ae20c]
[fv-az1110-714:74185] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f06362ae277]
[fv-az1110-714:74185] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f06362ae52b]
[fv-az1110-714:74185] [ 8] plumed(+0x12f48)[0x55bc1e4eaf48]
[fv-az1110-714:74185] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0635e29d90]
[fv-az1110-714:74185] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0635e29e40]
[fv-az1110-714:74185] [11] plumed(+0x131e5)[0x55bc1e4eb1e5]
[fv-az1110-714:74185] *** End of error message ***
</pre>
{% endraw %}
