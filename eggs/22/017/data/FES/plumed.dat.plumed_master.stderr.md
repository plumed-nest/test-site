**Project ID:** [plumID:22.017]({{ '/' | absolute_url }}eggs/22/017/)  
Stderr for source:  FES/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'std::runtime_error'
what():  The following operation failed in the TorchScript interpreter.
Traceback of TorchScript, serialized code (most recent call last):
File "code/__torch__/mlcvs/tica/___torch_mangle_30.py", line 30, in forward
_9 = int(x_size0)
_10 = int(x_size0)
Mean_0 = torch.expand(torch.unsqueeze(CONSTANTS.c2, 0), [_8, _10], implicit=False)
~~~~~~~~~~~~ <--- HERE
Range_0 = torch.expand(torch.unsqueeze(CONSTANTS.c3, 0), [_7, _9], implicit=False)
_11 = torch.div(torch.sub(x2, Mean_0, alpha=1), Range_0)

Traceback of TorchScript, original code (most recent call last):
/home/nansari@iit.local/Trypsin/DEEPTICA/mlcvs/nncv.py(86): _normalize
/home/nansari@iit.local/Trypsin/DEEPTICA/mlcvs/tica.py(191): forward
/home/nansari@iit.local/.local/lib/python3.8/site-packages/torch/nn/modules/module.py(534): _slow_forward
/home/nansari@iit.local/.local/lib/python3.8/site-packages/torch/nn/modules/module.py(548): __call__
/home/nansari@iit.local/.local/lib/python3.8/site-packages/torch/jit/__init__.py(1027): trace_module
/home/nansari@iit.local/.local/lib/python3.8/site-packages/torch/jit/__init__.py(873): trace
/home/nansari@iit.local/Trypsin/DEEPTICA/mlcvs/tica.py(454): export
/tmp/ipykernel_2298779/2827124850.py(6): <module>
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/interactiveshell.py(3251): run_code
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/interactiveshell.py(3191): run_ast_nodes
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/interactiveshell.py(3012): run_cell_async
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/async_helpers.py(129): _pseudo_sync_runner
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/interactiveshell.py(2814): _run_cell
/home/nansari@iit.local/.local/lib/python3.8/site-packages/IPython/core/interactiveshell.py(2768): run_cell
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/zmqshell.py(532): run_cell
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/ipkernel.py(353): do_execute
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/kernelbase.py(652): execute_request
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/kernelbase.py(357): dispatch_shell
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/kernelbase.py(450): process_one
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/kernelbase.py(461): dispatch_queue
/usr/lib/python3.8/asyncio/events.py(81): _run
/usr/lib/python3.8/asyncio/base_events.py(1859): _run_once
/usr/lib/python3.8/asyncio/base_events.py(570): run_forever
/home/nansari@iit.local/.local/lib/python3.8/site-packages/tornado/platform/asyncio.py(199): start
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel/kernelapp.py(677): start
/home/nansari@iit.local/.local/lib/python3.8/site-packages/traitlets/config/application.py(846): launch_instance
/home/nansari@iit.local/.local/lib/python3.8/site-packages/ipykernel_launcher.py(16): <module>
/usr/lib/python3.8/runpy.py(87): _run_code
/usr/lib/python3.8/runpy.py(194): _run_module_as_main
RuntimeError: The expanded size of the tensor (5) must match the existing size (3) at non-singleton dimension 1.  Target sizes: [18, 5].  Tensor sizes: [1, 3]

[fv-az532-512:07331] *** Process received signal ***
[fv-az532-512:07331] Signal: Aborted (6)
[fv-az532-512:07331] Signal code:  (-6)
[fv-az532-512:07331] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fca28e42520]
[fv-az532-512:07331] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fca28e969fc]
[fv-az532-512:07331] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fca28e42476]
[fv-az532-512:07331] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fca28e287f3]
[fv-az532-512:07331] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fca292a4f26]
[fv-az532-512:07331] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fca292b6d9c]
[fv-az532-512:07331] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fca292b6e07]
[fv-az532-512:07331] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fca292b70bb]
[fv-az532-512:07331] [ 8] plumed_master(+0x12ebf)[0x55c26d77cebf]
[fv-az532-512:07331] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fca28e29d90]
[fv-az532-512:07331] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fca28e29e40]
[fv-az532-512:07331] [11] plumed_master(+0x13155)[0x55c26d77d155]
[fv-az532-512:07331] *** End of error message ***
</pre>
{% endraw %}
