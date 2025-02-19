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
(tools/Grid.cpp:655) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const std::string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled metad.bias in in grid input
[fv-az1947-39:13845] *** Process received signal ***
[fv-az1947-39:13845] Signal: Aborted (6)
[fv-az1947-39:13845] Signal code:  (-6)
[fv-az1947-39:13845] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3723e45330]
[fv-az1947-39:13845] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3723e9eb2c]
[fv-az1947-39:13845] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3723e4527e]
[fv-az1947-39:13845] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3723e288ff]
[fv-az1947-39:13845] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f37242a5ff5]
[fv-az1947-39:13845] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f37242bb0da]
[fv-az1947-39:13845] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f37242a5a55]
[fv-az1947-39:13845] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f37242a5a6f]
[fv-az1947-39:13845] [ 8] plumed(+0x146dd)[0x55de9402a6dd]
[fv-az1947-39:13845] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3723e2a1ca]
[fv-az1947-39:13845] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3723e2a28b]
[fv-az1947-39:13845] [11] plumed(+0x15365)[0x55de9402b365]
[fv-az1947-39:13845] *** End of error message ***
</pre>
{% endraw %}
