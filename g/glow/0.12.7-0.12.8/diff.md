# Comparing `tmp/glow-0.12.7.tar.gz` & `tmp/glow-0.12.8.tar.gz`

## Comparing `glow-0.12.7.tar` & `glow-0.12.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/examples/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.7/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.7/examples/gan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/__init__.py
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/cli.pyi
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/distributed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/api/exporting.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_coro.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_import_hook.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_more.py
--rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_parallel.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_parallel.pyi
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_print.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_patch_scipy.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_profile.pyi
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_reduction.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_repr.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_sizeof.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_thread_quota.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/_uuid.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/debug.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/__init__.py
--rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/cache.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/cache.pyi
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/concurrency.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/concurrency.pyi
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/reusable.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/core/wrap/util.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/io/_svg.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/base.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/confusion.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/metrics/raw.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/__init__.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_loader.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_sampler.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/_trainer.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/amp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/driver.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/functional.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/optimizers.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/plot.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/proto.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/util.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/__init__.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/aggregates.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/context.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/convnets.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/lazy.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/simple.py
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/transformers.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/util.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/__init__.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/classes.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.7/src/glow/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.7/test/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.7/test/run_metrics.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_buffered.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_iter.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_loader.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_shm.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.7/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.7/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.7/README.md
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 glow-0.12.7/pyproject.toml
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 glow-0.12.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.8/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.8/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.8/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_more.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/debug.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0    10126 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.8/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.8/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.8/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_iter.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.8/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.8/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.8/README.md
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 glow-0.12.8/pyproject.toml
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 glow-0.12.8/PKG-INFO
```

### Comparing `glow-0.12.7/examples/cifar10.py` & `glow-0.12.8/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/cli.py` & `glow-0.12.8/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/cli.pyi` & `glow-0.12.8/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/distributed.py` & `glow-0.12.8/src/glow/distributed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/api/config.py` & `glow-0.12.8/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/api/exporting.py` & `glow-0.12.8/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/__init__.py` & `glow-0.12.8/src/glow/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_coro.py` & `glow-0.12.8/src/glow/core/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_import_hook.py` & `glow-0.12.8/src/glow/core/_import_hook.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,43 +12,59 @@
 _HookVar = TypeVar('_HookVar', bound=_Hook)
 
 _INITIALIZED = False
 _LOCK = RLock()
 _HOOKS: dict[str, list[_Hook]] = {}
 
 
-class _ImportHookChainedLoader:
+class _ImportHookChainedLoader(abc.Loader):
     def __init__(self, loader):
         self.loader = loader
 
-    def load_module(self, fullname):
-        module = self.loader.load_module(fullname)
+    def _set_loader(self, module):
+        undefined = object()
+        if getattr(module, '__loader__', undefined) in (None, self):
+            try:
+                module.__loader__ = self.loader
+            except AttributeError:
+                pass
+
+        if ((spec := getattr(module, '__spec__', None)) is not None
+                and getattr(spec, 'loader', None) is self):
+            spec.loader = self.loader
+
+    def create_module(self, spec):
+        return self.loader.create_module(spec)
+
+    def exec_module(self, module):
+        self._set_loader(module)
+        self.loader.exec_module(module)
 
+        name: str | None = getattr(module, '__name__', None)
         with _LOCK:
-            name = getattr(module, '__name__', None)
-            if hooks := _HOOKS.get(name):  # type: ignore[arg-type]
-                while hooks:
-                    hooks.pop()(module)
-
-        return module
+            hooks = _HOOKS.pop(name, [])  # type: ignore[arg-type]
+        for hook in hooks:
+            hook(module)
 
 
-class _ImportHookFinder(abc.MetaPathFinder, set):
-    def find_module(self, fullname, path=None):
+class _ImportHookFinder(abc.MetaPathFinder, set[str]):
+    def find_spec(self, fullname: str, path, target=None):
         with _LOCK:
             if fullname not in _HOOKS or fullname in self:
                 return None
 
-            self.add(fullname)
-            try:
-                if (spec := util.find_spec(fullname)) and spec.loader:
-                    return _ImportHookChainedLoader(spec.loader)
-            finally:
-                self.remove(fullname)
-            return None
+        self.add(fullname)
+        try:
+            if ((spec := util.find_spec(fullname)) and (loader := spec.loader)
+                    and not isinstance(loader, _ImportHookChainedLoader)):
+                spec.loader = _ImportHookChainedLoader(loader)
+                return spec
+        finally:
+            self.remove(fullname)
+        return None
 
 
 def register_post_import_hook(hook: _Hook, name: str) -> None:
     """Register a new post import hook for the target module name.
 
     This will result in a proxy callback being registered which will defer
     loading of the specified module containing the callback function until
```

### Comparing `glow-0.12.7/src/glow/core/_more.py` & `glow-0.12.8/src/glow/core/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_parallel.py` & `glow-0.12.8/src/glow/core/_parallel.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_parallel.pyi` & `glow-0.12.8/src/glow/core/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_patch_len.py` & `glow-0.12.8/src/glow/core/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_patch_print.py` & `glow-0.12.8/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_patch_scipy.py` & `glow-0.12.8/src/glow/core/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_profile.py` & `glow-0.12.8/src/glow/core/_profile.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_profile.pyi` & `glow-0.12.8/src/glow/core/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_reduction.py` & `glow-0.12.8/src/glow/core/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_repr.py` & `glow-0.12.8/src/glow/core/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_sizeof.py` & `glow-0.12.8/src/glow/core/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_thread_quota.py` & `glow-0.12.8/src/glow/core/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/_uuid.py` & `glow-0.12.8/src/glow/core/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/debug.py` & `glow-0.12.8/src/glow/core/debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/wrap/cache.py` & `glow-0.12.8/src/glow/core/wrap/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,68 +230,87 @@
         for key, job in jobs.items():
             evict(key)
             job.future.set_exception(exc)
 
 
 def _memoize_batched_aio(key_fn: _KeyFn, fn: _BatchedFn) -> _BatchedFn:
     assert callable(fn)
-    cache: dict[Hashable, asyncio.Future] = {}
+    futs: dict[Hashable, asyncio.Future] = {}
     queue: dict[Hashable, _Job] = {}
     loop = make_loop()
 
     def _load(token) -> asyncio.Future:
         key = key_fn(token)
-        if result := cache.get(key):
+        if result := futs.get(key):
             return result
 
         loop = asyncio.get_running_loop()
-        cache[key] = future = loop.create_future()
+        futs[key] = future = loop.create_future()
         queue[key] = _Job(token, future)
         if len(queue) == 1:
-            loop.call_soon(_dispatch, fn, cache, queue)
+            loop.call_soon(_dispatch, fn, futs.pop, queue)
 
         return future
 
     async def _load_many(tokens: Iterable) -> tuple:
         return await asyncio.gather(*map(_load, tokens))
 
     def wrapper(tokens: Iterable) -> tuple:
         coro = _load_many(tokens)
         return asyncio.run_coroutine_threadsafe(coro, loop).result()
 
-    wrapper.cache = cache  # type: ignore[attr-defined]
+    wrapper.stage = futs  # type: ignore[attr-defined]
     return cast(_BatchedFn, functools.update_wrapper(wrapper, fn))
 
 
-def _memoize_batched(key_fn: _KeyFn, fn: _BatchedFn) -> _BatchedFn:
+def _memoize_batched(cache: _DictMixin, key_fn: _KeyFn,
+                     fn: _BatchedFn) -> _BatchedFn:
     assert callable(fn)
     lock = RLock()
-    cache: dict[Hashable, cf.Future] = {}
+    futs = WeakValueDictionary[Hashable, cf.Future]()
     queue: dict[Hashable, _Job] = {}
 
-    def _load(stack: ExitStack, token: object) -> cf.Future:
-        key = key_fn(token)
+    def _load(stack: ExitStack, key: Hashable, token: object) -> cf.Future:
         with lock:
-            if result := cache.get(key):
+            if result := futs.get(key):
                 return result
 
-            cache[key] = future = cf.Future()  # type: ignore[var-annotated]
+            futs[key] = future = cf.Future()  # type: ignore[var-annotated]
             queue[key] = _Job(token, future)
             if len(queue) == 1:
-                stack.callback(_dispatch, fn, cache.pop, queue)
+                stack.callback(_dispatch, fn, futs.pop, queue)
 
         return future
 
     def wrapper(tokens: Iterable) -> list:
-        futs = []
+        keyed_tokens = [(key_fn(t), t) for t in tokens]
+
+        # Try to hit
+        misses = {}
+        hits = {}
+        with cache.lock:
+            for k, t in dict(keyed_tokens).items():
+                if (r := cache[k]) is not _empty:
+                    hits[k] = r
+                else:
+                    misses[k] = t
+
+        futs: dict[Hashable, cf.Future] = {}
         with ExitStack() as stack:
-            futs += [_load(stack, token) for token in tokens]
-        return [fut.result() for fut in futs]
+            futs |= {k: _load(stack, k, t) for k, t in misses.items()}
+        cf.wait(futs.values(), return_when='FIRST_EXCEPTION')
+
+        # Process misses
+        with cache.lock:
+            for k, f in futs.items():
+                hits[k] = cache[k] = f.result()
+        return [hits[k] for k, _ in keyed_tokens]
 
     wrapper.cache = cache  # type: ignore[attr-defined]
+    wrapper.stage = futs  # type: ignore[attr-defined]
     return cast(_BatchedFn, functools.update_wrapper(wrapper, fn))
 
 
 # ----------------------------- factory wrappers -----------------------------
 
 
 def memoize(
@@ -319,15 +338,15 @@
         'raw': _HeapCache,
         'lru': _LruCache,
         'mru': _MruCache,
     }
     size_fn = sizeof if bytesize else _unit_size
 
     if (cache_cls := caches.get(policy)) is not None:
-        if batched:
-            return functools.partial(_memoize_batched, key_fn)
         if capacity < 0:
             cache_cls = _HeapCache
-        return functools.partial(_memoize, cache_cls(capacity, size_fn),
-                                 key_fn)
+        cache = cache_cls(capacity, size_fn)
+        if batched:
+            return functools.partial(_memoize_batched, cache, key_fn)
+        return functools.partial(_memoize, cache, key_fn)
     raise ValueError(f'Unknown policy: "{policy}". '
                      f'Only "{set(caches)}" are available')
```

### Comparing `glow-0.12.7/src/glow/core/wrap/cache.pyi` & `glow-0.12.8/src/glow/core/wrap/cache.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 _KeyFn: TypeAlias = Callable[..., Hashable]
 
 
 @overload
 def memoize(capacity: int,
             *,
             policy: _Policy = ...,
-            key_fn: _KeyFn = ...) -> Callable[[_F], _F]:
+            key_fn: _KeyFn = ...,
+            bytesize: bool = ...) -> Callable[[_F], _F]:
     ...
 
 
 @overload
 def memoize(capacity: int,
             *,
             batched: Literal[True],
             policy: _Policy = ...,
-            key_fn: _KeyFn = ...) -> Callable[[_BatchedFn], _BatchedFn]:
+            key_fn: _KeyFn = ...,
+            bytesize: bool = ...) -> Callable[[_BatchedFn], _BatchedFn]:
     ...
```

### Comparing `glow-0.12.7/src/glow/core/wrap/concurrency.py` & `glow-0.12.8/src/glow/core/wrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/wrap/concurrency.pyi` & `glow-0.12.8/src/glow/core/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/wrap/reusable.py` & `glow-0.12.8/src/glow/core/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/core/wrap/util.py` & `glow-0.12.8/src/glow/core/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/io/_sound.py` & `glow-0.12.8/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/io/_svg.py` & `glow-0.12.8/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/metrics/__init__.py` & `glow-0.12.8/src/glow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/metrics/base.py` & `glow-0.12.8/src/glow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/metrics/confusion.py` & `glow-0.12.8/src/glow/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/metrics/raw.py` & `glow-0.12.8/src/glow/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/__init__.py` & `glow-0.12.8/src/glow/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/_loader.py` & `glow-0.12.8/src/glow/nn/_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/_sampler.py` & `glow-0.12.8/src/glow/nn/_sampler.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/_trainer.py` & `glow-0.12.8/src/glow/nn/_trainer.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/amp.py` & `glow-0.12.8/src/glow/nn/amp.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/driver.py` & `glow-0.12.8/src/glow/nn/driver.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/functional.py` & `glow-0.12.8/src/glow/nn/functional.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/optimizers.py` & `glow-0.12.8/src/glow/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/plot.py` & `glow-0.12.8/src/glow/nn/plot.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/proto.py` & `glow-0.12.8/src/glow/nn/proto.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/util.py` & `glow-0.12.8/src/glow/nn/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/__init__.py` & `glow-0.12.8/src/glow/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/aggregates.py` & `glow-0.12.8/src/glow/nn/modules/aggregates.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/context.py` & `glow-0.12.8/src/glow/nn/modules/context.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/convnets.py` & `glow-0.12.8/src/glow/nn/modules/convnets.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/lazy.py` & `glow-0.12.8/src/glow/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/simple.py` & `glow-0.12.8/src/glow/nn/modules/simple.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/transformers.py` & `glow-0.12.8/src/glow/nn/modules/transformers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/util.py` & `glow-0.12.8/src/glow/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/nn/modules/vision.py` & `glow-0.12.8/src/glow/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/transforms/__init__.py` & `glow-0.12.8/src/glow/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/transforms/classes.py` & `glow-0.12.8/src/glow/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/transforms/core.py` & `glow-0.12.8/src/glow/transforms/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/transforms/functional/core.py` & `glow-0.12.8/src/glow/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/src/glow/transforms/functional/numba.py` & `glow-0.12.8/src/glow/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/run_metrics.py` & `glow-0.12.8/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_api.py` & `glow-0.12.8/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_batch.py` & `glow-0.12.8/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_buffered.py` & `glow-0.12.8/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_cli.py` & `glow-0.12.8/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_iter.py` & `glow-0.12.8/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_loader.py` & `glow-0.12.8/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_shm.py` & `glow-0.12.8/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_thread_pool.py` & `glow-0.12.8/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_timed.py` & `glow-0.12.8/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/test/test_uuid.py` & `glow-0.12.8/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/LICENSE` & `glow-0.12.8/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/README.md` & `glow-0.12.8/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.12.7/pyproject.toml` & `glow-0.12.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.12.7"
+version = "0.12.8"
 description = "Functional Python tools with a PyTorch flavour"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "loky>=3.1",
     "lxml",
     "numpy~=1.21",
     "tqdm",
-    "wrapt",
+    "wrapt~=1.15",
 ]
 
 [project.urls]
 homepage = "https://github.com/arquolo/glow"
 
 [project.optional-dependencies]
 memprof = ["psutil"]
```

### Comparing `glow-0.12.7/PKG-INFO` & `glow-0.12.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glow
-Version: 0.12.7
+Version: 0.12.8
 Summary: Functional Python tools with a PyTorch flavour
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
@@ -34,15 +34,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Requires-Dist: loky>=3.1
 Requires-Dist: lxml
 Requires-Dist: numpy~=1.21
 Requires-Dist: tqdm
-Requires-Dist: wrapt
+Requires-Dist: wrapt~=1.15
 Provides-Extra: all
 Requires-Dist: glow[cv,io,nn]; extra == 'all'
 Requires-Dist: matplotlib; extra == 'all'
 Provides-Extra: cv
 Requires-Dist: opencv-python~=4.0; extra == 'cv'
 Requires-Dist: scipy; extra == 'cv'
 Provides-Extra: cv-dither
```

