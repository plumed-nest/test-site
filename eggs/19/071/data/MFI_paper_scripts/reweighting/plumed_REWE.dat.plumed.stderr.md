**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_REWE.dat   
Download: [zipped raw stdout](plumed_REWE.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_REWE.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:243) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az1493-330:08959] *** Process received signal ***
[fv-az1493-330:08959] Signal: Aborted (6)
[fv-az1493-330:08959] Signal code:  (-6)
[fv-az1493-330:08959] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9f9b442520]
[fv-az1493-330:08959] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9f9b4969fc]
[fv-az1493-330:08959] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9f9b442476]
[fv-az1493-330:08959] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9f9b4287f3]
[fv-az1493-330:08959] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f9f9b8a4f26]
[fv-az1493-330:08959] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f9f9b8b6d9c]
[fv-az1493-330:08959] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f9f9b8b6e07]
[fv-az1493-330:08959] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9f9b8b70bb]
[fv-az1493-330:08959] [ 8] plumed(+0x12f48)[0x55e39a445f48]
[fv-az1493-330:08959] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9f9b429d90]
[fv-az1493-330:08959] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9f9b429e40]
[fv-az1493-330:08959] [11] plumed(+0x131e5)[0x55e39a4461e5]
[fv-az1493-330:08959] *** End of error message ***
</pre>
{% endraw %}
