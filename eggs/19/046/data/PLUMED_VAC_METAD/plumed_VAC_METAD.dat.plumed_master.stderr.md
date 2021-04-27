**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_VAC_METAD/plumed_VAC_METAD.dat   
(download [zipped raw stdout](plumed_VAC_METAD.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: FPS LABEL=fps REFERENCE=Faidon_new_ref.pdb LIGAND=lig ANCHOR=2481 POINTS=-0.5910,0.3486,-1.6694,-0.6214,0.5475,-1.2516
Maybe a missing space or a typo?
[fv-az99-305:37133] *** Process received signal ***
[fv-az99-305:37133] Signal: Aborted (6)
[fv-az99-305:37133] Signal code:  (-6)
[fv-az99-305:37133] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc3bd7ea210]
[fv-az99-305:37133] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc3bd7ea18b]
[fv-az99-305:37133] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc3bd7c9859]
[fv-az99-305:37133] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc3bda51951]
[fv-az99-305:37133] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc3bda5d47c]
[fv-az99-305:37133] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc3bda5d4e7]
[fv-az99-305:37133] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7fc3bda5d7ed]
[fv-az99-305:37133] [ 7] plumed_master(+0xf568)[0x562294565568]
[fv-az99-305:37133] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc3bd7cb0b3]
[fv-az99-305:37133] [ 9] plumed_master(+0xf79e)[0x56229456579e]
[fv-az99-305:37133] *** End of error message ***
</pre>
{% endraw %}
