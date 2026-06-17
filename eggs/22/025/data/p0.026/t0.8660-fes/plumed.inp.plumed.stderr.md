**Project ID:** [plumID:22.025]({{ '/' | absolute_url }}eggs/22/025/)  
Stderr for source:  p0.026/t0.8660-fes/plumed.inp   
Download: [zipped raw stdout](plumed.inp.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.inp.plumed.stderr.txt.zip) 
{% raw %}
<pre style="overflow:scroll;">
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
Assembler messages:
Fatal error: can't create plumed_mklib.12QwwI/../../code/ReweightGeomFES.o: No such file or directory
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1494) void PLMD::PlumedMain::load(const std::string&)
An error happened while executing command env PLUMED_ROOT='/home/runner/opt/lib/plumed' PLUMED_VERSION='2.10.0' PLUMED_HTMLDIR='/home/runner/opt/share/doc/plumed' PLUMED_INCLUDEDIR='/home/runner/opt/include' PLUMED_PROGRAM_NAME='plumed' PLUMED_IS_INSTALLED='yes' "/home/runner/opt/lib/plumed"/scripts/mklib.sh -n -o ./../../code/ReweightGeomFES.2.10.0.so ../../code/ReweightGeomFES.cpp

[runnervm7b5n9:07209] *** Process received signal ***
[runnervm7b5n9:07209] Signal: Aborted (6)
[runnervm7b5n9:07209] Signal code:  (-6)
[runnervm7b5n9:07209] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1b49045330]
[runnervm7b5n9:07209] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1b4909eb2c]
[runnervm7b5n9:07209] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1b4904527e]
[runnervm7b5n9:07209] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1b490288ff]
[runnervm7b5n9:07209] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1b494a5ff5]
[runnervm7b5n9:07209] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1b494bb0da]
[runnervm7b5n9:07209] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1b494a5a55]
[runnervm7b5n9:07209] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1b494a5a6f]
[runnervm7b5n9:07209] [ 8] plumed(+0x146dd)[0x55f374ec26dd]
[runnervm7b5n9:07209] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1b4902a1ca]
[runnervm7b5n9:07209] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1b4902a28b]
[runnervm7b5n9:07209] [11] plumed(+0x15365)[0x55f374ec3365]
[runnervm7b5n9:07209] *** End of error message ***
</pre>
{% endraw %}
