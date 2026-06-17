**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
Download: [zipped raw stdout](plumed_FB_rewe.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_FB_rewe.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:655) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const std::string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[runnervm1li68:11383] *** Process received signal ***
[runnervm1li68:11383] Signal: Aborted (6)
[runnervm1li68:11383] Signal code:  (-6)
[runnervm1li68:11383] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7442245330]
[runnervm1li68:11383] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f744229eb2c]
[runnervm1li68:11383] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f744224527e]
[runnervm1li68:11383] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f74422288ff]
[runnervm1li68:11383] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f74426a5ff5]
[runnervm1li68:11383] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f74426bb0da]
[runnervm1li68:11383] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f74426a5a55]
[runnervm1li68:11383] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f74426a5a6f]
[runnervm1li68:11383] [ 8] plumed_master(+0x146dd)[0x5585c5ed66dd]
[runnervm1li68:11383] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f744222a1ca]
[runnervm1li68:11383] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f744222a28b]
[runnervm1li68:11383] [11] plumed_master(+0x15365)[0x5585c5ed7365]
[runnervm1li68:11383] *** End of error message ***
</pre>
{% endraw %}
