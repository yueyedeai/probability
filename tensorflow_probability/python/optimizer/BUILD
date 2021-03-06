# Copyright 2018 The TensorFlow Probability Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
# ============================================================================
# Description:
#   Optimizers.

package(
    default_visibility = [
        "//tensorflow_probability:__subpackages__",
    ],
)

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

py_library(
    name = "optimizer",
    srcs = ["__init__.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":bfgs",
        ":lbfgs",
        ":nelder_mead",
        ":sgld",
        ":variational_sgd",
        "//tensorflow_probability/python/optimizer/linesearch",
    ],
)

py_library(
    name = "sgld",
    srcs = ["sgld.py"],
    srcs_version = "PY2AND3",
    deps = [
        # tensorflow dep,
    ],
)

py_test(
    name = "sgld_test",
    size = "medium",
    srcs = ["sgld_test.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "variational_sgd",
    srcs = ["variational_sgd.py"],
    srcs_version = "PY2AND3",
    deps = [
        # tensorflow dep,
    ],
)

py_test(
    name = "variational_sgd_test",
    size = "medium",
    srcs = ["variational_sgd_test.py"],
    deps = [
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "bfgs",
    srcs = ["bfgs.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":bfgs_utils",
        # tensorflow dep,
    ],
)

py_test(
    name = "bfgs_test",
    size = "medium",
    timeout = "long",
    srcs = ["bfgs_test.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "lbfgs",
    srcs = ["lbfgs.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":bfgs_utils",
        # tensorflow dep,
    ],
)

py_test(
    name = "lbfgs_test",
    size = "medium",
    timeout = "long",
    srcs = ["lbfgs_test.py"],
    shard_count = 5,
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "bfgs_utils",
    srcs = ["bfgs_utils.py"],
    srcs_version = "PY2AND3",
    deps = [
        # tensorflow dep,
    ],
)

py_library(
    name = "nelder_mead",
    srcs = ["nelder_mead.py"],
    srcs_version = "PY2AND3",
    deps = [
        # tensorflow dep,
    ],
)

py_test(
    name = "nelder_mead_test",
    size = "medium",
    srcs = ["nelder_mead_test.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)
