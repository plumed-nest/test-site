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
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az1110-714:74224] *** Process received signal ***
[fv-az1110-714:74224] Signal: Aborted (6)
[fv-az1110-714:74224] Signal code:  (-6)
[fv-az1110-714:74224] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5ff8c42520]
[fv-az1110-714:74224] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5ff8c969fc]
[fv-az1110-714:74224] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5ff8c42476]
[fv-az1110-714:74224] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5ff8c287f3]
[fv-az1110-714:74224] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5ff90a2b9e]
[fv-az1110-714:74224] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5ff90ae20c]
[fv-az1110-714:74224] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5ff90ae277]
[fv-az1110-714:74224] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5ff90ae52b]
[fv-az1110-714:74224] [ 8] plumed_master(+0x14274)[0x5561549ea274]
[fv-az1110-714:74224] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5ff8c29d90]
[fv-az1110-714:74224] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5ff8c29e40]
[fv-az1110-714:74224] [11] plumed_master(+0x14ed5)[0x5561549eaed5]
[fv-az1110-714:74224] *** End of error message ***
</pre>
{% endraw %}
