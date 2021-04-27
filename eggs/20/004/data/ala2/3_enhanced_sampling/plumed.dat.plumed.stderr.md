**Project ID:** [plumID:20.004]({{ '/' | absolute_url }}eggs/20/004/)  
Stderr for source:  ala2/3_enhanced_sampling/plumed.dat   
(download [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip))  
{% raw %}
<pre>
../../code/PytorchModel.cpp:25:10: fatal error: torch/torch.h: No such file or directory
   25 | #include <torch/torch.h>
      |          ^~~~~~~~~~~~~~~
compilation terminated.
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
  what():  
+++ PLUMED error
+++ at PlumedMain.cpp:942, function void PLMD::PlumedMain::load(const string&)
+++ message follows +++
An error happened while executing command env PLUMED_ROOT="/home/runner/opt/lib/plumed" env PLUMED_HTMLDIR="/home/runner/opt/share/doc/plumed" env PLUMED_INCLUDEDIR="/home/runner/opt/include" env PLUMED_PROGRAM_NAME="plumed" env PLUMED_IS_INSTALLED="yes" "/home/runner/opt/lib/plumed"/scripts/mklib.sh ../../code/PytorchModel.cpp

[fv-az99-305:24587] *** Process received signal ***
[fv-az99-305:24587] Signal: Aborted (6)
[fv-az99-305:24587] Signal code:  (-6)
[fv-az99-305:24587] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x46210)[0x7f610f9fb210]
[fv-az99-305:24587] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f610f9fb18b]
[fv-az99-305:24587] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f610f9da859]
[fv-az99-305:24587] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e951)[0x7f610fc62951]
[fv-az99-305:24587] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa47c)[0x7f610fc6e47c]
[fv-az99-305:24587] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa4e7)[0x7f610fc6e4e7]
[fv-az99-305:24587] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa799)[0x7f610fc6e799]
[fv-az99-305:24587] [ 7] plumed(+0xf47d)[0x5617ae9a947d]
[fv-az99-305:24587] [ 8] plumed(+0x14004)[0x5617ae9ae004]
[fv-az99-305:24587] [ 9] plumed(+0xf698)[0x5617ae9a9698]
[fv-az99-305:24587] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f610f9dc0b3]
[fv-az99-305:24587] [11] plumed(+0xf76e)[0x5617ae9a976e]
[fv-az99-305:24587] *** End of error message ***
</pre>
{% endraw %}
