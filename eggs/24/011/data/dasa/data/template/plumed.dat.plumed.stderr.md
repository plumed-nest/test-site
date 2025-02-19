**Project ID:** [plumID:24.011]({{ '/' | absolute_url }}eggs/24/011/)  
Stderr for source:  dasa/data/template/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: using a legacy ActionRegister.h include path, please use <<#include "core/ActionRegister.h">>
In file included from /home/runner/opt/libtorch/include/ATen/ATen.h:7,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/types.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader_options.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader/base.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader/stateful.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/all.h:8,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/torch.h:3,
from ./pytorch_model_bias.VBWclW.cpp:28:
/home/runner/opt/libtorch/include/c10/core/Allocator.h:163:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
163 |     AT_ASSERT(dptr.get() == dptr.get_context());
|                                               ^
/home/runner/opt/libtorch/include/c10/core/Allocator.h:168:16: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
168 |     AT_ASSERT(d);
|                ^
In file included from /home/runner/opt/libtorch/include/c10/core/Backend.h:5,
from /home/runner/opt/libtorch/include/c10/core/Layout.h:3,
from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:4,
from /home/runner/opt/libtorch/include/ATen/Tensor.h:3,
from /home/runner/opt/libtorch/include/ATen/Context.h:4,
from /home/runner/opt/libtorch/include/ATen/ATen.h:9:
/home/runner/opt/libtorch/include/c10/core/DispatchKeySet.h:65:65: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
65 |     TORCH_INTERNAL_ASSERT_DEBUG_ONLY(t != DispatchKey::Undefined);
|                                                                 ^
/home/runner/opt/libtorch/include/c10/core/DispatchKeySet.h:142:85: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
142 |       TORCH_INTERNAL_ASSERT(i_ <= static_cast<uint8_t>(DispatchKey::NumDispatchKeys));
|                                                                                     ^
In file included from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:7:
/home/runner/opt/libtorch/include/c10/core/Stream.h:132:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
132 |     TORCH_CHECK(isValidDeviceType(device_type));
|                                               ^
In file included from /home/runner/opt/libtorch/include/c10/core/Storage.h:3,
from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:11:
/home/runner/opt/libtorch/include/c10/core/StorageImpl.h:132:27: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
132 |       AT_ASSERT(allocator_);
|                           ^
In file included from /home/runner/opt/libtorch/include/c10/core/TensorImpl.h:14,
from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:13:
/home/runner/opt/libtorch/include/c10/core/impl/SizesAndStrides.h:261:52: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
261 |     TORCH_INTERNAL_ASSERT_DEBUG_ONLY(rhs.isInline());
|                                                    ^
/home/runner/opt/libtorch/include/c10/core/impl/SizesAndStrides.h:275:49: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
275 |     TORCH_INTERNAL_ASSERT_DEBUG_ONLY(!isInline());
|                                                 ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:68:41: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
68 |   TORCH_CHECK((unsigned)k <= dims.size());
|                                         ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:78:40: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
78 |   TORCH_CHECK((unsigned)l < dims.size());
|                                        ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:94:35: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
94 |   TORCH_CHECK(axis_index >= -ndims);
|                                   ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:95:33: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
95 |   TORCH_CHECK(axis_index < ndims);
|                                 ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:607:37: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
607 |     TORCH_INTERNAL_ASSERT(dim() == 0);
|                                     ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:1106:48: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1106 |     TORCH_CHECK(sizes_and_strides_.size() >= 1u);
|                                                ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:1252:25: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1252 |       TORCH_CHECK(d >= 0);
|                         ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:1380:51: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1380 |         TORCH_INTERNAL_ASSERT(storage_offset_ == 0); // because we just reallocated
|                                                   ^
/home/runner/opt/libtorch/include/c10/core/TensorImpl.h:1407:49: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1407 |       TORCH_INTERNAL_ASSERT(storage_offset_ == 0); // because we just reallocated
|                                                 ^
In file included from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:21:
/home/runner/opt/libtorch/include/ATen/core/DeprecatedTypeProperties.h:107:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
107 |       AT_ASSERT(device.type() == device_type());
|                                               ^
In file included from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:22:
/home/runner/opt/libtorch/include/ATen/core/NamedTensor.h:51:98: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
51 |       std::any_of(names_.begin(), names_.end(), [](const Dimname& n) { return !n.isWildcard(); }));
|                                                                                                  ^
/home/runner/opt/libtorch/include/ATen/core/NamedTensor.h:55:60: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
55 |     TORCH_INTERNAL_ASSERT(new_names.size() == names_.size());
|                                                            ^
/home/runner/opt/libtorch/include/ATen/core/NamedTensor.h:61:60: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
61 |     TORCH_INTERNAL_ASSERT(new_names.size() == names_.size());
|                                                            ^
/home/runner/opt/libtorch/include/ATen/core/NamedTensor.h:90:38: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
90 |     TORCH_INTERNAL_ASSERT(initialized);
|                                      ^
/home/runner/opt/libtorch/include/ATen/core/TensorBody.h:64:113: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
64 |   TORCH_INTERNAL_ASSERT_DEBUG_ONLY(!c10::impl::tls_local_dispatch_key_set().excluded_.has(DispatchKey::Autograd));
|                                                                                                                 ^
In file included from /home/runner/opt/libtorch/include/ATen/Context.h:9:
/home/runner/opt/libtorch/include/ATen/core/LegacyTypeDispatch.h:52:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
52 |     TORCH_INTERNAL_ASSERT(enabled);
|                                  ^
In file included from /home/runner/opt/libtorch/include/c10/core/DeviceGuard.h:3,
from /home/runner/opt/libtorch/include/ATen/DeviceGuard.h:3,
from /home/runner/opt/libtorch/include/ATen/ATen.h:11:
/home/runner/opt/libtorch/include/c10/core/impl/InlineDeviceGuard.h:109:46: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
109 |               device.type() == U::static_type);
|                                              ^
/home/runner/opt/libtorch/include/c10/core/impl/InlineDeviceGuard.h:148:65: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
148 |       AT_ASSERT(impl == nullptr || impl->type() == device.type());
|                                                                 ^
In file included from /home/runner/opt/libtorch/include/ATen/record_function.h:3,
from /home/runner/opt/libtorch/include/ATen/Dispatch.h:5,
from /home/runner/opt/libtorch/include/ATen/ATen.h:13:
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:302:35: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
302 |     AT_ASSERT(rhs.is_intrusive_ptr);
|                                   ^
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:456:25: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
456 |     AT_ASSERT(isDouble());
|                         ^
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:503:22: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
503 |     AT_ASSERT(isInt());
|                      ^
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:522:23: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
522 |     AT_ASSERT(isBool());
|                       ^
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:650:23: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
650 |     AT_ASSERT(isNone());
|                       ^
/home/runner/opt/libtorch/include/ATen/core/ivalue.h:694:25: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
694 |     AT_ASSERT(isDevice());
|                         ^
In file included from /home/runner/opt/libtorch/include/ATen/core/List_inl.h:3,
from /home/runner/opt/libtorch/include/ATen/core/List.h:486,
from /home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:7,
from /home/runner/opt/libtorch/include/ATen/core/ivalue.h:1138:
/home/runner/opt/libtorch/include/ATen/core/jit_type_base.h:172:16: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
172 |     AT_ASSERT(r);
|                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type_base.h:178:16: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
178 |     AT_ASSERT(r);
|                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type_base.h:184:16: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
184 |     AT_ASSERT(r);
|                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type_base.h:190:16: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
190 |     AT_ASSERT(r);
|                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type_base.h:206:65: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
206 |     AT_ASSERT(current_contained.size() == contained_types.size());
|                                                                 ^
In file included from /home/runner/opt/libtorch/include/ATen/core/jit_type.h:7,
from /home/runner/opt/libtorch/include/ATen/core/List_inl.h:366:
/home/runner/opt/libtorch/include/ATen/core/qualified_name.h:16:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
16 |     TORCH_CHECK(!name.empty());
|                              ^
/home/runner/opt/libtorch/include/ATen/core/qualified_name.h:54:40: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
54 |     TORCH_INTERNAL_ASSERT(!name.empty());
|                                        ^
/home/runner/opt/libtorch/include/ATen/core/qualified_name.h:55:69: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
55 |     TORCH_INTERNAL_ASSERT(name.find(delimiter_) == std::string::npos);
|                                                                     ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:129:42: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
129 |     AT_ASSERT(contained_types.size() == 1);
|                                          ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:243:28: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
243 |     TORCH_CHECK(is_static());
|                            ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:572:63: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
572 |     TORCH_INTERNAL_ASSERT(sizes().concrete_sizes().has_value());
|                                                               ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:1950:40: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1950 |     AT_ASSERT(slot < attributes_.size());
|                                        ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:1955:40: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1955 |     AT_ASSERT(slot < attributes_.size());
|                                        ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2064:64: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2064 |     TORCH_CHECK(constantNames_.size() == constantValues_.size());
|                                                                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2088:64: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2088 |     TORCH_CHECK(constantNames_.size() == constantValues_.size());
|                                                                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2089:45: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2089 |     TORCH_CHECK(slot < constantNames_.size());
|                                             ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2104:74: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2104 |     TORCH_INTERNAL_ASSERT(constantNames_.size() == constantValues_.size());
|                                                                          ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2126:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2126 |     AT_ASSERT(numAttributes() == contained_types.size());
|                                                        ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2128:74: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2128 |       AT_ASSERT(attributes_[i].getType()->isSubtypeOf(contained_types[i]));
|                                                                          ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2482:32: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2482 |     TORCH_INTERNAL_ASSERT(type_);
|                                ^
/home/runner/opt/libtorch/include/ATen/core/jit_type.h:2489:33: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
2489 |     TORCH_INTERNAL_ASSERT(!type_);
|                                 ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:189:36: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
189 |   TORCH_INTERNAL_ASSERT(isCapsule());
|                                    ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:193:36: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
193 |   TORCH_INTERNAL_ASSERT(isCapsule());
|                                    ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:405:26: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
405 |     AT_ASSERT(completed());
|                          ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:416:26: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
416 |     AT_ASSERT(completed());
|                          ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:417:21: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
417 |     AT_ASSERT(!eptr_);
|                     ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:534:27: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
534 |     AT_ASSERT(!completed());
|                           ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:612:58: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
612 |     TORCH_INTERNAL_ASSERT_DEBUG_ONLY(slot < slots_.size());
|                                                          ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:619:37: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
619 |     TORCH_CHECK(slot < slots_.size());
|                                     ^
/home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:986:45: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
986 |   TORCH_CHECK(vals.size() == sizeof...(Args));
|                                             ^
In file included from /home/runner/opt/libtorch/include/ATen/ATen.h:17:
/home/runner/opt/libtorch/include/ATen/ScalarOps.h:34:36: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
34 |       AT_ASSERT(s.isIntegral(false));
|                                    ^
/home/runner/opt/libtorch/include/ATen/ScalarOps.h:45:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
45 |     AT_ASSERT(s.isIntegral(false));
|                                  ^
In file included from /home/runner/opt/libtorch/include/ATen/MetaFunctions.h:6,
from /home/runner/opt/libtorch/include/ATen/NativeFunctions.h:6,
from /home/runner/opt/libtorch/include/ATen/TensorIndexing.h:11,
from /home/runner/opt/libtorch/include/ATen/ATen.h:20:
/home/runner/opt/libtorch/include/ATen/TensorIterator.h:209:33: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
209 |     AT_ASSERT(arg < num_outputs_);
|                                 ^
/home/runner/opt/libtorch/include/ATen/TensorIterator.h:218:58: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
218 |     AT_ASSERT(arg >= 0 && arg < ntensors() - num_outputs_);
|                                                          ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/autograd/generated/variable_factories.h:11,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/types.h:7:
/home/runner/opt/libtorch/include/torch/csrc/autograd/variable.h:268:38: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
268 |       TORCH_INTERNAL_ASSERT(self_impl);
|                                      ^
In file included from /home/runner/opt/libtorch/include/ATen/core/function_schema.h:7,
from /home/runner/opt/libtorch/include/ATen/core/function.h:2,
from /home/runner/opt/libtorch/include/torch/csrc/jit/api/method.h:2,
from /home/runner/opt/libtorch/include/torch/csrc/jit/api/object.h:5,
from /home/runner/opt/libtorch/include/torch/csrc/jit/frontend/tracer.h:9,
from /home/runner/opt/libtorch/include/torch/csrc/autograd/generated/variable_factories.h:12:
/home/runner/opt/libtorch/include/ATen/core/alias_info.h:51:38: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
51 |     AT_ASSERT(beforeSets_.size() == 1);
|                                      ^
/home/runner/opt/libtorch/include/ATen/core/function_schema.h:58:32: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
58 |     TORCH_INTERNAL_ASSERT(type_);
|                                ^
In file included from /home/runner/opt/libtorch/include/ATen/core/function_schema.h:429:
/home/runner/opt/libtorch/include/ATen/core/function_schema_inl.h:189:42: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
189 |       AT_ASSERT(!argument.default_value());
|                                          ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/jit/api/function_impl.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/jit/api/method.h:5:
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/attributes.h:38:58: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
38 |   AT_ASSERT(size_t(kind) < sizeof(names) / sizeof(*names));
|                                                          ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:4:
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/graph_node_list.h:76:18: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
76 |     AT_ASSERT(cur);
|                  ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/graph_node_list.h:86:18: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
86 |     AT_ASSERT(cur);
|                  ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:5:
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/named_value.h:64:20: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
64 |     AT_ASSERT(name_);
|                    ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/named_value.h:69:19: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
69 |     AT_ASSERT(loc_);
|                   ^
In file included from /home/runner/opt/libtorch/include/ATen/core/dispatch/OperatorEntry.h:11,
from /home/runner/opt/libtorch/include/ATen/core/dispatch/Dispatcher.h:6,
from /home/runner/opt/libtorch/include/torch/csrc/jit/runtime/operator.h:6,
from /home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:7:
/home/runner/opt/libtorch/include/ATen/core/dispatch/DispatchKeyExtractor.h:116:76: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
116 |     TORCH_INTERNAL_ASSERT(dispatch_arg_indices_reverse_.is_entirely_unset());
|                                                                            ^
/home/runner/opt/libtorch/include/ATen/core/dispatch/OperatorEntry.h:78:46: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
78 |     TORCH_INTERNAL_ASSERT(schema_.has_value());
|                                              ^
/home/runner/opt/libtorch/include/ATen/core/dispatch/OperatorEntry.h:141:46: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
141 |     TORCH_INTERNAL_ASSERT(schema_.has_value());
|                                              ^
/home/runner/opt/libtorch/include/ATen/core/dispatch/Dispatcher.h:384:73: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
384 |   TORCH_INTERNAL_ASSERT_DEBUG_ONLY(!c10::isAliasDispatchKey(dispatchKey));
|                                                                         ^
In file included from /home/runner/opt/libtorch/include/torch/custom_class.h:4,
from /home/runner/opt/libtorch/include/torch/library.h:822,
from /home/runner/opt/libtorch/include/torch/csrc/jit/runtime/operator.h:13:
/home/runner/opt/libtorch/include/ATen/core/builtin_function.h:23:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
23 |     TORCH_INTERNAL_ASSERT(schema_.returns().size() == 1);
|                                                        ^
/home/runner/opt/libtorch/include/ATen/core/builtin_function.h:104:46: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
104 |     TORCH_CHECK(schema_.returns().size() == 1);
|                                              ^
/home/runner/opt/libtorch/include/ATen/core/builtin_function.h:113:32: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
113 |     TORCH_INTERNAL_ASSERT(false);
|                                ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:192:31: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
192 |     AT_ASSERT(type_ != nullptr);
|                               ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:443:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
443 |     AT_ASSERT(inputs_.size() == 1);
|                                  ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:447:35: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
447 |     AT_ASSERT(outputs_.size() == 1);
|                                   ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:451:35: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
451 |     AT_ASSERT(outputs_.size() == 1);
|                                   ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:455:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
455 |     AT_ASSERT(inputs_.size() == 1);
|                                  ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:748:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
748 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:755:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
755 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:762:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
762 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:847:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
847 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:859:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
859 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:873:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
873 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:880:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
880 |     AT_ASSERT(!required || it != values_.end());
|                                               ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:885:29: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
885 |     AT_ASSERT(name.is_attr());
|                             ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:892:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
892 |     AT_ASSERT(!required || it != values_.end());
|                                               ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:911:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
911 |       AT_ASSERT(prev() == nullptr);
|                                  ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1024:55: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1024 |     AT_ASSERT(n->graph_ == graph_ && !n->inBlockList());
|                                                       ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1029:55: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1029 |     AT_ASSERT(n->graph_ == graph_ && !n->inBlockList());
|                                                       ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1280:57: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1280 |         "insert point node is no longer in a block list");
|                                                         ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1285:39: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1285 |     AT_ASSERT(b->owningGraph() == this);
|                                       ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1292:59: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1292 |     AT_ASSERT(n->owningGraph() == this && n->inBlockList());
|                                                           ^
/home/runner/opt/libtorch/include/torch/csrc/jit/ir/ir.h:1380:17: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
1380 |   AT_ASSERT(type);
|                 ^
/home/runner/opt/libtorch/include/torch/csrc/jit/api/function_impl.h:82:22: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
82 |     AT_ASSERT(schema_);
|                      ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/detail/data_shuttle.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader/base.h:4:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/detail/queue.h:57:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
57 |     AT_ASSERT(!queue_.empty());
|                              ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader/base.h:5:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/detail/sequencers.h:82:59: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
82 |         AT_ASSERT(!detail::buffer_contains_result(buffer_));
|                                                           ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/detail/sequencers.h:92:61: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
92 |       AT_ASSERT(!buffer(result->sequence_number).has_value());
|                                                             ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader.h:4:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/dataloader/stateless.h:74:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
74 |     AT_ASSERT(indices->size() > 0);
|                                  ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/jit/api/module.h:14,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/serialize/input-archive.h:7,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/serialize/archive.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/samplers/serialize.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/samplers.h:8,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets/chunk.h:6,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data.h:4:
/home/runner/opt/libtorch/include/torch/csrc/jit/api/compilation_unit.h:229:50: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
229 |           TORCH_INTERNAL_ASSERT(it != dict_.end());
|                                                  ^
/home/runner/opt/libtorch/include/torch/csrc/jit/api/compilation_unit.h:338:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
338 |     TORCH_INTERNAL_ASSERT(cu_);
|                              ^
/home/runner/opt/libtorch/include/torch/csrc/jit/api/compilation_unit.h:339:36: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
339 |     TORCH_INTERNAL_ASSERT(function_);
|                                    ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets/chunk.h:75:22: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
75 |       AT_ASSERT(stop_);
|                      ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets/chunk.h:116:64: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
116 |           batch_example_indices.value().size() == example_count);
|                                                                ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets/chunk.h:395:39: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
395 |     AT_ASSERT(running_preloaders_ == 0);
|                                       ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/data/datasets/chunk.h:454:45: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
454 |     AT_ASSERT(running_preloaders_.load() > 0);
|                                             ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/module.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/cloneable.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/all.h:13:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/container/any_module_holder.h:43:42: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
43 |       AT_ASSERT(index < arguments_.size());
|                                          ^
In file included from /home/runner/opt/libtorch/include/ATen/Parallel.h:140,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/utils.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/cloneable.h:5:
/home/runner/opt/libtorch/include/ATen/ParallelOpenMP.h:20:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
20 |   TORCH_CHECK(grain_size >= 0);
|                              ^
/home/runner/opt/libtorch/include/ATen/ParallelOpenMP.h:71:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
71 |   TORCH_CHECK(grain_size >= 0);
|                              ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/loss.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional.h:10,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn.h:4:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:607:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
607 |   TORCH_INTERNAL_ASSERT(embed_dim == embed_dim_to_check);
|                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:608:53: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
608 |   TORCH_INTERNAL_ASSERT(key.sizes() == value.sizes());
|                                                     ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:637:47: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
637 |         TORCH_INTERNAL_ASSERT(!value.defined());
|                                               ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:687:60: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
687 |     TORCH_CHECK(len1 == embed_dim && len2 == query.size(-1));
|                                                            ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:693:58: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
693 |     TORCH_CHECK(len1 == embed_dim && len2 == key.size(-1));
|                                                          ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:699:60: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
699 |     TORCH_CHECK(len1 == embed_dim && len2 == value.size(-1));
|                                                            ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:742:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
742 |     TORCH_CHECK(!bias_k.defined());
|                                  ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:743:34: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
743 |     TORCH_CHECK(!bias_v.defined());
|                                  ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:753:52: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
753 |     TORCH_CHECK(static_k.size(0) == bsz * num_heads);
|                                                    ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:754:45: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
754 |     TORCH_CHECK(static_k.size(2) == head_dim);
|                                             ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:758:52: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
758 |     TORCH_CHECK(static_v.size(0) == bsz * num_heads);
|                                                    ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:759:45: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
759 |     TORCH_CHECK(static_v.size(2) == head_dim);
|                                             ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:764:49: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
764 |     TORCH_CHECK(key_padding_mask_.size(0) == bsz);
|                                                 ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:765:53: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
765 |     TORCH_CHECK(key_padding_mask_.size(1) == src_len);
|                                                     ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:805:94: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
805 |   TORCH_CHECK(attn_output_weights.sizes() == IntArrayRef({bsz * num_heads, tgt_len, src_len}));
|                                                                                              ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/activation.h:827:87: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
827 |   TORCH_CHECK(attn_output.sizes() == IntArrayRef({bsz * num_heads, tgt_len, head_dim}));
|                                                                                       ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/pooling.h:5,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/normalization.h:5,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional.h:11:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/utils.h:19:31: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
19 |   TORCH_INTERNAL_ASSERT(n >= 0);
|                               ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/pooling.h:772:55: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
772 |     TORCH_INTERNAL_ASSERT(output_ratio != c10::nullopt);
|                                                       ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/pooling.h:850:55: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
850 |     TORCH_INTERNAL_ASSERT(output_ratio != c10::nullopt);
|                                                       ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional.h:15:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/upsampling.h:42:53: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
42 |   TORCH_INTERNAL_ASSERT(scale_factor != c10::nullopt);
|                                                     ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/upsampling.h:125:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
125 |     TORCH_INTERNAL_ASSERT(align_corners != c10::nullopt);
|                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/upsampling.h:134:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
134 |     TORCH_INTERNAL_ASSERT(align_corners != c10::nullopt);
|                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/upsampling.h:144:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
144 |     TORCH_INTERNAL_ASSERT(align_corners != c10::nullopt);
|                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/functional/upsampling.h:148:56: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
148 |     TORCH_INTERNAL_ASSERT(align_corners != c10::nullopt);
|                                                        ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:20,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn.h:7:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/conv.h:284:75: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
284 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(c10::optional<at::IntArrayRef>())})
|                                                                           ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/conv.h:319:75: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
319 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(c10::optional<at::IntArrayRef>())})
|                                                                           ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/conv.h:354:75: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
354 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(c10::optional<at::IntArrayRef>())})
|                                                                           ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:23:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/embedding.h:118:76: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
118 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(Tensor())}, {2, AnyValue(Tensor())})
|                                                                            ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:28:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/pooling.h:482:80: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
482 |   FORWARD_HAS_DEFAULT_ARGS({2, AnyValue(c10::optional<std::vector<int64_t>>())})
|                                                                                ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/pooling.h:511:80: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
511 |   FORWARD_HAS_DEFAULT_ARGS({2, AnyValue(c10::optional<std::vector<int64_t>>())})
|                                                                                ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/pooling.h:540:80: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
540 |   FORWARD_HAS_DEFAULT_ARGS({2, AnyValue(c10::optional<std::vector<int64_t>>())})
|                                                                                ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:29:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:107:51: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
107 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(Tensor())})
|                                                   ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:152:88: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
152 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(torch::optional<std::tuple<Tensor, Tensor>>())})
|                                                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:203:58: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
203 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(torch::Tensor())})
|                                                          ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:279:51: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
279 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(Tensor())})
|                                                   ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:316:88: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
316 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(torch::optional<std::tuple<Tensor, Tensor>>())})
|                                                                                        ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/rnn.h:350:51: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
350 |   FORWARD_HAS_DEFAULT_ARGS({1, AnyValue(Tensor())})
|                                                   ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:32:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/activation.h:806:97: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
806 |   FORWARD_HAS_DEFAULT_ARGS({3, AnyValue(Tensor())}, {4, AnyValue(true)}, {5, AnyValue(Tensor())})
|                                                                                                 ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/autograd/profiler.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/autograd/function.h:6,
from /home/runner/opt/libtorch/include/torch/csrc/autograd/custom_function.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/_functions.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/normalization.h:4,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:33:
/home/runner/opt/libtorch/include/torch/csrc/autograd/profiler_legacy.h:148:38: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
148 |     TORCH_INTERNAL_ASSERT(cpu_ns_ > 0);
|                                      ^
/home/runner/opt/libtorch/include/torch/csrc/autograd/profiler_legacy.h:150:41: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
150 |       TORCH_INTERNAL_ASSERT(device_ >= 0);
|                                         ^
/home/runner/opt/libtorch/include/torch/csrc/autograd/profiler_legacy.h:151:42: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
151 |       TORCH_INTERNAL_ASSERT(cuda_us_ >= 0);
|                                          ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:34:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/transformerlayer.h:52:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
52 |       {2, AnyValue(Tensor())})
|                              ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/transformerlayer.h:173:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
173 |       {5, AnyValue(Tensor())})
|                              ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:35:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/transformercoder.h:51:32: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
51 |         {2, AnyValue(Tensor())})
|                                ^
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/transformercoder.h:130:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
130 |       {5, AnyValue(Tensor())})
|                              ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules.h:36:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/nn/modules/transformer.h:118:30: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
118 |       {7, AnyValue(Tensor())})
|                              ^
In file included from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/optim/adagrad.h:5,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/optim.h:3,
from /home/runner/opt/libtorch/include/torch/csrc/api/include/torch/all.h:14:
/home/runner/opt/libtorch/include/torch/csrc/api/include/torch/optim/serialize.h:153:67: warning: ISO C++11 requires at least one argument for the "..." in a variadic macro
153 |     TORCH_INTERNAL_ASSERT(pytorch_version.toStringRef() == "1.5.0");
|                                                                   ^
In file included from /home/runner/opt/libtorch/include/c10/util/string_view.h:5,
from /home/runner/opt/libtorch/include/c10/util/ConstexprCrc.h:4,
from /home/runner/opt/libtorch/include/c10/util/TypeIndex.h:4,
from /home/runner/opt/libtorch/include/c10/util/typeid.h:27,
from /home/runner/opt/libtorch/include/c10/core/ScalarTypeToTypeMeta.h:4,
from /home/runner/opt/libtorch/include/ATen/core/TensorBody.h:10:
/home/runner/opt/libtorch/include/c10/util/reverse_iterator.h:65:19: warning: ‘template<class _Category, class _Tp, class _Distance, class _Pointer, class _Reference> struct std::iterator’ is deprecated [-Wdeprecated-declarations]
65 |     : public std::iterator<
|                   ^~~~~~~~
In file included from /usr/include/c++/13/bits/stl_iterator_base_funcs.h:66,
from /usr/include/c++/13/string:47,
from /home/runner/opt/include/plumed/core/../tools/Exception.h:26,
from /home/runner/opt/include/plumed/core/../tools/TypesafePtr.h:25,
from /home/runner/opt/include/plumed/core/WithCmd.h:25,
from /home/runner/opt/include/plumed/core/PlumedMain.h:25,
from ./pytorch_model_bias.VBWclW.cpp:24:
/usr/include/c++/13/bits/stl_iterator_base_types.h:127:34: note: declared here
127 |     struct _GLIBCXX17_DEPRECATED iterator
|                                  ^~~~~~~~
In file included from /home/runner/opt/libtorch/include/ATen/core/ivalue_inl.h:6:
/home/runner/opt/libtorch/include/ATen/core/Dict.h:104:40: warning: ‘template<class _Category, class _Tp, class _Distance, class _Pointer, class _Reference> struct std::iterator’ is deprecated [-Wdeprecated-declarations]
104 | class DictIterator final : public std::iterator<std::forward_iterator_tag, DictEntryRef<Key, Value, Iterator>> {
|                                        ^~~~~~~~
/usr/include/c++/13/bits/stl_iterator_base_types.h:127:34: note: declared here
127 |     struct _GLIBCXX17_DEPRECATED iterator
|                                  ^~~~~~~~
/home/runner/opt/libtorch/include/ATen/core/Dict.h:139:24: warning: ‘template<class _Category, class _Tp, class _Distance, class _Pointer, class _Reference> struct std::iterator’ is deprecated [-Wdeprecated-declarations]
139 |   friend typename std::iterator<std::random_access_iterator_tag, DictEntryRef<Key, Value, Iterator>>::difference_type operator-(const DictIterator& lhs, const DictIterator& rhs) {
|                        ^~~~~~~~
/usr/include/c++/13/bits/stl_iterator_base_types.h:127:34: note: declared here
127 |     struct _GLIBCXX17_DEPRECATED iterator
|                                  ^~~~~~~~
/home/runner/opt/libtorch/include/ATen/core/List.h:115:40: warning: ‘template<class _Category, class _Tp, class _Distance, class _Pointer, class _Reference> struct std::iterator’ is deprecated [-Wdeprecated-declarations]
115 | class ListIterator final : public std::iterator<std::random_access_iterator_tag, T> {
|                                        ^~~~~~~~
/usr/include/c++/13/bits/stl_iterator_base_types.h:127:34: note: declared here
127 |     struct _GLIBCXX17_DEPRECATED iterator
|                                  ^~~~~~~~
/home/runner/opt/libtorch/include/ATen/core/List.h:165:24: warning: ‘template<class _Category, class _Tp, class _Distance, class _Pointer, class _Reference> struct std::iterator’ is deprecated [-Wdeprecated-declarations]
165 |   friend typename std::iterator<std::random_access_iterator_tag, T>::difference_type operator-(const ListIterator& lhs, const ListIterator& rhs) {
|                        ^~~~~~~~
/usr/include/c++/13/bits/stl_iterator_base_types.h:127:34: note: declared here
127 |     struct _GLIBCXX17_DEPRECATED iterator
|                                  ^~~~~~~~
</pre>
{% endraw %}
