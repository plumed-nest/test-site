**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_FM/plumed_FM.dat   
(download [zipped raw stdout](plumed_FM.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:706, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: FPS LABEL=fps REFERENCE=Faidon_new_ref.pdb LIGAND=lig ANCHOR=2481 POINTS=-0.5910,0.3486,-1.6694,-0.6214,0.5475,-1.2516
Maybe a missing space or a typo?
[fv-az99-305:37077] *** Process received signal ***
[fv-az99-305:37077] Signal: Aborted (6)
[fv-az99-305:37077] Signal code:  (-6)
[fv-az99-305:37077] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fa75666f210]
[fv-az99-305:37077] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fa75666f18b]
[fv-az99-305:37077] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fa75664e859]
[fv-az99-305:37077] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fa7568d6951]
[fv-az99-305:37077] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fa7568e247c]
[fv-az99-305:37077] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fa7568e24e7]
[fv-az99-305:37077] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fa7568e2799]
[fv-az99-305:37077] [ 7] plumed(+0xf47d)[0x557b6a1b247d]
[fv-az99-305:37077] [ 8] plumed(+0x14004)[0x557b6a1b7004]
[fv-az99-305:37077] [ 9] plumed(+0xf698)[0x557b6a1b2698]
[fv-az99-305:37077] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fa7566500b3]
[fv-az99-305:37077] [11] plumed(+0xf76e)[0x557b6a1b276e]
[fv-az99-305:37077] *** End of error message ***
</pre>
{% endraw %}
