**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
Download: [zipped raw stdout](plumed_FB_rewe.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_FB_rewe.dat.plumed.stderr.txt.zip) 
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
[runnervm1li68:11367] *** Process received signal ***
[runnervm1li68:11367] Signal: Aborted (6)
[runnervm1li68:11367] Signal code:  (-6)
[runnervm1li68:11367] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f85d4445330]
[runnervm1li68:11367] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f85d449eb2c]
[runnervm1li68:11367] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f85d444527e]
[runnervm1li68:11367] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f85d44288ff]
[runnervm1li68:11367] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f85d48a5ff5]
[runnervm1li68:11367] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f85d48bb0da]
[runnervm1li68:11367] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f85d48a5a55]
[runnervm1li68:11367] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f85d48a5a6f]
[runnervm1li68:11367] [ 8] plumed(+0x146dd)[0x5559300c96dd]
[runnervm1li68:11367] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f85d442a1ca]
[runnervm1li68:11367] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f85d442a28b]
[runnervm1li68:11367] [11] plumed(+0x15365)[0x5559300ca365]
[runnervm1li68:11367] *** End of error message ***
</pre>
{% endraw %}
