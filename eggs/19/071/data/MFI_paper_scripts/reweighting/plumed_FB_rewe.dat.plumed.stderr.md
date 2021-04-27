**Project ID:** [plumID:19.071]({{ '/' | absolute_url }}eggs/19/071/)  
Stderr for source:  MFI_paper_scripts/reweighting/plumed_FB_rewe.dat   
(download [zipped raw stdout](plumed_FB_rewe.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at Grid.cpp:575, function static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
+++ message follows +++
no column labelled metad.bias in in grid input
[fv-az99-305:31647] *** Process received signal ***
[fv-az99-305:31647] Signal: Aborted (6)
[fv-az99-305:31647] Signal code:  (-6)
[fv-az99-305:31647] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fccd3276210]
[fv-az99-305:31647] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fccd327618b]
[fv-az99-305:31647] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fccd3255859]
[fv-az99-305:31647] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fccd34dd951]
[fv-az99-305:31647] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fccd34e947c]
[fv-az99-305:31647] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fccd34e94e7]
[fv-az99-305:31647] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fccd34e9799]
[fv-az99-305:31647] [ 7] plumed(+0xf47d)[0x55af32e2647d]
[fv-az99-305:31647] [ 8] plumed(+0x14004)[0x55af32e2b004]
[fv-az99-305:31647] [ 9] plumed(+0xf698)[0x55af32e26698]
[fv-az99-305:31647] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fccd32570b3]
[fv-az99-305:31647] [11] plumed(+0xf76e)[0x55af32e2676e]
[fv-az99-305:31647] *** End of error message ***
</pre>
{% endraw %}
