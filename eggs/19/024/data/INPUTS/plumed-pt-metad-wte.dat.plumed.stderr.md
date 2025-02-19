**Project ID:** [plumID:19.024]({{ '/' | absolute_url }}eggs/19/024/)  
Stderr for source:  INPUTS/plumed-pt-metad-wte.dat   
Download: [zipped raw stdout](plumed-pt-metad-wte.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed-pt-metad-wte.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/Grid.cpp:655) static std::unique_ptr<PLMD::GridBase> PLMD::GridBase::create(const std::string&, const std::vector<PLMD::Value*>&, PLMD::IFile&, bool, bool, bool)
+++ assertion failed: ifile.FieldExist( funcl )
no column labelled @6.bias in in grid input
[fv-az1436-30:13320] *** Process received signal ***
[fv-az1436-30:13320] Signal: Aborted (6)
[fv-az1436-30:13320] Signal code:  (-6)
[fv-az1436-30:13320] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc695445330]
[fv-az1436-30:13320] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc69549eb2c]
[fv-az1436-30:13320] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc69544527e]
[fv-az1436-30:13320] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc6954288ff]
[fv-az1436-30:13320] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc6958a5ff5]
[fv-az1436-30:13320] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc6958bb0da]
[fv-az1436-30:13320] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc6958a5a55]
[fv-az1436-30:13320] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc6958a5a6f]
[fv-az1436-30:13320] [ 8] plumed(+0x146dd)[0x561b50cee6dd]
[fv-az1436-30:13320] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc69542a1ca]
[fv-az1436-30:13320] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc69542a28b]
[fv-az1436-30:13320] [11] plumed(+0x15365)[0x561b50cef365]
[fv-az1436-30:13320] *** End of error message ***
</pre>
{% endraw %}
