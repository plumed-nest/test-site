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
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : cannot understand the following words from the input line : REWEIGHTING_NGRID=200, REWEIGHTING_NHILLS=10
[fv-az1947-39:13897] *** Process received signal ***
[fv-az1947-39:13897] Signal: Aborted (6)
[fv-az1947-39:13897] Signal code:  (-6)
[fv-az1947-39:13897] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f690e645330]
[fv-az1947-39:13897] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f690e69eb2c]
[fv-az1947-39:13897] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f690e64527e]
[fv-az1947-39:13897] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f690e6288ff]
[fv-az1947-39:13897] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f690eaa5ff5]
[fv-az1947-39:13897] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f690eabb0da]
[fv-az1947-39:13897] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f690eaa5a55]
[fv-az1947-39:13897] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f690eaa5a6f]
[fv-az1947-39:13897] [ 8] plumed(+0x146dd)[0x559af427e6dd]
[fv-az1947-39:13897] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f690e62a1ca]
[fv-az1947-39:13897] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f690e62a28b]
[fv-az1947-39:13897] [11] plumed(+0x15365)[0x559af427f365]
[fv-az1947-39:13897] *** End of error message ***
</pre>
{% endraw %}
