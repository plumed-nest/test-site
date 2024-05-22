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
(core/Action.cpp:305) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az1435-553:43997] *** Process received signal ***
[fv-az1435-553:43997] Signal: Aborted (6)
[fv-az1435-553:43997] Signal code:  (-6)
[fv-az1435-553:43997] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0ff8a42520]
[fv-az1435-553:43997] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0ff8a969fc]
[fv-az1435-553:43997] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0ff8a42476]
[fv-az1435-553:43997] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0ff8a287f3]
[fv-az1435-553:43997] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0ff8ea2b9e]
[fv-az1435-553:43997] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0ff8eae20c]
[fv-az1435-553:43997] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0ff8eae277]
[fv-az1435-553:43997] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0ff8eae52b]
[fv-az1435-553:43997] [ 8] plumed_master(+0x14274)[0x558987ced274]
[fv-az1435-553:43997] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0ff8a29d90]
[fv-az1435-553:43997] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0ff8a29e40]
[fv-az1435-553:43997] [11] plumed_master(+0x14ed5)[0x558987ceded5]
[fv-az1435-553:43997] *** End of error message ***
</pre>
{% endraw %}
