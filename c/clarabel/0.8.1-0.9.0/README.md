# Comparing `tmp/clarabel-0.8.1.tar.gz` & `tmp/clarabel-0.9.0.tar.gz`

## Comparing `clarabel-0.8.1.tar` & `clarabel-0.9.0.tar`

### file list

```diff
@@ -1,175 +1,183 @@
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 clarabel-0.8.1/Cargo.toml
--rw-r--r--   0     1001      127      237 2024-05-21 12:42:41.000000 clarabel-0.8.1/.cargo/config.toml
--rw-r--r--   0     1001      127      496 2024-05-21 12:42:41.000000 clarabel-0.8.1/.github/dependabot.yml
--rw-r--r--   0     1001      127      760 2024-05-21 12:42:41.000000 clarabel-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     5159 2024-05-21 12:42:41.000000 clarabel-0.8.1/.github/workflows/pypi.yaml
--rw-r--r--   0     1001      127     4948 2024-05-21 12:42:41.000000 clarabel-0.8.1/.github/workflows/testpypi.yaml
--rw-r--r--   0     1001      127       82 2024-05-21 12:42:41.000000 clarabel-0.8.1/.gitignore
--rw-r--r--   0     1001      127     7173 2024-05-21 12:42:41.000000 clarabel-0.8.1/CHANGELOG.md
--rw-r--r--   0     1001      127    49028 2024-05-21 12:42:48.000000 clarabel-0.8.1/Cargo.lock
--rw-r--r--   0     1001      127    10779 2024-05-21 12:42:41.000000 clarabel-0.8.1/LICENSE.md
--rw-r--r--   0     1001      127     3896 2024-05-21 12:42:41.000000 clarabel-0.8.1/README.md
--rw-r--r--   0     1001      127      430 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_box.py
--rw-r--r--   0     1001      127      613 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_expcone.py
--rw-r--r--   0     1001      127      689 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_powcone.py
--rw-r--r--   0     1001      127      891 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_qp.py
--rw-r--r--   0     1001      127      710 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_sdp.py
--rw-r--r--   0     1001      127      650 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/python/example_socp.py
--rw-r--r--   0     1001      127      807 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_box.rs
--rw-r--r--   0     1001      127      711 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_expcone.rs
--rw-r--r--   0     1001      127      985 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_lp.rs
--rw-r--r--   0     1001      127     1141 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_powcone.rs
--rw-r--r--   0     1001      127     1756 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_qp.rs
--rw-r--r--   0     1001      127      830 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_sdp.rs
--rw-r--r--   0     1001      127      598 2024-05-21 12:42:41.000000 clarabel-0.8.1/examples/rust/example_socp.rs
--rw-r--r--   0     1001      127      696 2024-05-21 12:42:41.000000 clarabel-0.8.1/html/rustdocs-header.html
--rw-r--r--   0     1001      127      152 2024-05-21 12:42:41.000000 clarabel-0.8.1/python/clarabel/__init__.py
--rw-r--r--   0     1001      127       38 2024-05-21 12:42:41.000000 clarabel-0.8.1/rustfmt.toml
--rw-r--r--   0     1001      127     6019 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/csc/block_concatenate.rs
--rw-r--r--   0     1001      127    24016 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/csc/core.rs
--rw-r--r--   0     1001      127     9073 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/csc/matrix_math.rs
--rw-r--r--   0     1001      127      111 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/csc/mod.rs
--rw-r--r--   0     1001      127     9917 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/csc/utils.rs
--rw-r--r--   0     1001      127     3925 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/cholesky.rs
--rw-r--r--   0     1001      127     2210 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/gemm.rs
--rw-r--r--   0     1001      127     2050 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/gemv.rs
--rw-r--r--   0     1001      127     1575 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/lu.rs
--rw-r--r--   0     1001      127      237 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/mod.rs
--rw-r--r--   0     1001      127     7152 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/svd.rs
--rw-r--r--   0     1001      127     4690 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/syevr.rs
--rw-r--r--   0     1001      127     1060 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/symv.rs
--rw-r--r--   0     1001      127     1710 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/syr2k.rs
--rw-r--r--   0     1001      127     1727 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/syrk.rs
--rw-r--r--   0     1001      127    12290 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blas/traits.rs
--rw-r--r--   0     1001      127     3552 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/blaslike_traits.rs
--rw-r--r--   0     1001      127     3533 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/block_concatenate.rs
--rw-r--r--   0     1001      127      687 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/borrowed.rs
--rw-r--r--   0     1001      127     7476 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/core.rs
--rw-r--r--   0     1001      127     2148 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/kron.rs
--rw-r--r--   0     1001      127     7111 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/matrix_math.rs
--rw-r--r--   0     1001      127      250 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/mod.rs
--rw-r--r--   0     1001      127     4778 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/dense/types.rs
--rw-r--r--   0     1001      127     6895 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/densesym3x3/mod.rs
--rw-r--r--   0     1001      127     1251 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/error_types.rs
--rw-r--r--   0     1001      127     3774 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/floats.rs
--rw-r--r--   0     1001      127     6446 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/math_traits.rs
--rw-r--r--   0     1001      127     2423 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/matrix_traits.rs
--rw-r--r--   0     1001      127     2230 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/matrix_types.rs
--rw-r--r--   0     1001      127     1401 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/mod.rs
--rw-r--r--   0     1001      127     3099 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/scalarmath.rs
--rw-r--r--   0     1001      127     2420 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/sparsevector/mod.rs
--rw-r--r--   0     1001      127     9757 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/tests/matrix.rs
--rw-r--r--   0     1001      127       24 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/tests/mod.rs
--rw-r--r--   0     1001      127     3680 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/tests/vector.rs
--rw-r--r--   0     1001      127     3976 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/utils.rs
--rw-r--r--   0     1001      127     5114 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/algebra/vecmath.rs
--rw-r--r--   0     1001      127       14 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/.gitignore
--rw-r--r--   0     1001      127      418 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/Project.toml
--rw-r--r--   0     1001      127     1442 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/src/ClarabelRs.jl
--rw-r--r--   0     1001      127      218 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/src/MOI_wrapper.jl
--rw-r--r--   0     1001      127     4930 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/src/interface.jl
--rw-r--r--   0     1001      127     2570 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/src/types.jl
--rw-r--r--   0     1001      127     3283 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl
--rw-r--r--   0     1001      127      955 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/test/test_jump.jl
--rw-r--r--   0     1001      127     1059 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/ClarabelRs/test/test_problem_depot.jl
--rw-r--r--   0     1001      127      736 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/README.md
--rw-r--r--   0     1001      127     4032 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/interface.rs
--rw-r--r--   0     1001      127       48 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/mod.rs
--rw-r--r--   0     1001      127     3572 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/julia/types.rs
--rw-r--r--   0     1001      127     3093 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/lib.rs
--rw-r--r--   0     1001      127      685 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/.gitignore
--rw-r--r--   0     1001      127     5633 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/cones_py.rs
--rw-r--r--   0     1001      127     1000 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/cscmatrix_py.rs
--rw-r--r--   0     1001      127    15321 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/impl_default_py.rs
--rw-r--r--   0     1001      127     2588 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/io.rs
--rw-r--r--   0     1001      127      873 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/mod.rs
--rw-r--r--   0     1001      127     1765 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/module_py.rs
--rw-r--r--   0     1001      127      871 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/blas_loader.rs
--rw-r--r--   0     1001      127     3695 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/blas_types.rs
--rw-r--r--   0     1001      127     4962 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/blas_wrappers.rs
--rw-r--r--   0     1001      127      901 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/lapack_loader.rs
--rw-r--r--   0     1001      127     3803 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/lapack_types.rs
--rw-r--r--   0     1001      127     6008 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/lapack_wrappers.rs
--rw-r--r--   0     1001      127     1186 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/python/pyblas/mod.rs
--rw-r--r--   0     1001      127      117 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/qdldl/mod.rs
--rw-r--r--   0     1001      127    25421 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/qdldl/qdldl.rs
--rw-r--r--   0     1001      127     8531 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/qdldl/test.rs
--rw-r--r--   0     1001      127     9037 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/chordal_info.rs
--rw-r--r--   0     1001      127    19342 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/augment_compact.rs
--rw-r--r--   0     1001      127     4977 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/augment_standard.rs
--rw-r--r--   0     1001      127     2303 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/mod.rs
--rw-r--r--   0     1001      127     4449 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/psd_completion.rs
--rw-r--r--   0     1001      127     4311 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/reverse_compact.rs
--rw-r--r--   0     1001      127     1540 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/decomp/reverse_standard.rs
--rw-r--r--   0     1001      127    24274 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/merge/clique_graph.rs
--rw-r--r--   0     1001      127     3028 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/merge/disjoint_set_union.rs
--rw-r--r--   0     1001      127     2766 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/merge/mod.rs
--rw-r--r--   0     1001      127      921 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/merge/nomerge.rs
--rw-r--r--   0     1001      127     4341 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/merge/parent_child.rs
--rw-r--r--   0     1001      127      460 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/mod.rs
--rw-r--r--   0     1001      127     1785 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/sparsity_pattern.rs
--rw-r--r--   0     1001      127    13158 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/chordal/supernode_tree.rs
--rw-r--r--   0     1001      127    10556 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/compositecone.rs
--rw-r--r--   0     1001      127    13280 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/expcone.rs
--rw-r--r--   0     1001      127    13661 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/genpowcone.rs
--rw-r--r--   0     1001      127     5367 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/mod.rs
--rw-r--r--   0     1001      127     5738 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/nonnegativecone.rs
--rw-r--r--   0     1001      127     6478 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/nonsymmetric_common.rs
--rw-r--r--   0     1001      127    14539 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/powcone.rs
--rw-r--r--   0     1001      127    13970 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/psdtrianglecone.rs
--rw-r--r--   0     1001      127    15118 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/socone.rs
--rw-r--r--   0     1001      127     9188 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/supportedcone.rs
--rw-r--r--   0     1001      127     3391 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/symmetric_common.rs
--rw-r--r--   0     1001      127     2852 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/cones/zerocone.rs
--rw-r--r--   0     1001      127       35 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/mod.rs
--rw-r--r--   0     1001      127    11788 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
--rw-r--r--   0     1001      127    12389 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
--rw-r--r--   0     1001      127     8500 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
--rw-r--r--   0     1001      127       15 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
--rw-r--r--   0     1001      127     2764 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
--rw-r--r--   0     1001      127      757 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/mod.rs
--rw-r--r--   0     1001      127      517 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/kktsolvers/mod.rs
--rw-r--r--   0     1001      127      402 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/mod.rs
--rw-r--r--   0     1001      127      293 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/settings.rs
--rw-r--r--   0     1001      127    20832 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/solver.rs
--rw-r--r--   0     1001      127     7651 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/core/traits.rs
--rw-r--r--   0     1001      127     8443 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/data_updating.rs
--rw-r--r--   0     1001      127      953 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/equilibration.rs
--rw-r--r--   0     1001      127    11373 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/info.rs
--rw-r--r--   0     1001      127    10801 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/info_print.rs
--rw-r--r--   0     1001      127     8358 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/kktsystem.rs
--rw-r--r--   0     1001      127      592 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/mod.rs
--rw-r--r--   0     1001      127     5441 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/presolver.rs
--rw-r--r--   0     1001      127    11012 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/problemdata.rs
--rw-r--r--   0     1001      127     2984 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/residuals.rs
--rw-r--r--   0     1001      127     6231 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/settings.rs
--rw-r--r--   0     1001      127     2796 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/solution.rs
--rw-r--r--   0     1001      127     3167 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/solver.rs
--rw-r--r--   0     1001      127     8670 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/default/variables.rs
--rw-r--r--   0     1001      127       77 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/implementations/mod.rs
--rw-r--r--   0     1001      127     1998 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/mod.rs
--rw-r--r--   0     1001      127      832 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/tests/cones.rs
--rw-r--r--   0     1001      127       11 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/tests/mod.rs
--rw-r--r--   0     1001      127      761 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/utils/atomic.rs
--rw-r--r--   0     1001      127     1327 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/utils/infbounds.rs
--rw-r--r--   0     1001      127       49 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/solver/utils/mod.rs
--rw-r--r--   0     1001      127      367 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/stdio/mod.rs
--rw-r--r--   0     1001      127      109 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/timers/mod.rs
--rw-r--r--   0     1001      127     5066 2024-05-21 12:42:41.000000 clarabel-0.8.1/src/timers/timers.rs
--rw-r--r--   0     1001      127     2352 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/api_dimension_checks.rs
--rw-r--r--   0     1001      127     2328 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_eq_constrained.rs
--rw-r--r--   0     1001      127     2807 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_expcone.rs
--rw-r--r--   0     1001      127     1439 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_genpowcone.rs
--rw-r--r--   0     1001      127     2605 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_lp.rs
--rw-r--r--   0     1001      127     1382 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_powcone.rs
--rw-r--r--   0     1001      127     4426 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_qp.rs
--rw-r--r--   0     1001      127     2493 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_sdp.rs
--rw-r--r--   0     1001      127     2419 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_socp.rs
--rw-r--r--   0     1001      127      989 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/basic_unconstrained.rs
--rw-r--r--   0     1001      127     9191 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/data_updating.rs
--rw-r--r--   0     1001      127     2600 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/equilibration_bounds.rs
--rw-r--r--   0     1001      127     1126 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/mixed_conic.rs
--rw-r--r--   0     1001      127     2408 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/presolve.rs
--rw-r--r--   0     1001      127     2820 2024-05-21 12:42:41.000000 clarabel-0.8.1/tests/sdp_chordal.rs
--rw-r--r--   0     1001      127      290 2024-05-21 12:42:41.000000 clarabel-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 clarabel-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 clarabel-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127      237 2024-06-01 16:55:16.000000 clarabel-0.9.0/.cargo/config.toml
+-rw-r--r--   0     1001      127      126 2024-06-01 16:55:16.000000 clarabel-0.9.0/.github/codecov.yml
+-rw-r--r--   0     1001      127      496 2024-06-01 16:55:16.000000 clarabel-0.9.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127      778 2024-06-01 16:55:16.000000 clarabel-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     5457 2024-06-01 16:55:16.000000 clarabel-0.9.0/.github/workflows/pypi.yaml
+-rw-r--r--   0     1001      127     5214 2024-06-01 16:55:16.000000 clarabel-0.9.0/.github/workflows/testpypi.yaml
+-rw-r--r--   0     1001      127       82 2024-06-01 16:55:16.000000 clarabel-0.9.0/.gitignore
+-rw-r--r--   0     1001      127     8171 2024-06-01 16:55:16.000000 clarabel-0.9.0/CHANGELOG.md
+-rw-r--r--   0     1001      127      269 2024-06-01 16:55:16.000000 clarabel-0.9.0/CITATION.bib
+-rw-r--r--   0     1001      127    62849 2024-06-01 16:55:21.000000 clarabel-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      127    10779 2024-06-01 16:55:16.000000 clarabel-0.9.0/LICENSE.md
+-rw-r--r--   0     1001      127     4185 2024-06-01 16:55:16.000000 clarabel-0.9.0/README.md
+-rw-r--r--   0     1001      127     1589 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/data/hs35.json
+-rw-r--r--   0     1001      127      430 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_box.py
+-rw-r--r--   0     1001      127      613 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_expcone.py
+-rw-r--r--   0     1001      127      362 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_json.py
+-rw-r--r--   0     1001      127      689 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_powcone.py
+-rw-r--r--   0     1001      127      891 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_qp.py
+-rw-r--r--   0     1001      127      710 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_sdp.py
+-rw-r--r--   0     1001      127      650 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/python/example_socp.py
+-rw-r--r--   0     1001      127      809 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_box.rs
+-rw-r--r--   0     1001      127      880 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_box_faer.rs
+-rw-r--r--   0     1001      127      711 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_expcone.rs
+-rw-r--r--   0     1001      127      561 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_json.rs
+-rw-r--r--   0     1001      127      985 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_lp.rs
+-rw-r--r--   0     1001      127     1141 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_powcone.rs
+-rw-r--r--   0     1001      127     1756 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_qp.rs
+-rw-r--r--   0     1001      127      830 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_sdp.rs
+-rw-r--r--   0     1001      127      598 2024-06-01 16:55:16.000000 clarabel-0.9.0/examples/rust/example_socp.rs
+-rw-r--r--   0     1001      127      696 2024-06-01 16:55:16.000000 clarabel-0.9.0/html/rustdocs-header.html
+-rw-r--r--   0     1001      127      152 2024-06-01 16:55:16.000000 clarabel-0.9.0/python/clarabel/__init__.py
+-rw-r--r--   0     1001      127       38 2024-06-01 16:55:16.000000 clarabel-0.9.0/rustfmt.toml
+-rw-r--r--   0     1001      127     6019 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/csc/block_concatenate.rs
+-rw-r--r--   0     1001      127    24229 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/csc/core.rs
+-rw-r--r--   0     1001      127     9073 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/csc/matrix_math.rs
+-rw-r--r--   0     1001      127      111 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/csc/mod.rs
+-rw-r--r--   0     1001      127     9917 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/csc/utils.rs
+-rw-r--r--   0     1001      127     3925 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/cholesky.rs
+-rw-r--r--   0     1001      127     2210 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/gemm.rs
+-rw-r--r--   0     1001      127     2050 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/gemv.rs
+-rw-r--r--   0     1001      127     1575 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/lu.rs
+-rw-r--r--   0     1001      127      237 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/mod.rs
+-rw-r--r--   0     1001      127     7152 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/svd.rs
+-rw-r--r--   0     1001      127     4690 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/syevr.rs
+-rw-r--r--   0     1001      127     1060 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/symv.rs
+-rw-r--r--   0     1001      127     1710 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/syr2k.rs
+-rw-r--r--   0     1001      127     1727 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/syrk.rs
+-rw-r--r--   0     1001      127    12290 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blas/traits.rs
+-rw-r--r--   0     1001      127     3552 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/blaslike_traits.rs
+-rw-r--r--   0     1001      127     3533 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/block_concatenate.rs
+-rw-r--r--   0     1001      127      687 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/borrowed.rs
+-rw-r--r--   0     1001      127     7476 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/core.rs
+-rw-r--r--   0     1001      127     2148 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/kron.rs
+-rw-r--r--   0     1001      127     7111 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/matrix_math.rs
+-rw-r--r--   0     1001      127      250 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/mod.rs
+-rw-r--r--   0     1001      127     4778 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/dense/types.rs
+-rw-r--r--   0     1001      127     6895 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/densesym3x3/mod.rs
+-rw-r--r--   0     1001      127     1251 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/error_types.rs
+-rw-r--r--   0     1001      127     3828 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/floats.rs
+-rw-r--r--   0     1001      127     6446 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/math_traits.rs
+-rw-r--r--   0     1001      127     2435 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/matrix_traits.rs
+-rw-r--r--   0     1001      127     2230 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/matrix_types.rs
+-rw-r--r--   0     1001      127     1401 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/mod.rs
+-rw-r--r--   0     1001      127     3147 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/scalarmath.rs
+-rw-r--r--   0     1001      127     2420 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/sparsevector/mod.rs
+-rw-r--r--   0     1001      127     9757 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/tests/matrix.rs
+-rw-r--r--   0     1001      127       24 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/tests/mod.rs
+-rw-r--r--   0     1001      127     3752 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/tests/vector.rs
+-rw-r--r--   0     1001      127     4016 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/utils.rs
+-rw-r--r--   0     1001      127     5082 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/algebra/vecmath.rs
+-rw-r--r--   0     1001      127       14 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/.gitignore
+-rw-r--r--   0     1001      127      418 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/Project.toml
+-rw-r--r--   0     1001      127     1442 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/src/ClarabelRs.jl
+-rw-r--r--   0     1001      127      218 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/src/MOI_wrapper.jl
+-rw-r--r--   0     1001      127     5792 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/src/interface.jl
+-rw-r--r--   0     1001      127     2672 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/src/types.jl
+-rw-r--r--   0     1001      127     3283 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl
+-rw-r--r--   0     1001      127      955 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/test/test_jump.jl
+-rw-r--r--   0     1001      127     1059 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/ClarabelRs/test/test_problem_depot.jl
+-rw-r--r--   0     1001      127      736 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/README.md
+-rw-r--r--   0     1001      127     5794 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/interface.rs
+-rw-r--r--   0     1001      127       48 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/mod.rs
+-rw-r--r--   0     1001      127     3572 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/julia/types.rs
+-rw-r--r--   0     1001      127     3093 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127      685 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/.gitignore
+-rw-r--r--   0     1001      127     5633 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/cones_py.rs
+-rw-r--r--   0     1001      127     1000 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/cscmatrix_py.rs
+-rw-r--r--   0     1001      127    16106 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/impl_default_py.rs
+-rw-r--r--   0     1001      127     2588 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/io.rs
+-rw-r--r--   0     1001      127      873 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/mod.rs
+-rw-r--r--   0     1001      127     1844 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/module_py.rs
+-rw-r--r--   0     1001      127      871 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/blas_loader.rs
+-rw-r--r--   0     1001      127     3695 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/blas_types.rs
+-rw-r--r--   0     1001      127     4962 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/blas_wrappers.rs
+-rw-r--r--   0     1001      127      901 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/lapack_loader.rs
+-rw-r--r--   0     1001      127     3803 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/lapack_types.rs
+-rw-r--r--   0     1001      127     6008 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/lapack_wrappers.rs
+-rw-r--r--   0     1001      127     1186 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/python/pyblas/mod.rs
+-rw-r--r--   0     1001      127      117 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/qdldl/mod.rs
+-rw-r--r--   0     1001      127    26672 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/qdldl/qdldl.rs
+-rw-r--r--   0     1001      127     8526 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/qdldl/test.rs
+-rw-r--r--   0     1001      127     9037 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/chordal_info.rs
+-rw-r--r--   0     1001      127    19342 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/augment_compact.rs
+-rw-r--r--   0     1001      127     4977 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/augment_standard.rs
+-rw-r--r--   0     1001      127     2303 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/mod.rs
+-rw-r--r--   0     1001      127     4449 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/psd_completion.rs
+-rw-r--r--   0     1001      127     4311 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/reverse_compact.rs
+-rw-r--r--   0     1001      127     1540 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/decomp/reverse_standard.rs
+-rw-r--r--   0     1001      127    24274 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/merge/clique_graph.rs
+-rw-r--r--   0     1001      127     3028 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/merge/disjoint_set_union.rs
+-rw-r--r--   0     1001      127     2766 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/merge/mod.rs
+-rw-r--r--   0     1001      127      921 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/merge/nomerge.rs
+-rw-r--r--   0     1001      127     4341 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/merge/parent_child.rs
+-rw-r--r--   0     1001      127      460 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/mod.rs
+-rw-r--r--   0     1001      127     1785 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/sparsity_pattern.rs
+-rw-r--r--   0     1001      127    13158 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/chordal/supernode_tree.rs
+-rw-r--r--   0     1001      127    10556 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/compositecone.rs
+-rw-r--r--   0     1001      127    13280 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/expcone.rs
+-rw-r--r--   0     1001      127    13661 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/genpowcone.rs
+-rw-r--r--   0     1001      127     5367 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/mod.rs
+-rw-r--r--   0     1001      127     5738 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/nonnegativecone.rs
+-rw-r--r--   0     1001      127     6478 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/nonsymmetric_common.rs
+-rw-r--r--   0     1001      127    14539 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/powcone.rs
+-rw-r--r--   0     1001      127    13970 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/psdtrianglecone.rs
+-rw-r--r--   0     1001      127    15118 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/socone.rs
+-rw-r--r--   0     1001      127     9360 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/supportedcone.rs
+-rw-r--r--   0     1001      127     3391 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/symmetric_common.rs
+-rw-r--r--   0     1001      127     2852 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/cones/zerocone.rs
+-rw-r--r--   0     1001      127       35 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/mod.rs
+-rw-r--r--   0     1001      127    11788 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs
+-rw-r--r--   0     1001      127    12621 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs
+-rw-r--r--   0     1001      127     8500 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs
+-rw-r--r--   0     1001      127    11937 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/faer_ldl.rs
+-rw-r--r--   0     1001      127       65 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/mod.rs
+-rw-r--r--   0     1001      127     2764 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs
+-rw-r--r--   0     1001      127      757 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/mod.rs
+-rw-r--r--   0     1001      127      517 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/kktsolvers/mod.rs
+-rw-r--r--   0     1001      127      402 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/mod.rs
+-rw-r--r--   0     1001      127      293 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/settings.rs
+-rw-r--r--   0     1001      127    21167 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/solver.rs
+-rw-r--r--   0     1001      127     7651 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/core/traits.rs
+-rw-r--r--   0     1001      127     8443 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/data_updating.rs
+-rw-r--r--   0     1001      127      953 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/equilibration.rs
+-rw-r--r--   0     1001      127    11373 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/info.rs
+-rw-r--r--   0     1001      127    10801 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/info_print.rs
+-rw-r--r--   0     1001      127     3965 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/json.rs
+-rw-r--r--   0     1001      127     8358 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/kktsystem.rs
+-rw-r--r--   0     1001      127      629 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/mod.rs
+-rw-r--r--   0     1001      127     5441 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/presolver.rs
+-rw-r--r--   0     1001      127    11042 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/problemdata.rs
+-rw-r--r--   0     1001      127     2984 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/residuals.rs
+-rw-r--r--   0     1001      127     9641 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/settings.rs
+-rw-r--r--   0     1001      127     2796 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/solution.rs
+-rw-r--r--   0     1001      127     3167 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/solver.rs
+-rw-r--r--   0     1001      127     8682 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/default/variables.rs
+-rw-r--r--   0     1001      127       77 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/implementations/mod.rs
+-rw-r--r--   0     1001      127     2107 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/mod.rs
+-rw-r--r--   0     1001      127      832 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/tests/cones.rs
+-rw-r--r--   0     1001      127       11 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/tests/mod.rs
+-rw-r--r--   0     1001      127      761 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/utils/atomic.rs
+-rw-r--r--   0     1001      127     1327 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/utils/infbounds.rs
+-rw-r--r--   0     1001      127       49 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/solver/utils/mod.rs
+-rw-r--r--   0     1001      127      367 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/stdio/mod.rs
+-rw-r--r--   0     1001      127      109 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/timers/mod.rs
+-rw-r--r--   0     1001      127     5202 2024-06-01 16:55:16.000000 clarabel-0.9.0/src/timers/timers.rs
+-rw-r--r--   0     1001      127     2352 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/api_dimension_checks.rs
+-rw-r--r--   0     1001      127     2328 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_eq_constrained.rs
+-rw-r--r--   0     1001      127     2807 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_expcone.rs
+-rw-r--r--   0     1001      127     1439 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_genpowcone.rs
+-rw-r--r--   0     1001      127     2605 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_lp.rs
+-rw-r--r--   0     1001      127     1382 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_powcone.rs
+-rw-r--r--   0     1001      127     4426 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_qp.rs
+-rw-r--r--   0     1001      127     2493 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_sdp.rs
+-rw-r--r--   0     1001      127     2419 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_socp.rs
+-rw-r--r--   0     1001      127      989 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/basic_unconstrained.rs
+-rw-r--r--   0     1001      127     9191 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/data_updating.rs
+-rw-r--r--   0     1001      127     2649 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/equilibration_bounds.rs
+-rw-r--r--   0     1001      127     1126 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/mixed_conic.rs
+-rw-r--r--   0     1001      127     2408 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/presolve.rs
+-rw-r--r--   0     1001      127     2820 2024-06-01 16:55:16.000000 clarabel-0.9.0/tests/sdp_chordal.rs
+-rw-r--r--   0     1001      127      290 2024-06-01 16:55:16.000000 clarabel-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4759 1970-01-01 00:00:00.000000 clarabel-0.9.0/PKG-INFO
```

### Comparing `clarabel-0.8.1/Cargo.toml` & `clarabel-0.9.0/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "clarabel"
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Paul Goulart <paul.goulart@eng.ox.ac.uk>"]
 edition = "2021"
 rust-version = "1.66"
 license = "Apache-2.0"
 description = "Clarabel Conic Interior Point Solver for Rust / Python"
 readme = "README.md"
 repository = "https://github.com/oxfordcontrol/Clarabel.rs"
@@ -25,35 +25,44 @@
 itertools      = "0.11"
 
 # -------------------------------
 # features
 # -------------------------------
 
 [features]
+default = ["serde"]
+
+# enable reading / writing of problems from json files 
+serde = ["dep:serde", "dep:serde_json"]
 
 # enables blas/lapack for SDP support, with blas/lapack src unspecified
 # also enable packages required for chordal decomposition 
 sdp = ["blas","lapack", "indexmap"]
 
 # explicit configuration options for different blas flavours
 sdp-accelerate = ["sdp", "blas-src/accelerate", "lapack-src/accelerate"]
 sdp-netlib     = ["sdp", "blas-src/netlib", "lapack-src/netlib"]
 sdp-openblas   = ["sdp", "blas-src/openblas", "lapack-src/openblas"]
 sdp-mkl        = ["sdp", "blas-src/intel-mkl", "lapack-src/intel-mkl"]
 sdp-r          = ["sdp", "blas-src/r", "lapack-src/r"]
 
+
 # build as the julia interface 
-julia = ["sdp", "dep:libc", "dep:num-derive", "dep:serde", "dep:serde_json"] 
+julia = ["sdp", "dep:libc", "dep:num-derive",  "serde", "faer-sparse"] 
  
 # build as the python interface via maturin.
 # NB: python builds use scipy shared libraries
 # for blas/lapack, and should *not* explicitly 
 # enable a blas/lapack source package 
-python = ["sdp", "dep:libc", "dep:pyo3", "dep:num-derive"]
+python = ["sdp", "dep:libc", "dep:pyo3", "dep:num-derive", "serde", "faer-sparse"]
+
+wasm = ["dep:web-time"]
 
+#compile with faer supernodal solver option
+faer-sparse = ["dep:faer", "dep:faer-entity"]
 
 # -------------------------------
 # SDP configuration
 # -------------------------------
 
 [dependencies.blas]
 version = "0.22.0"
@@ -71,14 +80,22 @@
 version = "0.10"
 optional = true 
 
 [dependencies.indexmap]
 version = "2.2"
 optional = true
 
+[dependencies.faer]
+version = "0.19"
+optional = true 
+
+[dependencies.faer-entity]
+version = "0.19"
+optional = true 
+
 
 # -------------------------------
 # examples
 # -------------------------------
 
 [[example]]
 name = "lp"
@@ -105,14 +122,26 @@
 path = "examples/rust/example_box.rs"
 
 [[example]]
 name = "sdp"
 path = "examples/rust/example_sdp.rs"
 required-features = ["sdp"]
 
+[[example]]
+name = "box_faer"
+path = "examples/rust/example_box_faer.rs"
+required-features = ["faer-sparse"]
+
+[[example]]
+name = "json"
+path = "examples/rust/example_json.rs"
+required-features = ["serde"]
+
+
+
 
 # -------------------------------
 # custom build profiles 
 # -------------------------------
 [profile.release-with-debug]
 inherits = "release"
 debug = true
@@ -158,7 +187,21 @@
 # credit: https://github.com/victe/rust-latex-doc-minimal-example
 # ------------------------------
 
 [package.metadata.docs.rs]
 rustdoc-args = [ "--html-in-header", "./html/rustdocs-header.html" ]
 features = ["sdp","sdp-mkl"]
 
+# ------------------------------
+# wasm compatibility
+# ------------------------------
+
+[dependencies.web-time]
+optional = true
+version = "0.2.3"
+
+# ------------------------------
+# testing, benchmarking etc 
+# ------------------------------
+[dev-dependencies]
+tempfile = "3"
+
```

### Comparing `clarabel-0.8.1/.github/workflows/ci.yml` & `clarabel-0.9.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       run: cargo test --verbose --features sdp-accelerate
 
     - name: Install cargo-tarpaulin
       run: cargo install cargo-tarpaulin
 
     - name: Generate code coverage 
       run: |
-        cargo tarpaulin --out xml --features sdp-accelerate --exclude-files "src/python/*,src/julia/*"
+        cargo tarpaulin --out xml --features sdp-accelerate,serde,faer-sparse --exclude-files "src/python/*,src/julia/*"
 
     - name: Upload to codecov.io
       uses: codecov/codecov-action@v4
       with:
         token: ${{secrets.CODECOV_TOKEN}}
```

### Comparing `clarabel-0.8.1/.github/workflows/pypi.yaml` & `clarabel-0.9.0/.github/workflows/pypi.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,17 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-linux-${{ matrix.target }}
           path: dist
 
 
   macos:
     runs-on: macos-13
     # if: "startsWith(github.ref, 'refs/tags/v')"
     steps:
@@ -96,17 +96,17 @@
           pip install --upgrade pip
           pip install dist/${{ env.PACKAGE_NAME }}-*universal2.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos
           path: dist
 
   windows:
     runs-on: windows-latest
     # if: "startsWith(github.ref, 'refs/tags/v')"
     strategy:
       matrix:
@@ -130,17 +130,17 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-windows-${{ matrix.target }}
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
@@ -150,39 +150,47 @@
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           manylinux: auto
           args: --out dist 
 
+      - name: Test sdist
+        run: |
+          pip install --force-reinstall --verbose dist/*.tar.gz
+          python -c 'import clarabel'
+          
       - name: Upload sdist
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: sdist
           path: dist
 
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/v')"
     needs: 
       - macos
       - windows
       - linux
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: wheels
-      - uses: actions/download-artifact@v3
+          pattern: wheels-*
+          merge-multiple: true
+          path: dist
+      - uses: actions/download-artifact@v4
         with:
           name: sdist
+          path: dist
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Publish to PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
           pip install --upgrade twine
-          twine upload --skip-existing --repository ${{ env.PYPI_TARGET  }} *
+          twine upload --skip-existing --repository ${{ env.PYPI_TARGET  }} dist/*
```

### Comparing `clarabel-0.8.1/.github/workflows/testpypi.yaml` & `clarabel-0.9.0/.github/workflows/testpypi.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -36,28 +36,27 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-linux-${{ matrix.target }}
           path: dist
 
 
   macos:
-    runs-on: macos-latest
+    runs-on: macos-13
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
-          architecture: x64
 
       - name: Install Rust toolchain
         uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           profile: minimal
           default: true
@@ -88,17 +87,17 @@
           pip install --upgrade pip
           pip install dist/${{ env.PACKAGE_NAME }}-*universal2.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos
           path: dist
 
   windows:
     runs-on: windows-latest
     strategy:
       matrix:
         target: [x64, x86]
@@ -121,17 +120,17 @@
         run: |
           python -m pip install dist/${{ env.PACKAGE_NAME }}-*.whl --force-reinstall
           python -c "import clarabel"
           python examples/python/example_qp.py 
           python examples/python/example_sdp.py 
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-windows-${{ matrix.target }}
           path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
@@ -141,38 +140,46 @@
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           manylinux: auto
           args: --out dist 
 
+      - name: Test sdist
+        run: |
+          pip install --force-reinstall --verbose dist/*.tar.gz
+          python -c 'import clarabel'
+          
       - name: Upload sdist
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: sdist
           path: dist
 
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: 
       - macos
       - windows
       - linux
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: wheels
-      - uses: actions/download-artifact@v3
+          pattern: wheels-*
+          merge-multiple: true
+          path: dist
+      - uses: actions/download-artifact@v4
         with:
           name: sdist
+          path: dist
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Publish to Test PyPi
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TEST_PYPI_TOKEN }}
         run: |
           pip install --upgrade twine
-          twine upload --skip-existing --repository ${{ env.PYPI_TARGET  }} *
+          twine upload --skip-existing --repository ${{ env.PYPI_TARGET  }} dist/*
```

### Comparing `clarabel-0.8.1/CHANGELOG.md` & `clarabel-0.9.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 
 Changes for the Rust version of Clarabel are documented in this file. For the Julia version, see [here](https://github.com/oxfordcontrol/Clarabel.jl/blob/main/CHANGELOG.md).
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 Version numbering in this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).  We aim to keep the core solver functionality and minor releases in sync between the Rust/Python and Julia implementations.  Small fixes that affect one implementation only may result in the patch release versions differing.
 
+## [0.9.0] - 2024-01-06
+
+- ## What's Changed
+- Read/write problems to JSON files [#111](https://github.com/oxfordcontrol/Clarabel.rs/pull/111)
+
+## Rust specific changes
+- validation tools for solver settings [#113](https://github.com/oxfordcontrol/Clarabel.rs/pull/113)
+
+- adds feature to include supernodal LDL solver from `faer-rs` [#112](https://github.com/oxfordcontrol/Clarabel.rs/pull/112)
+
+- Add wasm feature by @alexarice in [#114](https://github.com/oxfordcontrol/Clarabel.rs/pull/114)
+- pypi and testpypi build updates by @tschm in [#110](https://github.com/oxfordcontrol/Clarabel.rs/pull/110), [#115](https://github.com/oxfordcontrol/Clarabel.rs/pull/115), [#109](https://github.com/oxfordcontrol/Clarabel.rs/pull/109)
+
+
+
+## [0.8.1] - 2024-21-05
+### Changed 
+
+- change to docs.rs configuration so that SDP documentation will build
+
 ## [0.8.0] - 2024-21-05
 ### Changed 
 
 - implements chordal decomposition for PSD cones [#100](https://github.com/oxfordcontrol/Clarabel.rs/pull/100)
 - updates scaling bounds. Fixes [#96](https://github.com/oxfordcontrol/Clarabel.rs/issues/96)
 
 ### Rust specific changes
@@ -134,15 +154,16 @@
 
 ## [0.2.0] - 2022-07-31
 
 - Rust/python implementation released starting from this version.
 
 - Ported all documentation to the common site [here](https://github.com/oxfordcontrol/ClarabelDocs)
 
-
+[0.9.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.8.1...v0.9.0
+[0.8.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.7.1...v0.8.0
 [0.7.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.6.0...v0.7.0
 [0.6.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.4.1...v0.5.0
 [0.4.1]: https://github.com/oxfordcontrol/Clarabel.rs/compare/v0.4.0...v0.4.1
```

### Comparing `clarabel-0.8.1/Cargo.lock` & `clarabel-0.9.0/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -128,14 +128,40 @@
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
+name = "bytemuck"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
+dependencies = [
+ "bytemuck_derive",
+]
+
+[[package]]
+name = "bytemuck_derive"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ee891b04274a59bd38b412188e24b849617b2e45a0fd8d057deb63e7403761b"
+dependencies = [
+ "proc-macro2 1.0.84",
+ "quote 1.0.36",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "byteorder"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
+
+[[package]]
 name = "cc"
 version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
@@ -155,46 +181,56 @@
  "num-traits",
  "wasm-bindgen",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "clarabel"
-version = "0.8.1"
+version = "0.9.0"
 dependencies = [
  "amd",
  "blas",
  "blas-src",
  "cfg-if",
  "derive_builder 0.11.2",
  "enum_dispatch",
+ "faer",
+ "faer-entity",
  "indexmap",
  "itertools",
  "lapack",
  "lapack-src",
  "lazy_static",
  "libc",
  "num-derive",
  "num-traits",
  "pyo3",
  "serde",
  "serde_json",
+ "tempfile",
  "thiserror",
+ "web-time",
 ]
 
 [[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "coe-rs"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e8f1e641542c07631228b1e0dc04b69ae3c1d58ef65d5691a439711d805c698"
+
+[[package]]
 name = "core-foundation"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -221,14 +257,45 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
+
+[[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
@@ -258,32 +325,32 @@
 name = "darling_core"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
 dependencies = [
  "fnv",
  "ident_case",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "strsim 0.10.0",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling_core"
 version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
 dependencies = [
  "fnv",
  "ident_case",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "strsim 0.11.1",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
@@ -297,18 +364,24 @@
 name = "darling_macro"
 version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
 dependencies = [
  "darling_core 0.20.9",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
+name = "dbgf"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6ca96b45ca70b8045e0462f191bd209fcb3c3bfe8dbfb1257ada54c4dd59169"
+
+[[package]]
 name = "derive_builder"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d07adf7be193b71cc36b193d0f5fe60b918a3a9db4dad0449f57bcfd519704a3"
 dependencies = [
  "derive_builder_macro 0.11.2",
 ]
@@ -325,29 +398,29 @@
 [[package]]
 name = "derive_builder_core"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f91d4cfa921f1c05904dc3c57b4a32c38aed3340cce209f3a6fd1478babafc4"
 dependencies = [
  "darling 0.14.4",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_builder_core"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling 0.20.9",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f0314b72bed045f3a68671b3c86328386762c93f82d98c65c3cb5e5f573dd68"
@@ -359,15 +432,15 @@
 [[package]]
 name = "derive_builder_macro"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core 0.20.0",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -414,29 +487,71 @@
  "libc",
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "dyn-stack"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56e53799688f5632f364f8fb387488dd05db9fe45db7011be066fc20e7027f8b"
+dependencies = [
+ "bytemuck",
+ "reborrow",
+]
+
+[[package]]
 name = "either"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
+name = "enum-as-inner"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
+dependencies = [
+ "heck",
+ "proc-macro2 1.0.84",
+ "quote 1.0.36",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "enum_dispatch"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "equator"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c35da53b5a021d2484a7cc49b2ac7f2d840f8236a286f84202369bd338d761ea"
+dependencies = [
+ "equator-macro",
+]
+
+[[package]]
+name = "equator-macro"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3bf679796c0322556351f287a51b49e48f7c4986e727b5dd78c972d30e2e16cc"
+dependencies = [
+ "proc-macro2 1.0.84",
+ "quote 1.0.36",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -448,14 +563,57 @@
 checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "faer"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ef9e1a4098a9e3a03c47bc5061406c04820552d869fd0fcd92587d07b271f0"
+dependencies = [
+ "bytemuck",
+ "coe-rs",
+ "dbgf",
+ "dyn-stack",
+ "equator",
+ "faer-entity",
+ "gemm",
+ "libm",
+ "matrixcompare",
+ "matrixcompare-core",
+ "nano-gemm",
+ "npyz",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "rand",
+ "rand_distr",
+ "rayon",
+ "reborrow",
+ "serde",
+]
+
+[[package]]
+name = "faer-entity"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab968a02be27be95de0f1ad0af901b865fa0866b6a9b553a6cc9cf7f19c2ce71"
+dependencies = [
+ "bytemuck",
+ "coe-rs",
+ "libm",
+ "num-complex",
+ "num-traits",
+ "pulp",
+ "reborrow",
+]
+
+[[package]]
 name = "fastrand"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "filetime"
@@ -506,14 +664,132 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "gemm"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e400f2ffd14e7548356236c35dc39cad6666d833a852cb8a8f3f28029359bb03"
+dependencies = [
+ "dyn-stack",
+ "gemm-c32",
+ "gemm-c64",
+ "gemm-common",
+ "gemm-f16",
+ "gemm-f32",
+ "gemm-f64",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "seq-macro",
+]
+
+[[package]]
+name = "gemm-c32"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10dc4a6176c8452d60eac1a155b454c91c668f794151a303bf3c75ea2874812d"
+dependencies = [
+ "dyn-stack",
+ "gemm-common",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "seq-macro",
+]
+
+[[package]]
+name = "gemm-c64"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc2032ce2c0bb150da0256338759a6fb01ca056f6dfe28c4d14af32d7f878f6f"
+dependencies = [
+ "dyn-stack",
+ "gemm-common",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "seq-macro",
+]
+
+[[package]]
+name = "gemm-common"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90fd234fc525939654f47b39325fd5f55e552ceceea9135f3aa8bdba61eabef6"
+dependencies = [
+ "bytemuck",
+ "dyn-stack",
+ "half",
+ "num-complex",
+ "num-traits",
+ "once_cell",
+ "paste",
+ "pulp",
+ "raw-cpuid",
+ "rayon",
+ "seq-macro",
+ "sysctl",
+]
+
+[[package]]
+name = "gemm-f16"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fc3652651f96a711d46b8833e1fac27a864be4bdfa81a374055f33ddd25c0c6"
+dependencies = [
+ "dyn-stack",
+ "gemm-common",
+ "gemm-f32",
+ "half",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "rayon",
+ "seq-macro",
+]
+
+[[package]]
+name = "gemm-f32"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbc51c44ae3defd207e6d9416afccb3c4af1e7cef5e4960e4c720ac4d6f998e"
+dependencies = [
+ "dyn-stack",
+ "gemm-common",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "seq-macro",
+]
+
+[[package]]
+name = "gemm-f64"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f37fc86e325c2415a4d0cab8324a0c5371ec06fc7d2f9cb1636fcfc9536a8d8"
+dependencies = [
+ "dyn-stack",
+ "gemm-common",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "raw-cpuid",
+ "seq-macro",
+]
+
+[[package]]
 name = "generic-array"
 version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
@@ -533,20 +809,32 @@
 [[package]]
 name = "getset"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e45727250e75cc04ff2846a66397da8ef2b3db8e40e0cef4df67950a07621eb9"
 dependencies = [
  "proc-macro-error",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "half"
+version = "2.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
+dependencies = [
+ "bytemuck",
+ "cfg-if",
+ "crunchy",
+ "num-traits",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
@@ -697,14 +985,20 @@
 [[package]]
 name = "libc"
 version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
+name = "libm"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
+
+[[package]]
 name = "libredox"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
@@ -729,14 +1023,30 @@
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "matrixcompare"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37832ba820e47c93d66b4360198dccb004b43c74abc3ac1ce1fed54e65a80445"
+dependencies = [
+ "matrixcompare-core",
+ "num-traits",
+]
+
+[[package]]
+name = "matrixcompare-core"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0bdabb30db18805d5290b3da7ceaccbddba795620b86c02145d688e04900a73"
+
+[[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
@@ -753,20 +1063,89 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "nano-gemm"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f563548d38f390ef9893e4883ec38c1fb312f569e98d76bededdd91a3b41a043"
+dependencies = [
+ "equator",
+ "nano-gemm-c32",
+ "nano-gemm-c64",
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "nano-gemm-f32",
+ "nano-gemm-f64",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-c32"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a40449e57a5713464c3a1208c4c3301c8d29ee1344711822cf022bc91373a91b"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-c64"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "743a6e6211358fba85d1009616751e4107da86f4c95b24e684ce85f25c25b3bf"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+ "num-complex",
+]
+
+[[package]]
+name = "nano-gemm-codegen"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "963bf7c7110d55430169dc74c67096375491ed580cd2ef84842550ac72e781fa"
+
+[[package]]
+name = "nano-gemm-core"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe3fc4f83ae8861bad79dc3c016bd6b0220da5f9de302e07d3112d16efc24aa6"
+
+[[package]]
+name = "nano-gemm-f32"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e3681b7ce35658f79da94b7f62c60a005e29c373c7111ed070e3bf64546a8bb"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+]
+
+[[package]]
+name = "nano-gemm-f64"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc1e619ed04d801809e1f63e61b669d380c4119e8b0cdd6ed184c6b111f046d8"
+dependencies = [
+ "nano-gemm-codegen",
+ "nano-gemm-core",
+]
+
+[[package]]
 name = "native-tls"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
+checksum = "a8614eb2c83d59d1c8cc974dd3f920198647674a0a035e1af1fa58707e317466"
 dependencies = [
- "lazy_static",
  "libc",
  "log",
  "openssl",
  "openssl-probe",
  "openssl-sys",
  "schannel",
  "security-framework",
@@ -780,40 +1159,73 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39f41f36bb4d46906d5a72da5b73a804d9de1a7282eb7c89617201acda7b8212"
 dependencies = [
  "cmake",
 ]
 
 [[package]]
+name = "npyz"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "13f27ea175875c472b3df61ece89a6d6ef4e0627f43704e400c782f174681ebd"
+dependencies = [
+ "byteorder",
+ "num-bigint",
+ "py_literal",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
+dependencies = [
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-complex"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
+ "bytemuck",
  "num-traits",
+ "rand",
 ]
 
 [[package]]
 name = "num-derive"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eafd0b45c5537c3ba526f79d3e75120036502bebacbb3f3220914067ce39dbf2"
 dependencies = [
  "proc-macro2 0.4.30",
  "quote 0.6.13",
  "syn 0.15.44",
 ]
 
 [[package]]
+name = "num-integer"
+version = "0.1.46"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "oci-spec"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e423c4f827362c0d8d8da4b1f571270f389ebde73bcd3240a3d23c6d6f61d0f0"
@@ -901,17 +1313,17 @@
 
 [[package]]
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -932,17 +1344,17 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -954,20 +1366,71 @@
  "libc",
  "redox_syscall 0.5.1",
  "smallvec",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
+
+[[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pest"
+version = "2.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "560131c633294438da9f7c4b08189194b20946c8274c6b9e38881a7874dc8ee8"
+dependencies = [
+ "memchr",
+ "thiserror",
+ "ucd-trie",
+]
+
+[[package]]
+name = "pest_derive"
+version = "2.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26293c9193fbca7b1a3bf9b79dc1e388e927e6cacaa78b4a3ab705a1d3d41459"
+dependencies = [
+ "pest",
+ "pest_generator",
+]
+
+[[package]]
+name = "pest_generator"
+version = "2.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3ec22af7d3fb470a85dd2ca96b7c577a1eb4ef6f1683a9fe9a8c16e136c04687"
+dependencies = [
+ "pest",
+ "pest_meta",
+ "proc-macro2 1.0.84",
+ "quote 1.0.36",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "pest_meta"
+version = "2.7.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d7a240022f37c361ec1878d646fc5b7d7c4d28d5946e1a80ad5a7a4f4ca0bdcd"
+dependencies = [
+ "once_cell",
+ "pest",
+ "sha2",
+]
+
+[[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "portable-atomic"
@@ -978,27 +1441,27 @@
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
 version = "0.4.30"
@@ -1006,22 +1469,47 @@
 checksum = "cf3d2011ab5c909338f7887f4fc896d35932e29146c12c8d01da6b22a80ba759"
 dependencies = [
  "unicode-xid",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.83"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "pulp"
+version = "0.18.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ec8d02258294f59e4e223b41ad7e81c874aa6b15bc4ced9ba3965826da0eed5"
+dependencies = [
+ "bytemuck",
+ "libm",
+ "num-complex",
+ "reborrow",
+]
+
+[[package]]
+name = "py_literal"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "102df7a3d46db9d3891f178dcc826dc270a6746277a9ae6436f8d29fd490a8e1"
+dependencies = [
+ "num-bigint",
+ "num-complex",
+ "num-traits",
+ "pest",
+ "pest_derive",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
@@ -1057,31 +1545,31 @@
 
 [[package]]
 name = "pyo3-macros"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "pyo3-macros-backend",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "pyo3-build-config",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
 version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ce23b6b870e8f94f81fb0a363d65d86675884b34a09043c81e5562f11c1f8e1"
@@ -1091,24 +1579,84 @@
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
 ]
 
 [[package]]
 name = "r-src"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea397956e1043a8d947ea84b13971d9cb30fce65ca66a921081755ff2e899b6a"
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+
+[[package]]
+name = "rand_distr"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
+dependencies = [
+ "num-traits",
+ "rand",
+]
+
+[[package]]
+name = "raw-cpuid"
+version = "10.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c297679cb867470fa8c9f67dbba74a78d78e3e98d7cf2b08d6d71540f797332"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "reborrow"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03251193000f4bd3b042892be858ee50e8b3719f2b08e5833ac4353724632430"
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -1294,31 +1842,37 @@
 checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
+name = "seq-macro"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
+
+[[package]]
 name = "serde"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -1391,31 +1945,45 @@
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.65"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
  "unicode-ident",
 ]
 
 [[package]]
+name = "sysctl"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec7dddc5f0fee506baf8b9fdb989e242f17e4b11c61dfbb0635b705217199eea"
+dependencies = [
+ "bitflags 2.5.0",
+ "byteorder",
+ "enum-as-inner",
+ "libc",
+ "thiserror",
+ "walkdir",
+]
+
+[[package]]
 name = "tar"
 version = "0.4.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b16afcea1f22891c49a00c751c7b63b2233284064f11a200fc624137c51e2ddb"
 dependencies = [
  "filetime",
  "libc",
@@ -1451,17 +2019,17 @@
 
 [[package]]
 name = "thiserror-impl"
 version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1512,14 +2080,20 @@
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
+name = "ucd-trie"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
@@ -1638,17 +2212,17 @@
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1660,28 +2234,38 @@
 
 [[package]]
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
- "proc-macro2 1.0.83",
+ "proc-macro2 1.0.84",
  "quote 1.0.36",
- "syn 2.0.65",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
+name = "web-time"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa30049b1c872b72c89866d458eae9f20380ab280ffd1b1e18df2d3e2d98cfe0"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "webpki-roots"
 version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
 dependencies = [
  "rustls-pki-types",
 ]
@@ -1863,17 +2447,17 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
-version = "0.6.8"
+version = "0.6.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
+checksum = "86c949fede1d13936a99f14fafd3e76fd642b556dd2ce96287fbe2e0151bfac6"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
@@ -1883,10 +2467,10 @@
  "libc",
  "linux-raw-sys",
  "rustix",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
```

### Comparing `clarabel-0.8.1/LICENSE.md` & `clarabel-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/README.md` & `clarabel-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Interior Point Conic Optimization for Rust and Python
 </h1>
 <p align="center">
    <a href="https://github.com/oxfordcontrol/Clarabel.rs/actions"><img src="https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/oxfordcontrol/Clarabel.rs"><img src="https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/main/graph/badge.svg"></a>
   <a href="https://clarabel.org"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.8.0-blue.svg"></a>
+  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.9.0-blue.svg"></a>
 </p>
 
 <p align="center">
   <a href="#features">Features</a> •
   <a href="#installation">Installation</a> •
   <a href="#license-">License</a> •
   <a href="https://clarabel.org">Documentation</a>
@@ -66,9 +66,21 @@
 To use the Python interface to the solver:
 ```
 pip install clarabel
 ```
 
 To install the Python interface from source, see the [Python Installation Documentation](https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
 
+## Citing
+```
+@misc{Clarabel_2024,
+      title={Clarabel: An interior-point solver for conic programs with quadratic objectives}, 
+      author={Paul J. Goulart and Yuwen Chen},
+      year={2024},
+      eprint={2405.12762},
+      archivePrefix={arXiv},
+      primaryClass={math.OC}
+}
+```
+
 ## License 🔍
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                               [Clarabel.jl logo]
       ************ IInntteerriioorr PPooiinntt CCoonniicc OOppttiimmiizzaattiioonn ffoorr RRuusstt aanndd PPyytthhoonn ************
           _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_w_o_r_k_f_l_o_w_s_/_c_i_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_b_r_a_n_c_h_/
    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_s_t_a_b_l_e_-
 _p_u_r_p_l_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/
-                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._8_._0_-_b_l_u_e_._s_v_g_]
+                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._9_._0_-_b_l_u_e_._s_v_g_]
             _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _L_i_c_e_n_s_e â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver
 for convex optimization problems using a novel homogeneous embedding.
 Clarabel.rs solves the following problem: $$ \begin{array}{r} \text{minimize} &
 \frac{1}{2}x^T P x + q^T x\\\\[2ex] \text{subject to} & Ax + s = b \\\\[1ex] &
 s \in \mathcal{K} \end{array} $$ with decision variables $x \in \mathbb{R}^n$,
 $s \in \mathbb{R}^m$ and data matrices $P=P^\top \succeq 0$, $q \in \mathbb
@@ -31,9 +31,12 @@
 License # Installation Clarabel can be imported to Cargo based Rust projects by
 adding ```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml`
 file. To install from source, see the [Rust Installation Documentation](https:/
 /oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
 Python interface to the solver: ``` pip install clarabel ``` To install the
 Python interface from source, see the [Python Installation Documentation]
 (https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
-## License ð This project is licensed under the Apache License 2.0 - see the
-[LICENSE.md](LICENSE.md) file for details.
+## Citing ``` @misc{Clarabel_2024, title={Clarabel: An interior-point solver
+for conic programs with quadratic objectives}, author={Paul J. Goulart and
+Yuwen Chen}, year={2024}, eprint={2405.12762}, archivePrefix={arXiv},
+primaryClass={math.OC} } ``` ## License ð This project is licensed under the
+Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
```

### Comparing `clarabel-0.8.1/examples/python/example_expcone.py` & `clarabel-0.9.0/examples/python/example_expcone.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/python/example_powcone.py` & `clarabel-0.9.0/examples/python/example_powcone.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/python/example_qp.py` & `clarabel-0.9.0/examples/python/example_qp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/python/example_sdp.py` & `clarabel-0.9.0/examples/python/example_sdp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/python/example_socp.py` & `clarabel-0.9.0/examples/python/example_socp.py`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_box.rs` & `clarabel-0.9.0/examples/rust/example_box.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(non_snake_case)]
 use clarabel::algebra::*;
 use clarabel::solver::*;
 
 fn problem_data() -> (CscMatrix<f64>, Vec<f64>, CscMatrix<f64>, Vec<f64>) {
-    let n = 20000;
+    let n = 2000000;
 
     let P = CscMatrix::identity(n);
 
     // construct A = [I; -I]
     let I1 = CscMatrix::<f64>::identity(n);
     let mut I2 = CscMatrix::<f64>::identity(n);
     I2.negate();
```

### Comparing `clarabel-0.8.1/examples/rust/example_expcone.rs` & `clarabel-0.9.0/examples/rust/example_expcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_lp.rs` & `clarabel-0.9.0/examples/rust/example_lp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_powcone.rs` & `clarabel-0.9.0/examples/rust/example_powcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_qp.rs` & `clarabel-0.9.0/examples/rust/example_qp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_sdp.rs` & `clarabel-0.9.0/examples/rust/example_sdp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/examples/rust/example_socp.rs` & `clarabel-0.9.0/examples/rust/example_socp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/html/rustdocs-header.html` & `clarabel-0.9.0/html/rustdocs-header.html`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/csc/block_concatenate.rs` & `clarabel-0.9.0/src/algebra/csc/block_concatenate.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/csc/core.rs` & `clarabel-0.9.0/src/algebra/csc/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 use crate::algebra::permute;
 use crate::algebra::utils::sortperm_by;
 use crate::algebra::{Adjoint, MatrixShape, ShapedMatrix, SparseFormatError, Symmetric};
 use num_traits::Num;
 use std::iter::{repeat, zip};
 
+#[cfg(feature = "serde")]
+use serde::{de::DeserializeOwned, Deserialize, Serialize};
+
 /// Sparse matrix in standard Compressed Sparse Column (CSC) format
 ///
 /// __Example usage__ : To construct the 3 x 3 matrix
 /// ```text
 /// A = [1.  3.  5.]
 ///     [2.  0.  6.]
 ///     [0.  4.  7.]
@@ -34,14 +37,16 @@
 ///      &[[1.0, 3.0, 5.0],
 ///        [2.0, 0.0, 6.0],
 ///        [0.0, 4.0, 7.0]]);
 ///
 /// ```
 ///
 
+#[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
+#[serde(bound = "T: Serialize + DeserializeOwned")]
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub struct CscMatrix<T = f64> {
     /// number of rows
     pub m: usize,
     /// number of columns
     pub n: usize,
     /// CSC format column pointer.   
@@ -265,15 +270,15 @@
 
         self.rowval.resize(writeidx, 0);
         self.nzval.resize(writeidx, T::zero());
     }
 
     /// Return matrix data in triplet format.
     ///
-    #[cfg_attr(not(sdp), allow(dead_code))]
+    #[cfg_attr(not(feature = "sdp"), allow(dead_code))]
     pub(crate) fn findnz(&self) -> (Vec<usize>, Vec<usize>, Vec<T>) {
         let I = self.rowval.clone();
         let mut J = Vec::with_capacity(self.nnz());
         let V = self.nzval.clone();
 
         for c in 0..self.ncols() {
             let times = self.colptr[c + 1] - self.colptr[c];
```

### Comparing `clarabel-0.8.1/src/algebra/csc/matrix_math.rs` & `clarabel-0.9.0/src/algebra/csc/matrix_math.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/csc/utils.rs` & `clarabel-0.9.0/src/algebra/csc/utils.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/cholesky.rs` & `clarabel-0.9.0/src/algebra/dense/blas/cholesky.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/gemm.rs` & `clarabel-0.9.0/src/algebra/dense/blas/gemm.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/gemv.rs` & `clarabel-0.9.0/src/algebra/dense/blas/gemv.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/lu.rs` & `clarabel-0.9.0/src/algebra/dense/blas/lu.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/svd.rs` & `clarabel-0.9.0/src/algebra/dense/blas/svd.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/syevr.rs` & `clarabel-0.9.0/src/algebra/dense/blas/syevr.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/symv.rs` & `clarabel-0.9.0/src/algebra/dense/blas/symv.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/syr2k.rs` & `clarabel-0.9.0/src/algebra/dense/blas/syr2k.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/syrk.rs` & `clarabel-0.9.0/src/algebra/dense/blas/syrk.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blas/traits.rs` & `clarabel-0.9.0/src/algebra/dense/blas/traits.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/blaslike_traits.rs` & `clarabel-0.9.0/src/algebra/dense/blaslike_traits.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/block_concatenate.rs` & `clarabel-0.9.0/src/algebra/dense/block_concatenate.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/borrowed.rs` & `clarabel-0.9.0/src/algebra/dense/borrowed.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/core.rs` & `clarabel-0.9.0/src/algebra/dense/core.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/kron.rs` & `clarabel-0.9.0/src/algebra/dense/kron.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/matrix_math.rs` & `clarabel-0.9.0/src/algebra/dense/matrix_math.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/dense/types.rs` & `clarabel-0.9.0/src/algebra/dense/types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/densesym3x3/mod.rs` & `clarabel-0.9.0/src/algebra/densesym3x3/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/error_types.rs` & `clarabel-0.9.0/src/algebra/error_types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/floats.rs` & `clarabel-0.9.0/src/algebra/floats.rs`

 * *Files 15% similar despite different names*

```diff
@@ -36,61 +36,58 @@
         + Display
         + LowerExp
         + Debug
         + Sized
 {
 }
 
+// additional traits that add bounds to CoreFloatT
+// when optional dependencies are enabled
+
 // if "sdp" is enabled, we must add an additional trait
 // trait bound to restrict compilation for f32/f64 types
 // since there is no BLAS support otherwise
 
-// Define the documentation string as a macro so that FloatT gets documentation
-// regardless of whether the "sdp" feature is enabled.
-macro_rules! floatT_doc_header {
-    () => {
-        r#"Main trait for floating point types used in the Clarabel solver."#
-    };
-}
-macro_rules! floatT_doc_long {
-    () => {
-        r#"All floating point calculations in Clarabel are represented internally on values 
-         implementing the `FloatT` trait, with implementations provided only for f32 and f64 
-         native types when compiled with BLAS/LAPACK support for SDPs. If SDP support is not 
-         enabled then it should be possible to compile Clarabel to support any any other 
-         floating point type provided that it satisfies the trait bounds of `CoreFloatT`. 
-        \
-        \
-         `FloatT` relies on [`num_traits`](num_traits) for most of its constituent trait bounds."#
-    };
-}
 cfg_if::cfg_if! {
-    if #[cfg(not(feature="sdp"))] {
-    #[doc = floatT_doc_header!()]
-    ///
-    #[doc = floatT_doc_long!()]
-        pub trait FloatT: CoreFloatT {}
-    } else{
-        #[doc = floatT_doc_header!()]
-        ///
-        #[doc = floatT_doc_long!()]
-        ///
-        /// The trait bound `BlasFloatT` is only enforced when compiling with the `sdp` feature.
-        pub trait FloatT: CoreFloatT + BlasFloatT {}
+    if #[cfg(feature="sdp")] {
+        pub trait MaybeBlasFloatT : BlasFloatT {}
+        impl<T> MaybeBlasFloatT for T where T: BlasFloatT {}
+    }
+    else {
+        pub trait MaybeBlasFloatT {}
+        impl<T> MaybeBlasFloatT for T {}
     }
 }
 
+// if "faer" is enabled, we must add an additional bound
+// to restrict compilation to Reals implementing SimpleEntity
+
 cfg_if::cfg_if! {
-    if #[cfg(feature="sdp")] {
-        impl<T> FloatT for T where T: CoreFloatT + BlasFloatT {}
-    } else{
-        impl<T> FloatT for T where T: CoreFloatT {}
+    if #[cfg(feature="faer-sparse")] {
+        pub trait MaybeFaerFloatT : faer::SimpleEntity + faer::ComplexField<Real=Self> {}
+        impl<T> MaybeFaerFloatT for T where T: faer::SimpleEntity + faer::ComplexField<Real=Self> {}
+    }
+    else {
+        pub trait MaybeFaerFloatT {}
+        impl<T> MaybeFaerFloatT for T {}
     }
 }
 
+/// Main trait for floating point types used in the Clarabel solver.
+///
+/// All floating point calculations in Clarabel are represented internally on values
+/// implementing the `FloatT` trait, with implementations provided only for f32 and f64
+/// native types when compiled with BLAS/LAPACK support for SDPs. If SDP support is not
+/// enabled then it should be possible to compile Clarabel to support any any other
+/// floating point type provided that it satisfies the trait bounds of `CoreFloatT`.
+///
+/// `FloatT` relies on [`num_traits`](num_traits) for most of its constituent trait bounds.
+pub trait FloatT: CoreFloatT + MaybeBlasFloatT + MaybeFaerFloatT {}
+impl<T> FloatT for T where T: CoreFloatT + MaybeBlasFloatT + MaybeFaerFloatT {}
+
 /// Trait for convering Rust primitives to [`FloatT`](crate::algebra::FloatT)
 ///
 /// This convenience trait is implemented on f32/64 and u32/64.  This trait
 /// is required internally by the solver for converting constant primitives
 /// to [`FloatT`](crate::algebra::FloatT).  It is also used by the
 /// [user settings](crate::solver::implementations::default::DefaultSettings)
 /// for converting defaults of primitive type to [`FloatT`](crate::algebra::FloatT).
```

### Comparing `clarabel-0.8.1/src/algebra/math_traits.rs` & `clarabel-0.9.0/src/algebra/math_traits.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/matrix_traits.rs` & `clarabel-0.9.0/src/algebra/matrix_traits.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(non_snake_case)]
 
 use crate::algebra::MatrixConcatenationError;
 use crate::algebra::MatrixShape;
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) trait ShapedMatrix {
     fn shape(&self) -> MatrixShape;
     fn size(&self) -> (usize, usize);
     fn nrows(&self) -> usize {
         self.size().0
     }
     fn ncols(&self) -> usize {
```

### Comparing `clarabel-0.8.1/src/algebra/matrix_types.rs` & `clarabel-0.9.0/src/algebra/matrix_types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/mod.rs` & `clarabel-0.9.0/src/algebra/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/scalarmath.rs` & `clarabel-0.9.0/src/algebra/scalarmath.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,38 +20,38 @@
     }
 }
 
 pub(crate) fn triangular_number(k: usize) -> usize {
     (k * (k + 1)) >> 1
 }
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn triangular_index(k: usize) -> usize {
     // 0-based index into a packed triangle. Same as:
     // triangular number(k+1) - 1 = (((k+1) * (k+2)) >> 1) - 1
     (k * (k + 3)) >> 1
 }
 
 // given an index into the upper triangular part of a matrix, return
 // its row and column position
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn upper_triangular_index_to_coord(linearidx: usize) -> (usize, usize) {
     if linearidx == 0 {
         return (0, 0);
     }
 
     let col = ((isqrt(8 * linearidx + 1) + 1) >> 1) - 1;
 
     let row = linearidx - triangular_index(col - 1) - 1;
     (row, col)
 }
 
 // given a row and column position, return the index into the upper
 // triangular part of the matrix
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn coord_to_upper_triangular_index(coord: (usize, usize)) -> usize {
     if coord == (0, 0) {
         return 0;
     }
 
     let (i, j) = coord;
     if i <= j {
@@ -61,15 +61,15 @@
     }
 }
 
 // isqrt : rust does not currently have a stable isqrt yet.   See issue
 // here: https://github.com/rust-lang/rust/issues/116226
 // For now, implement a simple truncation method, which works
 // for inputs < 2^53 or so (otherwise possibly off-by-one).
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 fn isqrt(v: usize) -> usize {
     (v as f64).sqrt() as usize
 }
 
 #[test]
 fn test_triangular_number() {
     let v = vec![1, 2, 3, 4, 5, 6, 7];
```

### Comparing `clarabel-0.8.1/src/algebra/sparsevector/mod.rs` & `clarabel-0.9.0/src/algebra/sparsevector/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/tests/matrix.rs` & `clarabel-0.9.0/src/algebra/tests/matrix.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/algebra/tests/vector.rs` & `clarabel-0.9.0/src/algebra/tests/vector.rs`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,17 @@
     assert_eq!(x.norm_scaled(&s), 13.);
 }
 
 #[test]
 fn test_norm_inf() {
     let x = [-3., 4., -12.];
     assert_eq!(x.norm_inf(), 12.);
+
+    let x = [-3., f64::NAN, -12.];
+    assert!(x.norm_inf().is_nan());
 }
 
 #[test]
 fn test_norm_one() {
     let x = [-3., 4., -12.];
     assert_eq!(x.norm_one(), 19.);
 }
```

### Comparing `clarabel-0.8.1/src/algebra/utils.rs` & `clarabel-0.9.0/src/algebra/utils.rs`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 // assorted other functionality missing from std
 
 // a drop-in replacement for the julia "findall" function,
 // which serves as a vectorized version of the std::iter::position
 // returning indices of *all* elements satisfying a predicate
 
+use crate::qdldl;
 use num_traits::Num;
 use std::cmp::Ordering;
-use std::iter::zip;
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) trait PositionAll<T>: Iterator<Item = T> {
     fn position_all<F>(&mut self, predicate: F) -> Vec<usize>
     where
         F: FnMut(&T) -> bool;
 }
 
 impl<T, I> PositionAll<T> for I
@@ -30,24 +30,24 @@
             .map(|(index, _)| index)
             .collect::<Vec<_>>()
     }
 }
 
 // permutation and inverse permutation
 pub(crate) fn permute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
-    zip(p, x).for_each(|(p, x)| *x = b[*p]);
+    qdldl::permute(x, b, p);
 }
 
 #[allow(dead_code)]
 pub(crate) fn ipermute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
-    zip(p, b).for_each(|(p, b)| x[*p] = *b);
+    qdldl::ipermute(x, b, p);
 }
 
 // Construct an inverse permutation from a permutation
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn invperm(p: &[usize]) -> Vec<usize> {
     let mut b = vec![0; p.len()];
     for (i, j) in p.iter().enumerate() {
         assert!(*j < p.len() && b[*j] == 0);
         b[*j] = i;
     }
     b
@@ -59,15 +59,15 @@
     T: Sized + Ord + Copy,
 {
     assert_eq!(p.len(), v.len());
     p.iter_mut().enumerate().for_each(|(i, p)| *p = i);
     p.sort_by_key(|&k| v[k]);
 }
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn sortperm_rev<T>(p: &mut [usize], v: &[T])
 where
     T: Sized + Ord + Copy,
 {
     assert_eq!(p.len(), v.len());
     sortperm_by(p, v, |&a, &b| b.cmp(&a));
 }
@@ -82,15 +82,15 @@
     p.sort_by(|&i, &j| f(&v[i], &v[j]));
 }
 
 // PJG: maybe should be a vector trait, but T needs to admit
 // non-float types (e.g. usize).  Would require partition of the
 // vector math traits into those that require FloatT and those
 // that only require Num + Ord.
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) fn findmax<T>(v: &[T]) -> Option<usize>
 where
     T: Num + Copy + Ord,
 {
     v.iter()
         .enumerate()
         .max_by_key(|(_, &value)| value)
@@ -102,16 +102,16 @@
 
 #[test]
 fn test_position_all() {
     let test = [3, 1, 0, 5, 9];
     let idx = test.iter().position_all(|&v| *v > 2);
     assert_eq!(idx, vec![0, 3, 4]);
 
-    let idx = test.iter().position_all(|&v| *v == 2);
-    assert_eq!(idx, vec![]);
+    let idx: Vec<usize> = test.iter().position_all(|&v| *v == 2);
+    assert_eq!(idx, Vec::<usize>::new());
 }
 
 #[test]
 fn test_permute() {
     let mut x = vec![0; 5];
     let b = [6, 7, 8, 9, 10];
     let p = [2, 4, 1, 3, 0];
```

### Comparing `clarabel-0.8.1/src/algebra/vecmath.rs` & `clarabel-0.9.0/src/algebra/vecmath.rs`

 * *Files 3% similar despite different names*

```diff
@@ -113,19 +113,19 @@
     fn norm(&self) -> T {
         T::sqrt(self.sumsq())
     }
 
     // Returns infinity norm
     fn norm_inf(&self) -> T {
         let mut out = T::zero();
-        for v in self.iter().map(|v| v.abs()) {
+        for &v in self {
             if v.is_nan() {
                 return T::nan();
             }
-            out = if v > out { v } else { out };
+            out = T::max(out, v.abs());
         }
         out
     }
 
     // Returns one norm
     fn norm_one(&self) -> T {
         self.iter().fold(T::zero(), |acc, v| acc + v.abs())
```

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/src/ClarabelRs.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/src/ClarabelRs.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/src/interface.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/src/interface.jl`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,27 @@
 
 function print_timers(solver::Solver)
 
     solver_print_timers_jlrs(solver::Solver)
 
 end
 
+function write_to_file(solver::Solver, filename::String)
+
+    solver_write_to_file_jlrs(solver::Solver, filename::String)
+
+end
+
+function read_from_file(filename::String)
+
+    solver_read_from_file_jlrs(filename::String)
+
+end
+
+
 # -------------------------------------
 # Wrappers for rust-side interface  
 #--------------------------------------
 
 function solver_new_jlrs(P,q,A,b,cones,settings)
 
 
@@ -73,14 +86,15 @@
 function solver_solve_jlrs(solver::Solver)
 
     ccall(Libdl.dlsym(librust,:solver_solve_jlrs),SolutionJLRS,
         (Ptr{Cvoid},), solver.ptr)
 
 end 
 
+
 function solver_get_info_jlrs(solver::Solver)
 
     ccall(Libdl.dlsym(librust,:solver_get_info_jlrs),Clarabel.DefaultInfo{Float64},
     (Ptr{Cvoid},), solver.ptr)
     
 end
 
@@ -88,14 +102,47 @@
 function solver_print_timers_jlrs(solver::Solver)
 
     ccall(Libdl.dlsym(librust,:solver_print_timers_jlrs),Cvoid,
     (Ptr{Cvoid},), solver.ptr)
     
 end
 
+function solver_write_to_file_jlrs(solver::Solver, filename::String)
+
+    status = ccall(Libdl.dlsym(librust,:solver_write_to_file_jlrs),Cint,
+    (
+        Ptr{Cvoid},
+        Cstring
+    ), 
+        solver.ptr,
+        filename,
+    )
+
+    if status != 0
+        error("Error writing to file $filename")
+    end
+    
+end
+
+function solver_read_from_file_jlrs(filename::String)
+
+    ptr = ccall(Libdl.dlsym(librust,:solver_read_from_file_jlrs),Ptr{Cvoid},
+    (
+        Cstring,
+    ), 
+        filename,
+    )
+
+    if ptr == C_NULL
+        error("Error reading from file $filename")
+    end
+    return Solver{Float64}(ptr)
+    
+end
+
 function solver_drop_jlrs(solver::Solver)
     ccall(Libdl.dlsym(librust,:solver_drop_jlrs),Cvoid,
         (Ptr{Cvoid},), solver.ptr)
 
 end
```

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/src/types.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/src/types.jl`

 * *Files 4% similar despite different names*

```diff
@@ -103,13 +103,18 @@
 end
 
 
 mutable struct Solver{T <: Float64} <: Clarabel.AbstractSolver{Float64}
     ptr:: Ptr{Cvoid}
 
     function Solver{T}(ptr) where T
+
+        if ptr == C_NULL
+            throw(ErrorException("Solver constructor failed"))
+        end
+
         obj = new(ptr)
         finalizer(solver_drop_jlrs,obj)
         return obj
     end
 
 end
```

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/test/MOI_wrapper_tests.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/test/test_jump.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/test/test_jump.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/julia/ClarabelRs/test/test_problem_depot.jl` & `clarabel-0.9.0/src/julia/ClarabelRs/test/test_problem_depot.jl`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/julia/README.md` & `clarabel-0.9.0/src/julia/README.md`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/julia/interface.rs` & `clarabel-0.9.0/src/julia/interface.rs`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,19 @@
         cones::{SupportedConeT, SupportedConeT::*},
         IPSolver,
     },
     implementations::default::*,
 };
 use num_traits::FromPrimitive;
 use serde_json::*;
-use std::{ffi::CStr, os::raw::c_void};
+use std::fs::File;
+use std::{
+    ffi::CStr,
+    os::raw::{c_char, c_int, c_void},
+};
 
 // functions for converting solver to / from c void pointers
 
 fn to_ptr(solver: Box<DefaultSolver<f64>>) -> *mut c_void {
     Box::into_raw(solver) as *mut c_void
 }
 
@@ -50,27 +54,34 @@
 #[no_mangle]
 pub(crate) extern "C" fn solver_new_jlrs(
     P: &CscMatrixJLRS,
     q: &VectorJLRS<f64>,
     A: &CscMatrixJLRS,
     b: &VectorJLRS<f64>,
     jlcones: &VectorJLRS<ConeDataJLRS>,
-    json_settings: *const std::os::raw::c_char,
+    json_settings: *const c_char,
 ) -> *mut c_void {
     let P = P.to_CscMatrix();
     let A = A.to_CscMatrix();
     let q = Vec::from(q);
     let b = Vec::from(b);
 
     let cones = ccall_arrays_to_cones(jlcones);
-
     let settings = settings_from_json(json_settings);
 
-    let solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
+    // manually validate settings from Julia side
+    match settings.validate() {
+        Ok(_) => (),
+        Err(e) => {
+            println!("Invalid settings: {}", e);
+            return std::ptr::null_mut();
+        }
+    };
 
+    let solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
     to_ptr(Box::new(solver))
 }
 
 #[no_mangle]
 pub(crate) extern "C" fn solver_solve_jlrs(ptr: *mut c_void) -> SolutionJLRS {
     let mut solver = from_ptr(ptr);
     solver.solve();
@@ -107,14 +118,77 @@
     }
 
     // don't drop, since the memory is owned by
     // Julia and we might want to solve again
     std::mem::forget(solver);
 }
 
+// dump problem data to a file
+// returns -1 on failure, 0 on success
+#[no_mangle]
+pub(crate) extern "C" fn solver_write_to_file_jlrs(
+    ptr: *mut c_void,
+    filename: *const std::os::raw::c_char,
+) -> c_int {
+    let slice = unsafe { CStr::from_ptr(filename) };
+
+    let filename = match slice.to_str() {
+        Ok(s) => s,
+        Err(_) => {
+            return -1;
+        }
+    };
+
+    let mut file = match File::create(&filename) {
+        Ok(f) => f,
+        Err(_) => {
+            return -1;
+        }
+    };
+
+    let solver = from_ptr(ptr);
+    let status = solver.write_to_file(&mut file).is_ok();
+    let status = if status { 0 } else { -1 } as c_int;
+
+    // don't drop, since the memory is owned by Julia
+    std::mem::forget(solver);
+
+    return status;
+}
+
+// dump problem data to a file
+// returns NULL on failure, pointer to solver on success
+#[no_mangle]
+pub(crate) extern "C" fn solver_read_from_file_jlrs(
+    filename: *const std::os::raw::c_char,
+) -> *const c_void {
+    let slice = unsafe { CStr::from_ptr(filename) };
+
+    let filename = match slice.to_str() {
+        Ok(s) => s,
+        Err(_) => {
+            return std::ptr::null();
+        }
+    };
+
+    let mut file = match File::open(&filename) {
+        Ok(f) => f,
+        Err(_) => {
+            return std::ptr::null();
+        }
+    };
+
+    let solver = DefaultSolver::read_from_file(&mut file);
+
+    match solver {
+        Ok(solver) => to_ptr(Box::new(solver)),
+        Err(_) => std::ptr::null(),
+    }
+}
+
 // safely drop a solver object through its pointer.
 // called by the Julia side finalizer when a solver
 // is out of scope
 #[no_mangle]
 pub(crate) extern "C" fn solver_drop_jlrs(ptr: *mut c_void) {
     drop(from_ptr(ptr));
 }
```

### Comparing `clarabel-0.8.1/src/julia/types.rs` & `clarabel-0.9.0/src/julia/types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/lib.rs` & `clarabel-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/.gitignore` & `clarabel-0.9.0/src/python/.gitignore`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/cones_py.rs` & `clarabel-0.9.0/src/python/cones_py.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/cscmatrix_py.rs` & `clarabel-0.9.0/src/python/cscmatrix_py.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/impl_default_py.rs` & `clarabel-0.9.0/src/python/impl_default_py.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 use super::*;
 use crate::solver::{
     core::{
         traits::{InfoPrint, Settings},
         IPSolver, SolverStatus,
     },
     implementations::default::*,
+    SolverJSONReadWrite,
 };
 use num_derive::ToPrimitive;
 use num_traits::ToPrimitive;
+use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
 use std::fmt::Write;
 
 //Here we end up repeating several datatypes defined internally
 //in the Clarabel default implementation.   We would prefer
 //to just apply the PyO3 macros to autoderive these types,
 //except there are currently problems using cfg_attr with
@@ -397,20 +399,28 @@
     fn new(
         P: PyCscMatrix,
         q: Vec<f64>,
         A: PyCscMatrix,
         b: Vec<f64>,
         cones: Vec<PySupportedCone>,
         settings: PyDefaultSettings,
-    ) -> Self {
+    ) -> PyResult<Self> {
         let cones = _py_to_native_cones(cones);
         let settings = settings.to_internal();
-        let solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
 
-        Self { inner: solver }
+        //manually validate settings from Python side
+        match settings.validate() {
+            Ok(_) => (),
+            Err(e) => {
+                return Err(PyException::new_err(format!("Invalid settings: {}", e)));
+            }
+        }
+
+        let solver = DefaultSolver::new(&P, &q, &A, &b, &cones, settings);
+        Ok(Self { inner: solver })
     }
 
     fn solve(&mut self) -> PyDefaultSolution {
         self.inner.solve();
         PyDefaultSolution::new_from_internal(&self.inner.solution)
     }
 
@@ -435,8 +445,21 @@
 
     fn print_timers(&self) {
         match &self.inner.timers {
             Some(timers) => timers.print(),
             None => println!("no timers enabled"),
         };
     }
+
+    fn write_to_file(&self, filename: &str) -> PyResult<()> {
+        let mut file = std::fs::File::create(filename)?;
+        self.inner.write_to_file(&mut file)?;
+        Ok(())
+    }
+}
+
+#[pyfunction(name = "read_from_file")]
+pub fn read_from_file_py(filename: &str) -> PyResult<PyDefaultSolver> {
+    let mut file = std::fs::File::open(filename)?;
+    let solver = DefaultSolver::<f64>::read_from_file(&mut file)?;
+    Ok(PyDefaultSolver { inner: solver })
 }
```

### Comparing `clarabel-0.8.1/src/python/io.rs` & `clarabel-0.9.0/src/python/io.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/mod.rs` & `clarabel-0.9.0/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/module_py.rs` & `clarabel-0.9.0/src/python/module_py.rs`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     //module globs
     m.add_function(wrap_pyfunction!(get_infinity_py, m)?)
         .unwrap();
     m.add_function(wrap_pyfunction!(set_infinity_py, m)?)
         .unwrap();
     m.add_function(wrap_pyfunction!(default_infinity_py, m)?)
         .unwrap();
+    m.add_function(wrap_pyfunction!(read_from_file_py, m)?)
+        .unwrap();
 
     // API Cone types
     m.add_class::<PyZeroConeT>()?;
     m.add_class::<PyNonnegativeConeT>()?;
     m.add_class::<PySecondOrderConeT>()?;
     m.add_class::<PyExponentialConeT>()?;
     m.add_class::<PyPowerConeT>()?;
```

### Comparing `clarabel-0.8.1/src/python/pyblas/blas_loader.rs` & `clarabel-0.9.0/src/python/pyblas/blas_loader.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/blas_types.rs` & `clarabel-0.9.0/src/python/pyblas/blas_types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/blas_wrappers.rs` & `clarabel-0.9.0/src/python/pyblas/blas_wrappers.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/lapack_loader.rs` & `clarabel-0.9.0/src/python/pyblas/lapack_loader.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/lapack_types.rs` & `clarabel-0.9.0/src/python/pyblas/lapack_types.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/lapack_wrappers.rs` & `clarabel-0.9.0/src/python/pyblas/lapack_wrappers.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/python/pyblas/mod.rs` & `clarabel-0.9.0/src/python/pyblas/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/qdldl/qdldl.rs` & `clarabel-0.9.0/src/qdldl/qdldl.rs`

 * *Files 3% similar despite different names*

```diff
@@ -97,27 +97,27 @@
         assert!(!self.is_logical);
 
         // bomb if b is the wrong size
         assert_eq!(b.len(), self.D.len());
 
         // permute b
         let tmp = &mut self.workspace.fwork;
-        _permute(tmp, b, &self.perm);
+        permute(tmp, b, &self.perm);
 
         //solve in place with tmp as permuted RHS
         _solve(
             &self.L.colptr,
             &self.L.rowval,
             &self.L.nzval,
             &self.Dinv,
             tmp,
         );
 
         // inverse permutation to put unpermuted soln in b
-        _ipermute(b, tmp, &self.perm);
+        ipermute(b, tmp, &self.perm);
     }
 
     pub fn update_values(&mut self, indices: &[usize], values: &[T]) {
         let nzval = &mut self.workspace.triuA.nzval; // post perm internal data
         let AtoPAPt = &self.workspace.AtoPAPt; //mapping from input matrix entries to triuA
 
         for (i, &idx) in indices.iter().enumerate() {
@@ -191,28 +191,28 @@
     //is not supplied.   For no ordering at all, the
     //user would need to pass (0..n).collect() explicitly
     let (perm, iperm);
     if let Some(_perm) = opts.perm {
         iperm = _invperm(&_perm)?;
         perm = _perm;
     } else {
-        (perm, iperm) = _get_amd_ordering(Ain, opts.amd_dense_scale);
+        (perm, iperm) = get_amd_ordering(Ain, opts.amd_dense_scale);
     }
 
     //permute to (another) upper triangular matrix and store the
     //index mapping the input's entries to the permutation's entries
-    let (A, AtoPAPt) = _permute_symmetric(Ain, &iperm);
+    let (A, AtoPAPt) = permute_symmetric(Ain, &iperm);
 
     // handle the (possibly permuted) vector of
     // diagonal D signs if one was specified.  Otherwise
     // otherwise all signs are positive
     let mut Dsigns = vec![1_i8; n];
     if let Some(ds) = opts.Dsigns {
         Dsigns = vec![1_i8; n];
-        _permute(&mut Dsigns, &ds, &perm);
+        permute(&mut Dsigns, &ds, &perm);
     }
 
     // allocate workspace
     let mut workspace = QDLDLWorkspace::<T>::new(
         A,
         AtoPAPt,
         Dsigns,
@@ -448,16 +448,16 @@
     let (elim_buffer, next_colspace) = iwork.split_at_mut(n);
     let y_vals = fwork;
 
     //set Lp to cumsum(Lnz), starting from zero
     Lp[0] = 0;
     let mut acc = 0;
     for (Lp, Lnz) in zip(&mut Lp[1..], Lnz) {
-        *Lp = acc + Lnz;
-        acc = *Lp;
+        acc += Lnz;
+        *Lp = acc;
     }
 
     //  set all y_idx to be 'unused' initially
     // in each column of L, the next available space
     // to start is just the first space in the column
     y_markers.fill(QDLDL_UNUSED);
     y_vals.fill(T::zero());
@@ -567,54 +567,57 @@
                 unsafe {
                     //Safety : Here the Lij index comes from the rowval
                     //field of the sparse L factor matrix, and should
                     //always be bounded by the matrix dimension.
                     for (&Lxj, &Lij) in zip(&Lx[f..l], &Li[f..l]) {
                         *(y_vals.get_unchecked_mut(Lij)) -= Lxj * y_vals_cidx;
                     }
-                }
 
-                // Now I have the cidx^th element of y = L\b.
-                // so compute the corresponding element of
-                // this row of L and put it into the right place
-                Lx[tmp_idx] = y_vals_cidx * Dinv[cidx];
-                D[k] -= y_vals_cidx * Lx[tmp_idx];
+                    // Now I have the cidx^th element of y = L\b.
+                    // so compute the corresponding element of
+                    // this row of L and put it into the right place
+                    let Lx_tmp_idx = y_vals_cidx * *Dinv.get_unchecked(cidx);
+                    *Lx.get_unchecked_mut(tmp_idx) = Lx_tmp_idx;
+                    *D.get_unchecked_mut(k) -= y_vals_cidx * Lx_tmp_idx;
+                }
             }
 
             // record which row it went into
             Li[tmp_idx] = k;
             next_colspace[cidx] += 1;
 
             // reset the y_vals and indices back to zero and QDLDL_UNUSED
             // once I'm done with them
             y_vals[cidx] = T::zero();
             y_markers[cidx] = QDLDL_UNUSED;
         }
 
-        // apply dynamic regularization
-        if regularize_enable {
-            let sign = T::from_i8(Dsigns[k]).unwrap();
-            if D[k] * sign < regularize_eps {
-                D[k] = regularize_delta * sign;
-                *regularize_count += 1;
+        if !logical_factor {
+            // apply dynamic regularization
+            if regularize_enable {
+                let sign = T::from_i8(Dsigns[k]).unwrap();
+                if D[k] * sign < regularize_eps {
+                    D[k] = regularize_delta * sign;
+                    *regularize_count += 1;
+                }
             }
-        }
 
-        // Maintain a count of the positive entries
-        // in D.  If we hit a zero, we can't factor
-        // this matrix, so abort
-        if D[k] == T::zero() {
-            return Err(QDLDLError::ZeroPivot);
-        }
-        if D[k] > T::zero() {
-            positiveValuesInD += 1;
-        }
+            // Maintain a count of the positive entries
+            // in D.  If we hit a zero, we can't factor
+            // this matrix, so abort
+            if D[k] == T::zero() {
+                return Err(QDLDLError::ZeroPivot);
+            }
+            if D[k] > T::zero() {
+                positiveValuesInD += 1;
+            }
 
-        // compute the inverse of the diagonal
-        Dinv[k] = T::recip(D[k]);
+            // compute the inverse of the diagonal
+            Dinv[k] = T::recip(D[k]);
+        }
     } //end for k
 
     Ok(positiveValuesInD)
 }
 
 // Solves (L+I)x = b, with x replacing b (with standard bounds checks)
 fn _lsolve_safe<T: FloatT>(Lp: &[usize], Li: &[usize], Lx: &[T], x: &mut [T]) {
@@ -677,23 +680,46 @@
                 s += Lxj * (*x.get_unchecked(Lij));
             }
             *x.get_unchecked_mut(i) -= s;
         }
     }
 }
 
+// Solves D(L+I)'x = b, with x replacing b.  Unchecked version.
+fn _dltsolve_unsafe<T: FloatT>(Lp: &[usize], Li: &[usize], Lx: &[T], Dinv: &[T], x: &mut [T]) {
+    unsafe {
+        for i in (0..x.len()).rev() {
+            let mut s = T::zero();
+            let f = *Lp.get_unchecked(i);
+            let l = *Lp.get_unchecked(i + 1);
+            for (&Lxj, &Lij) in zip(&Lx[f..l], &Li[f..l]) {
+                s += Lxj * (*x.get_unchecked(Lij));
+            }
+
+            let xi = x.get_unchecked_mut(i);
+            *xi *= *Dinv.get_unchecked(i);
+            *xi -= s;
+        }
+    }
+}
+
 // Solves Ax = b where A has given LDL factors, with x replacing b
 fn _solve<T: FloatT>(Lp: &[usize], Li: &[usize], Lx: &[T], Dinv: &[T], b: &mut [T]) {
     // We call the `unsafe`d version of the forward and backward substitution
     // functions here, since the matrix data should be well posed and x of
     // compatible dimensions.   For super safety or debugging purposes, there
     // are also `safe` versions implemented above.
     _lsolve_unsafe(Lp, Li, Lx, b);
-    zip(b.iter_mut(), Dinv).for_each(|(b, d)| *b *= *d);
-    _ltsolve_unsafe(Lp, Li, Lx, b);
+
+    // combined D and L^T solve in one pass
+    _dltsolve_unsafe(Lp, Li, Lx, Dinv, b);
+
+    // in separate passes for reference
+    //zip(b.iter_mut(), Dinv).for_each(|(b, d)| *b *= *d);
+    //_ltsolve_unsafe(Lp, Li, Lx, b);
 }
 
 // Construct an inverse permutation from a permutation
 fn _invperm(p: &[usize]) -> Result<Vec<usize>, QDLDLError> {
     let mut b = vec![0; p.len()];
 
     for (i, j) in p.iter().enumerate() {
@@ -702,29 +728,40 @@
         } else {
             return Err(QDLDLError::InvalidPermutation);
         }
     }
     Ok(b)
 }
 
-// internal permutation and inverse permutation
-// functions that require no memory allocations
+// permutation and inverse permutation
+// functions that require no allocation
+// p must be a valid permutation vector
+// in both cases for safety
 
-fn _permute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
-    zip(p, x).for_each(|(p, x)| *x = b[*p]);
+pub(crate) fn permute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
+    debug_assert!(*p.iter().max().unwrap_or(&0) < x.len());
+    unsafe {
+        zip(p, x).for_each(|(p, x)| *x = *b.get_unchecked(*p));
+    }
 }
 
-fn _ipermute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
-    zip(p, b).for_each(|(p, b)| x[*p] = *b);
+pub(crate) fn ipermute<T: Copy>(x: &mut [T], b: &[T], p: &[usize]) {
+    debug_assert!(*p.iter().max().unwrap_or(&0) < x.len());
+    unsafe {
+        zip(p, b).for_each(|(p, b)| *x.get_unchecked_mut(*p) = *b);
+    }
 }
 
 // Given a sparse symmetric matrix `A` (with only upper triangular entries), return
 // permuted sparse symmetric matrix `P` (also only upper triangular) given the
 // inverse permutation vector `iperm`."
-fn _permute_symmetric<T: FloatT>(A: &CscMatrix<T>, iperm: &[usize]) -> (CscMatrix<T>, Vec<usize>) {
+pub(crate) fn permute_symmetric<T: FloatT>(
+    A: &CscMatrix<T>,
+    iperm: &[usize],
+) -> (CscMatrix<T>, Vec<usize>) {
     // perform a number of argument checks
     let (_m, n) = A.size();
     let mut P = CscMatrix::<T>::spalloc((n, n), A.nnz());
 
     // we will record a mapping of entries from A to PAPt
     let mut AtoPAPt = vec![0; A.nnz()];
 
@@ -812,15 +849,15 @@
                 // increment next free location
                 row_starts[col_idx] += 1;
             }
         }
     }
 }
 
-fn _get_amd_ordering<T: FloatT>(
+pub(crate) fn get_amd_ordering<T: FloatT>(
     A: &CscMatrix<T>,
     amd_dense_scale: f64,
 ) -> (Vec<usize>, Vec<usize>) {
     // PJG: For interested readers - setting amd_dense_scale to 1.5 seems to work better
     // for KKT systems in QP problems, but this ad hoc method can surely be improved
 
     // computes a permutation for A using AMD default parameters
```

### Comparing `clarabel-0.8.1/src/qdldl/test.rs` & `clarabel-0.9.0/src/qdldl/test.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 #[test]
 fn test_permute() {
     let perm = vec![3, 0, 2, 1]; //index too big
     let b = vec![1., 2., 3., 4.];
     let mut x = vec![0.; 4];
     let mut y = vec![0.; 4];
 
-    _permute(&mut x, &b, &perm);
+    permute(&mut x, &b, &perm);
     assert_eq!(x, vec![4., 1., 3., 2.]);
 
-    _ipermute(&mut y, &x, &perm);
+    ipermute(&mut y, &x, &perm);
     assert_eq!(y, b);
 }
 
 #[test]
 fn test_solve_from_factors() {
     //L =
     //[ ⋅    ⋅     ⋅    ⋅ ]
@@ -120,25 +120,25 @@
 
     assert_eq!(etree, vec![1, 2, 3, QDLDL_UNKNOWN]);
 }
 
 #[test]
 fn test_amd() {
     let A = test_matrix_4x4();
-    let (perm, iperm) = _get_amd_ordering(&A, 1.5);
+    let (perm, iperm) = get_amd_ordering(&A, 1.5);
     assert_eq!(perm, [3, 0, 1, 2]);
     assert_eq!(iperm, [1, 2, 3, 0]);
 }
 
 #[test]
 fn test_permute_symmetric() {
     //no permutation at all
     let A = test_matrix_4x4();
     let iperm: Vec<usize> = vec![0, 1, 2, 3];
-    let (P, AtoPAPt) = _permute_symmetric(&A, &iperm);
+    let (P, AtoPAPt) = permute_symmetric(&A, &iperm);
 
     assert_eq!(&A.colptr, &P.colptr);
     assert_eq!(&A.rowval, &P.rowval);
     assert_eq!(&A.nzval, &P.nzval);
     let linearidx: Vec<usize> = (0..AtoPAPt.len()).collect();
     assert_eq!(&linearidx, &AtoPAPt);
 
@@ -153,15 +153,15 @@
     //set the problem data to increasing values columnwise
     for i in 0..A.nzval.len() {
         A.nzval[i] = i as f64 + 1.;
     }
 
     let perm: Vec<usize> = vec![2, 3, 0, 1];
     let iperm = _invperm(&perm).unwrap();
-    let (P, _) = _permute_symmetric(&A, &iperm);
+    let (P, _) = permute_symmetric(&A, &iperm);
 
     assert_eq!(&P.colptr, &vec![0, 1, 3, 5, 8]);
     assert_eq!(&P.rowval, &vec![0, 0, 1, 2, 0, 2, 3, 0]);
     assert_eq!(&P.nzval, &vec![6.0, 7.0, 8.0, 1.0, 4.0, 2.0, 3.0, 5.0]);
 }
 
 #[test]
```

### Comparing `clarabel-0.8.1/src/solver/chordal/chordal_info.rs` & `clarabel-0.9.0/src/solver/chordal/chordal_info.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/augment_compact.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/augment_compact.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/augment_standard.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/augment_standard.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/mod.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/psd_completion.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/psd_completion.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/reverse_compact.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/reverse_compact.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/decomp/reverse_standard.rs` & `clarabel-0.9.0/src/solver/chordal/decomp/reverse_standard.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/merge/clique_graph.rs` & `clarabel-0.9.0/src/solver/chordal/merge/clique_graph.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/merge/disjoint_set_union.rs` & `clarabel-0.9.0/src/solver/chordal/merge/disjoint_set_union.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/merge/mod.rs` & `clarabel-0.9.0/src/solver/chordal/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/merge/nomerge.rs` & `clarabel-0.9.0/src/solver/chordal/merge/nomerge.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/merge/parent_child.rs` & `clarabel-0.9.0/src/solver/chordal/merge/parent_child.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/sparsity_pattern.rs` & `clarabel-0.9.0/src/solver/chordal/sparsity_pattern.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/chordal/supernode_tree.rs` & `clarabel-0.9.0/src/solver/chordal/supernode_tree.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/compositecone.rs` & `clarabel-0.9.0/src/solver/core/cones/compositecone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/expcone.rs` & `clarabel-0.9.0/src/solver/core/cones/expcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/genpowcone.rs` & `clarabel-0.9.0/src/solver/core/cones/genpowcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/mod.rs` & `clarabel-0.9.0/src/solver/core/cones/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/nonnegativecone.rs` & `clarabel-0.9.0/src/solver/core/cones/nonnegativecone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/nonsymmetric_common.rs` & `clarabel-0.9.0/src/solver/core/cones/nonsymmetric_common.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/powcone.rs` & `clarabel-0.9.0/src/solver/core/cones/powcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/psdtrianglecone.rs` & `clarabel-0.9.0/src/solver/core/cones/psdtrianglecone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/socone.rs` & `clarabel-0.9.0/src/solver/core/cones/socone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/supportedcone.rs` & `clarabel-0.9.0/src/solver/core/cones/supportedcone.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 use super::*;
 
 #[cfg(feature = "sdp")]
 use crate::algebra::triangular_number;
+#[cfg(feature = "serde")]
+use serde::{Deserialize, Serialize};
 
 // ---------------------------------------------------
 // We define some machinery here for enumerating the
 // different cone types that can live in the composite cone
 // ---------------------------------------------------
 
 /// API type describing the type of a conic constraint.
-///  
+///
+#[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 #[derive(Debug, Clone)]
 pub enum SupportedConeT<T> {
     /// The zero cone (used for equality constraints).
     ///
     /// The parameter indicates the cones dimension.
     ZeroConeT(usize),
     /// The nonnegative orthant.  
@@ -196,22 +199,22 @@
 
 // ----------------------------------------------
 // Iterator for the range of indices of the cone
 
 //PJG: type names are not satisfactory.   Try to combine
 //with the internal cone generators.
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) struct RangeSupportedConesIterator<'a, T> {
     cones: &'a [SupportedConeT<T>],
     index: usize,
     start: usize,
 }
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 impl<'a, T> Iterator for RangeSupportedConesIterator<'a, T> {
     type Item = std::ops::Range<usize>;
 
     fn next(&mut self) -> Option<Self::Item> {
         if self.index < self.cones.len() {
             let cone = &self.cones[self.index];
             let stop = self.start + cone.nvars();
@@ -220,20 +223,20 @@
             self.start = stop;
             Some(range)
         } else {
             None
         }
     }
 }
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 pub(crate) trait ConeRanges<'a, T> {
     fn rng_cones_iter(&'a self) -> RangeSupportedConesIterator<'a, T>;
 }
 
-#[cfg_attr(not(sdp), allow(dead_code))]
+#[cfg_attr(not(feature = "sdp"), allow(dead_code))]
 impl<'a, T> ConeRanges<'a, T> for [SupportedConeT<T>] {
     fn rng_cones_iter(&'a self) -> RangeSupportedConesIterator<'a, T> {
         RangeSupportedConesIterator::<'a, T> {
             cones: self,
             index: 0,
             start: 0,
         }
```

### Comparing `clarabel-0.8.1/src/solver/core/cones/symmetric_common.rs` & `clarabel-0.9.0/src/solver/core/cones/symmetric_common.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/cones/zerocone.rs` & `clarabel-0.9.0/src/solver/core/cones/zerocone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/datamaps.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/directldlkktsolver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #![allow(non_snake_case)]
 
+#[cfg(feature = "faer-sparse")]
+use super::ldlsolvers::faer_ldl::*;
+
 use super::ldlsolvers::qdldl::*;
 use super::*;
 use crate::solver::core::kktsolvers::KKTSolver;
 use crate::solver::core::{cones::*, CoreSettings};
 use std::iter::zip;
 
 // -------------------------------------
@@ -341,16 +344,18 @@
     let kktshape: MatrixTriangle;
 
     match settings.direct_solve_method.as_str() {
         "qdldl" => {
             kktshape = QDLDLDirectLDLSolver::<T>::required_matrix_shape();
             ldlptr = |M, D, S| Box::new(QDLDLDirectLDLSolver::<T>::new(M, D, S));
         }
-        "custom" => {
-            unimplemented!();
+        #[cfg(feature = "faer-sparse")]
+        "faer" => {
+            kktshape = FaerDirectLDLSolver::<T>::required_matrix_shape();
+            ldlptr = |M, D, S| Box::new(FaerDirectLDLSolver::<T>::new(M, D, S));
         }
         _ => {
             panic! {"Unrecognized LDL solver type"};
         }
     }
     (kktshape, ldlptr)
 }
```

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/kkt_assembly.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/ldlsolvers/qdldl.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/direct/quasidef/mod.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/direct/quasidef/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/kktsolvers/mod.rs` & `clarabel-0.9.0/src/solver/core/kktsolvers/mod.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/core/solver.rs` & `clarabel-0.9.0/src/solver/core/solver.rs`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,22 @@
 
 impl std::fmt::Display for SolverStatus {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
         write!(f, "{:?}", self)
     }
 }
 
+/// JSON file read/write trait for solver data.
+/// Only available with the "serde" feature enabled.
+#[cfg(feature = "serde")]
+pub trait SolverJSONReadWrite: Sized {
+    fn write_to_file(&self, file: &mut std::fs::File) -> Result<(), std::io::Error>;
+    fn read_from_file(file: &mut std::fs::File) -> Result<Self, std::io::Error>;
+}
+
 // ---------------------------------
 // top level solver container type
 // ---------------------------------
 
 // The top-level solver.
 
 // This trait is defined with a collection of mutually interacting associated types.
```

### Comparing `clarabel-0.8.1/src/solver/core/traits.rs` & `clarabel-0.9.0/src/solver/core/traits.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/data_updating.rs` & `clarabel-0.9.0/src/solver/implementations/default/data_updating.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/equilibration.rs` & `clarabel-0.9.0/src/solver/implementations/default/equilibration.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/info.rs` & `clarabel-0.9.0/src/solver/implementations/default/info.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/info_print.rs` & `clarabel-0.9.0/src/solver/implementations/default/info_print.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/kktsystem.rs` & `clarabel-0.9.0/src/solver/implementations/default/kktsystem.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/mod.rs` & `clarabel-0.9.0/src/solver/implementations/default/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 pub use presolver::*;
 pub use problemdata::*;
 pub use residuals::*;
 pub use settings::*;
 pub use solution::*;
 pub use solver::*;
 pub use variables::*;
+
+#[cfg(feature = "serde")]
+mod json;
```

### Comparing `clarabel-0.8.1/src/solver/implementations/default/presolver.rs` & `clarabel-0.9.0/src/solver/implementations/default/presolver.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/problemdata.rs` & `clarabel-0.9.0/src/solver/implementations/default/problemdata.rs`

 * *Files 0% similar despite different names*

```diff
@@ -354,16 +354,16 @@
 
     Some(presolver)
 }
 
 // -- utility function that tries to unwrap and slice a vector, or return
 // an alternative.   Necessary since the Options for q and b are &Vec, but
 // the user supplied data is a slice &[T]
-
-pub fn unwrap_and_slice_or_else<'a, T, F>(opt: &'a Option<Vec<T>>, f: F) -> &'a [T]
+#[cfg(feature = "sdp")]
+pub(crate) fn unwrap_and_slice_or_else<'a, T, F>(opt: &'a Option<Vec<T>>, f: F) -> &'a [T]
 where
     F: FnOnce() -> &'a [T],
     T: FloatT,
 {
     if opt.is_some() {
         opt.as_ref().unwrap().as_slice()
     } else {
```

### Comparing `clarabel-0.8.1/src/solver/implementations/default/residuals.rs` & `clarabel-0.9.0/src/solver/implementations/default/residuals.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/solution.rs` & `clarabel-0.9.0/src/solver/implementations/default/solution.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/solver.rs` & `clarabel-0.9.0/src/solver/implementations/default/solver.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/implementations/default/variables.rs` & `clarabel-0.9.0/src/solver/implementations/default/variables.rs`

 * *Files 0% similar despite different names*

```diff
@@ -279,12 +279,12 @@
         self.z.hadamard(e).scale(scaleinv / cscale);
         self.s.hadamard(einv).scale(scaleinv);
 
         self.τ *= scaleinv;
         self.κ *= scaleinv;
     }
 
-    #[cfg_attr(not(sdp), allow(dead_code))]
+    #[cfg_attr(not(feature = "sdp"), allow(dead_code))]
     pub(crate) fn dims(&self) -> (usize, usize) {
         (self.x.len(), self.s.len())
     }
 }
```

### Comparing `clarabel-0.8.1/src/solver/mod.rs` & `clarabel-0.9.0/src/solver/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 //user facing traits required to interact with solver
 pub use crate::solver::core::{IPSolver, SolverStatus};
 
 //user facing traits required to define new implementatiions
 pub use crate::solver::core::traits;
 pub use crate::solver::core::CoreSettings;
 
-//If we had implementations for multple alternative
+// read/write types if enabled
+#[cfg(feature = "serde")]
+pub use crate::solver::core::SolverJSONReadWrite;
+
+//If we had implementations for multiple alternative
 //problem formats, they would live here.   Since we
 //only have default, it is exposed at the top level
 //in the use statements directly below instead.
 
 // pub mod implementations {
 //     pub mod default {
 //         pub use clarabel_solver::implementations::default::*;
```

### Comparing `clarabel-0.8.1/src/solver/tests/cones.rs` & `clarabel-0.9.0/src/solver/tests/cones.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/utils/atomic.rs` & `clarabel-0.9.0/src/solver/utils/atomic.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/solver/utils/infbounds.rs` & `clarabel-0.9.0/src/solver/utils/infbounds.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/src/timers/timers.rs` & `clarabel-0.9.0/src/timers/timers.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 use std::collections::HashMap;
 use std::ops::{Deref, DerefMut};
-use std::time::{Duration, Instant};
+
+cfg_if::cfg_if! {
+    if #[cfg(feature="wasm")] {
+        use web_time::{Duration, Instant};
+    }
+    else {
+        use std::time::{Duration, Instant};
+    }
+}
+        
 
 #[derive(Debug, Default)]
 struct InnerTimer {
     start: Option<Instant>,
     elapsed: Duration,
     subtimers: SubTimersMap,
 }
```

### Comparing `clarabel-0.8.1/tests/api_dimension_checks.rs` & `clarabel-0.9.0/tests/api_dimension_checks.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_eq_constrained.rs` & `clarabel-0.9.0/tests/basic_eq_constrained.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_expcone.rs` & `clarabel-0.9.0/tests/basic_expcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_genpowcone.rs` & `clarabel-0.9.0/tests/basic_genpowcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_lp.rs` & `clarabel-0.9.0/tests/basic_lp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_powcone.rs` & `clarabel-0.9.0/tests/basic_powcone.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_qp.rs` & `clarabel-0.9.0/tests/basic_qp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_sdp.rs` & `clarabel-0.9.0/tests/basic_sdp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_socp.rs` & `clarabel-0.9.0/tests/basic_socp.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/basic_unconstrained.rs` & `clarabel-0.9.0/tests/basic_unconstrained.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/data_updating.rs` & `clarabel-0.9.0/tests/data_updating.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/equilibration_bounds.rs` & `clarabel-0.9.0/tests/equilibration_bounds.rs`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,24 @@
     let (P, c, mut A, b, cones) = equilibration_test_data();
     let settings = DefaultSettings::default();
 
     A.nzval[0] = 1e+15;
 
     let mut solver = DefaultSolver::new(&P, &c, &A, &b, &cones, settings.clone());
 
-    solver.solve();
-
     let d = &solver.data.equilibration.d;
     let e = &solver.data.equilibration.e;
 
     assert!(d.minimum() >= settings.equilibrate_min_scaling);
     assert!(e.minimum() >= settings.equilibrate_min_scaling);
     assert!(d.maximum() <= settings.equilibrate_max_scaling);
     assert!(e.maximum() <= settings.equilibrate_max_scaling);
+
+    // forces poorly converging test for codecov
+    solver.solve();
 }
 
 #[test]
 fn test_equilibrate_zero_rows() {
     let (P, c, mut A, b, cones) = equilibration_test_data();
     let settings = DefaultSettings::default();
```

### Comparing `clarabel-0.8.1/tests/mixed_conic.rs` & `clarabel-0.9.0/tests/mixed_conic.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/presolve.rs` & `clarabel-0.9.0/tests/presolve.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/tests/sdp_chordal.rs` & `clarabel-0.9.0/tests/sdp_chordal.rs`

 * *Files identical despite different names*

### Comparing `clarabel-0.8.1/PKG-INFO` & `clarabel-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: clarabel
-Version: 0.8.1
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Requires-Dist: numpy
 Requires-Dist: scipy
 License-File: LICENSE.md
 Summary: Clarabel Conic Interior Point Solver for Rust / Python
 Keywords: convex,optimization,conic,solver,linear-programming
 Author: Paul Goulart <paul.goulart@eng.ox.ac.uk>
@@ -24,15 +24,15 @@
 Interior Point Conic Optimization for Rust and Python
 </h1>
 <p align="center">
    <a href="https://github.com/oxfordcontrol/Clarabel.rs/actions"><img src="https://github.com/oxfordcontrol/Clarabel.rs/workflows/ci/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/oxfordcontrol/Clarabel.rs"><img src="https://codecov.io/gh/oxfordcontrol/Clarabel.rs/branch/main/graph/badge.svg"></a>
   <a href="https://clarabel.org"><img src="https://img.shields.io/badge/Documentation-stable-purple.svg"></a>
   <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"></a>
-  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.8.0-blue.svg"></a>
+  <a href="https://github.com/oxfordcontrol/Clarabel.rs/releases"><img src="https://img.shields.io/badge/Release-v0.9.0-blue.svg"></a>
 </p>
 
 <p align="center">
   <a href="#features">Features</a> •
   <a href="#installation">Installation</a> •
   <a href="#license-">License</a> •
   <a href="https://clarabel.org">Documentation</a>
@@ -82,10 +82,22 @@
 To use the Python interface to the solver:
 ```
 pip install clarabel
 ```
 
 To install the Python interface from source, see the [Python Installation Documentation](https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
 
+## Citing
+```
+@misc{Clarabel_2024,
+      title={Clarabel: An interior-point solver for conic programs with quadratic objectives}, 
+      author={Paul J. Goulart and Yuwen Chen},
+      year={2024},
+      eprint={2405.12762},
+      archivePrefix={arXiv},
+      primaryClass={math.OC}
+}
+```
+
 ## License 🔍
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.3 Name: clarabel Version: 0.8.1 Classifier: Programming
+Metadata-Version: 2.3 Name: clarabel Version: 0.9.0 Classifier: Programming
 Language :: Rust Requires-Dist: numpy Requires-Dist: scipy License-File:
 LICENSE.md Summary: Clarabel Conic Interior Point Solver for Rust / Python
 Keywords: convex,optimization,conic,solver,linear-programming Author: Paul
 Goulart
 eng.ox.ac.uk> Author-email: Paul Goulart
 eng.ox.ac.uk> License: Apache-2.0 Requires-Python: >=3.7 Description-Content-
 Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Source Code,
 https://github.com/oxfordcontrol/Clarabel.rs
                               [Clarabel.jl logo]
       ************ IInntteerriioorr PPooiinntt CCoonniicc OOppttiimmiizzaattiioonn ffoorr RRuusstt aanndd PPyytthhoonn ************
           _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_w_o_r_k_f_l_o_w_s_/_c_i_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_o_x_f_o_r_d_c_o_n_t_r_o_l_/_C_l_a_r_a_b_e_l_._r_s_/_b_r_a_n_c_h_/
    _m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_D_o_c_u_m_e_n_t_a_t_i_o_n_-_s_t_a_b_l_e_-
 _p_u_r_p_l_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/
-                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._8_._0_-_b_l_u_e_._s_v_g_]
+                _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_l_e_a_s_e_-_v_0_._9_._0_-_b_l_u_e_._s_v_g_]
             _F_e_a_t_u_r_e_s â¢ _I_n_s_t_a_l_l_a_t_i_o_n â¢ _L_i_c_e_n_s_e â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 __Clarabel.rs__ is a Rust implementation of an interior point numerical solver
 for convex optimization problems using a novel homogeneous embedding.
 Clarabel.rs solves the following problem: $$ \begin{array}{r} \text{minimize} &
 \frac{1}{2}x^T P x + q^T x\\\\[2ex] \text{subject to} & Ax + s = b \\\\[1ex] &
 s \in \mathcal{K} \end{array} $$ with decision variables $x \in \mathbb{R}^n$,
 $s \in \mathbb{R}^m$ and data matrices $P=P^\top \succeq 0$, $q \in \mathbb
@@ -40,9 +40,12 @@
 License # Installation Clarabel can be imported to Cargo based Rust projects by
 adding ```rust [dependencies] clarabel = "0" ``` to the project's `Cargo.toml`
 file. To install from source, see the [Rust Installation Documentation](https:/
 /oxfordcontrol.github.io/ClarabelDocs/stable/rust/installation_rs/). To use the
 Python interface to the solver: ``` pip install clarabel ``` To install the
 Python interface from source, see the [Python Installation Documentation]
 (https://oxfordcontrol.github.io/ClarabelDocs/stable/python/installation_py/).
-## License ð This project is licensed under the Apache License 2.0 - see the
-[LICENSE.md](LICENSE.md) file for details.
+## Citing ``` @misc{Clarabel_2024, title={Clarabel: An interior-point solver
+for conic programs with quadratic objectives}, author={Paul J. Goulart and
+Yuwen Chen}, year={2024}, eprint={2405.12762}, archivePrefix={arXiv},
+primaryClass={math.OC} } ``` ## License ð This project is licensed under the
+Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
```

