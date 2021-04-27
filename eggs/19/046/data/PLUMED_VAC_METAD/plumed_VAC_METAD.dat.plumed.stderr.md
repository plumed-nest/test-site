**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_VAC_METAD/plumed_VAC_METAD.dat   
(download [zipped raw stdout](plumed_VAC_METAD.dat.plumed.stdout.txt.zip))  
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
[fv-az99-305:37125] *** Process received signal ***
[fv-az99-305:37125] Signal: Aborted (6)
[fv-az99-305:37125] Signal code:  (-6)
[fv-az99-305:37125] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7fc4b464d210]
[fv-az99-305:37125] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7fc4b464d18b]
[fv-az99-305:37125] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7fc4b462c859]
[fv-az99-305:37125] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7fc4b48b4951]
[fv-az99-305:37125] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7fc4b48c047c]
[fv-az99-305:37125] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7fc4b48c04e7]
[fv-az99-305:37125] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7fc4b48c0799]
[fv-az99-305:37125] [ 7] plumed(+0xf47d)[0x55e19b72747d]
[fv-az99-305:37125] [ 8] plumed(+0x14004)[0x55e19b72c004]
[fv-az99-305:37125] [ 9] plumed(+0xf698)[0x55e19b727698]
[fv-az99-305:37125] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7fc4b462e0b3]
[fv-az99-305:37125] [11] plumed(+0xf76e)[0x55e19b72776e]
[fv-az99-305:37125] *** End of error message ***
</pre>
{% endraw %}
