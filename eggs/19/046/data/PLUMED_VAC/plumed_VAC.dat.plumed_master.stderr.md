**Project ID:** [plumID:19.046]({{ '/' | absolute_url }}eggs/19/046/)  
Stderr for source:  PLUMED_VAC/plumed_VAC.dat   
(download [zipped raw stdout](plumed_VAC.dat.plumed_master.stdout.txt.zip))  
{% raw %}
<pre>
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:704, function void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
+++ message follows +++
ERROR
I cannot understand line: TICA ARG=Prot_norm,wBpock_norm,ab_t,lig_OW_large_norm EIGEN_NUMBERS=4 LAGGED_TIME=150000 TAU_NUMBER=5000 STEP_SIZE=0.5 LOGWEIGHTS=rw
Maybe a missing space or a typo?
[fv-az99-305:37109] *** Process received signal ***
[fv-az99-305:37109] Signal: Aborted (6)
[fv-az99-305:37109] Signal code:  (-6)
[fv-az99-305:37109] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f09ce1b8210]
[fv-az99-305:37109] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f09ce1b818b]
[fv-az99-305:37109] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f09ce197859]
[fv-az99-305:37109] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f09ce41f951]
[fv-az99-305:37109] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f09ce42b47c]
[fv-az99-305:37109] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f09ce42b4e7]
[fv-az99-305:37109] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f09ce42b7ed]
[fv-az99-305:37109] [ 7] plumed_master(+0xf568)[0x55e237159568]
[fv-az99-305:37109] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f09ce1990b3]
[fv-az99-305:37109] [ 9] plumed_master(+0xf79e)[0x55e23715979e]
[fv-az99-305:37109] *** End of error message ***
</pre>
{% endraw %}
