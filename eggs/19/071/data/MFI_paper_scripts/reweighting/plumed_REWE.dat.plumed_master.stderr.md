**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_REWE.dat   
Download: [zipped raw stdout](plumed_REWE.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_REWE.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:288) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az1493-330:08967] *** Process received signal ***
[fv-az1493-330:08967] Signal: Aborted (6)
[fv-az1493-330:08967] Signal code:  (-6)
[fv-az1493-330:08967] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1303c42520]
[fv-az1493-330:08967] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1303c969fc]
[fv-az1493-330:08967] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1303c42476]
[fv-az1493-330:08967] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1303c287f3]
[fv-az1493-330:08967] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f13040a4f26]
[fv-az1493-330:08967] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f13040b6d9c]
[fv-az1493-330:08967] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f13040b6e07]
[fv-az1493-330:08967] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f13040b70bb]
[fv-az1493-330:08967] [ 8] plumed_master(+0x12ebf)[0x5560d0acbebf]
[fv-az1493-330:08967] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1303c29d90]
[fv-az1493-330:08967] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1303c29e40]
[fv-az1493-330:08967] [11] plumed_master(+0x13155)[0x5560d0acc155]
[fv-az1493-330:08967] *** End of error message ***
</pre>
{% endraw %}
