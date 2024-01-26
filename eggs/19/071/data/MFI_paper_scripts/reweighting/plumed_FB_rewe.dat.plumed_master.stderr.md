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
(tools/Grid.cpp:564) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[fv-az1493-330:08936] *** Process received signal ***
[fv-az1493-330:08936] Signal: Aborted (6)
[fv-az1493-330:08936] Signal code:  (-6)
[fv-az1493-330:08936] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f59f4642520]
[fv-az1493-330:08936] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f59f46969fc]
[fv-az1493-330:08936] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f59f4642476]
[fv-az1493-330:08936] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f59f46287f3]
[fv-az1493-330:08936] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f59f4aa4f26]
[fv-az1493-330:08936] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f59f4ab6d9c]
[fv-az1493-330:08936] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f59f4ab6e07]
[fv-az1493-330:08936] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f59f4ab70bb]
[fv-az1493-330:08936] [ 8] plumed_master(+0x12ebf)[0x56502923aebf]
[fv-az1493-330:08936] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f59f4629d90]
[fv-az1493-330:08936] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f59f4629e40]
[fv-az1493-330:08936] [11] plumed_master(+0x13155)[0x56502923b155]
[fv-az1493-330:08936] *** End of error message ***
</pre>
{% endraw %}
