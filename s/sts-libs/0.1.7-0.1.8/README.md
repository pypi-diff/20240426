# Comparing `tmp/sts_libs-0.1.7.tar.gz` & `tmp/sts_libs-0.1.8.tar.gz`

## Comparing `sts_libs-0.1.7.tar` & `sts_libs-0.1.8.tar`

### file list

```diff
@@ -1,98 +1,105 @@
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.gitlab-ci.yml
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sts_libs-0.1.7/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.1.7/noxfile.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.fmf/version
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 sts_libs-0.1.7/docs/contributing.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/main.fmf
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/be2iscsi.fmf
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/bnx2i.fmf
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/cxgb4i.fmf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/local.fmf
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/qedi.fmf
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/tier0.fmf
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/iscsi/libiscsi/main.fmf
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/main.fmf
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/regression.fmf
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sts_libs-0.1.7/plans/rdma/test_case_vars.yaml
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 sts_libs-0.1.7/scripts/install-python.sh
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    52285 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    38610 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    73771 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    41777 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/rdma.py
--rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17006 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    22417 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/iscsi_fixtures.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/fixtures/rdma_fixtures.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/log.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/conftest.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/pytest.ini
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/main.fmf
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/be2iscsi.yaml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/bnx2i.yaml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/cxgb4i.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/qedi.yaml
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/_vars/template_iscsi_host.yaml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/main.fmf
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/local/libiscsi-local.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/libiscsi/local/main.fmf
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/login-logout-stress/login-logout-stress.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/login-logout-stress/main.fmf
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/many-luns/main.fmf
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/many-luns/many-luns-local.py
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/parameters/iscsi_params.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/iscsi/parameters/main.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/main.fmf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/main.fmf
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/main.fmf
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/customer_1/issue_23967_verify_speed.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/customers/customer_1/main.fmf
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/others/main.fmf
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/bugs/others/reproducers.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/pyverbs-tests/core/main.fmf
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/pyverbs-tests/core/pyverbs-tests.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/sriov/core/main.fmf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 sts_libs-0.1.7/tests/rdma/sriov/core/sriov.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.1.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.1.7/LICENSE
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 sts_libs-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.1.7/sts_libs/README.md
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 sts_libs-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 sts_libs-0.1.8/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 sts_libs-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 sts_libs-0.1.8/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sts_libs-0.1.8/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sts_libs-0.1.8/.fmf/version
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 sts_libs-0.1.8/docs/contributing.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/main.fmf
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/be2iscsi.fmf
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/bnx2i.fmf
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/cxgb4i.fmf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/local.fmf
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/qedi.fmf
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/tier0.fmf
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/rdma/main.fmf
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/rdma/regression.fmf
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sts_libs-0.1.8/plans/rdma/test_case_vars.yaml
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 sts_libs-0.1.8/scripts/install-python.sh
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/blockdevice.py
+-rw-r--r--   0        0        0    20697 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    41636 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    52263 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    73709 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    35864 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    35890 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    41772 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    17929 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/nvme.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/rdma.py
+-rw-r--r--   0        0        0    28172 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    22383 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fixtures/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fixtures/common_fixtures.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fixtures/iscsi_fixtures.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fixtures/rdma_fixtures.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/fixtures/stratis_fixtures.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/log.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/pytest.ini
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/main.fmf
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/_vars/be2iscsi.yaml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/_vars/bnx2i.yaml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/_vars/cxgb4i.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/_vars/qedi.yaml
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/_vars/template_iscsi_host.yaml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/libiscsi/main.fmf
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/libiscsi/local/libiscsi-local.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/libiscsi/local/main.fmf
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/login-logout-stress/login-logout-stress.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/login-logout-stress/main.fmf
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/many-luns/main.fmf
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/many-luns/many-luns-local.py
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/parameters/iscsi_params.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/iscsi/parameters/main.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/main.fmf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/main.fmf
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/customers/main.fmf
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/customers/customer_1/issue_23967_verify_speed.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/customers/customer_1/main.fmf
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/others/main.fmf
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/bugs/others/reproducers.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/pyverbs-tests/core/main.fmf
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/pyverbs-tests/core/pyverbs-tests.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/sriov/core/main.fmf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/rdma/sriov/core/sriov.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/stratis/main.fmf
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/stratis/pool_create_destroy/main.fmf
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 sts_libs-0.1.8/tests/stratis/pool_create_destroy/test_pool.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sts_libs-0.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 sts_libs-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sts_libs-0.1.8/sts_libs/README.md
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 sts_libs-0.1.8/PKG-INFO
```

### Comparing `sts_libs-0.1.7/.pre-commit-config.yaml` & `sts_libs-0.1.8/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 repos:
-  - repo: https://github.com/psf/black
-    rev: 24.2.0
-    hooks:
-      - id: black
-
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.4.1
     hooks:
       - id: ruff
-        args: [--fix, --preview]
+        args: [--fix]
+      - id: ruff-format
 
   - repo: https://github.com/lyz-code/yamlfix/
     rev: 1.16.0
     hooks:
       - id: yamlfix
         types:
           - text
         files: '\.(fmf|yaml)$'
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-case-conflict
       - id: check-ast
       - id: check-docstring-first
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-builtin-literals
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
+      - id: pretty-format-json
         args: [--markdown-linebreak-ext=md]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
       - id: mypy
 
   - repo: https://github.com/teemtee/tmt.git
-    rev: 1.31.0
+    rev: 1.32.2
     hooks:
       - id: tmt-lint
```

### Comparing `sts_libs-0.1.7/README.md` & `sts_libs-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # :construction: Work in progress :construction:
 
 # sts - Storage Tests
 
-The goal of this project is to be able to easily and rapidly write tests for kernel storage drivers and related user-space tools in Fedora, CentOS Stream and Red Hat Enterprise Linux.  
+The goal of this project is to be able to easily and rapidly write tests for kernel storage drivers and related user-space tools in Fedora, CentOS Stream and Red Hat Enterprise Linux.
 
 It is designed to work with pytest and [tmt](https://tmt.readthedocs.io/en/stable/). It consists of two main parts:
 1) Python [sts-libs](sts_libs/README.md)
 2) Tests, Plans with tmt metadata
 
 For contribution guide, please see [docs](docs/contributing.md)
```

### Comparing `sts_libs-0.1.7/noxfile.py` & `sts_libs-0.1.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/docs/contributing.md` & `sts_libs-0.1.8/docs/contributing.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # Contributing to sts
 
 ## Python code contributions
 ### Local environment
 - Fork the [project](https://gitlab.com/rh-kernel-stqe/sts/)
-- Create a python virtualenv by running `hatch env create`
+- Clone your fork and enter the directory
+- Create and enter python virtualenv
+  - `hatch shell`
 - Enable pre-commit hooks
-  - `python3 -m pip install pipx`
-  - `python3 -m pipx install pre-commit`
   - `pre-commit install`
-- Feel free to use hatch commands to ensure passing pre-commit and CI checks
+- If you're using an IDE
+  - set max line length to `120` and Python compatibility checks to 3.9+.
+  - consider installing ruff plugin
+- To check your changes without commiting
+  - pre-commit run --all-files
+- To list available hatch env scripts, run `hatch env show`
   - `hatch run container-prep` will use buildah to prepare a Fedora container
   - `hatch run tests` will run the tests within the container
-  - `hatch run format` will run black formatter and ruff linter with autofix enabled
-  - `hatch run lint` will run black and ruff without autofix
+  - `hatch run format` will run ruff formatter and linter with autofix enabled
+  - `hatch run lint` will run ruff without autofix
   - `hatch run check` will run mypy type annotation checks
   - `hatch run all` will run format, check and tests
-- Set max line length to `120` and Python compatibility checks to 3.8+.
-  - consider also adding ruff plugin to your IDE
 
 ### Typing and Docstrings
 All new functions, methods, classes in sts-libs should include
-[type annotations](https://docs.python.org/3/library/typing.html), so they pass `mypy --strict` check.  
+[type annotations](https://docs.python.org/3/library/typing.html), so they pass `mypy --strict` check.
 
 There should always be a single-line docstring and optionally:
 
   - Argument documentation.
 
     - when the usage of the argument is not clear even with proper type annotation
     - not all arguments needs to be documented
@@ -60,20 +63,20 @@
     """
 ```
 
 The pre-commit check does not include `--strict` mypy argument, mainly due to the existing untyped legacy code (contributions very welcome),
 but also to allow more freedom when writing sts tests. You might be however asked to add type annotations when creating a merge request to sts-libs.
 
 ### Commits
-First line up to 50 characters.  
-Additional details should be separated by a blank line.  
+First line up to 50 characters.
+Additional details should be separated by a blank line.
 
 Consider following [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) rules.
 
 It is encouraged to do multiple smaller commits instead of one large one.
 
-The pre-commit hooks include some auto-fixes, like `black` formatter, or 'fixable' ruff rules.  
+The pre-commit hooks include some auto-fixes by ruff linter and formatter.
 Please check any changed files before trying to commit again.
 
 ### Creating a merge request
 Follow the [gitlab documentation](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html#when-you-work-in-a-fork)
 for how to create a merge request.
```

### Comparing `sts_libs-0.1.7/plans/rdma/regression.fmf` & `sts_libs-0.1.8/plans/rdma/regression.fmf`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/dm.py` & `sts_libs-0.1.8/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/dmpd.py` & `sts_libs-0.1.8/sts_libs/src/sts/dmpd.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/fc.py` & `sts_libs-0.1.8/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/fio.py` & `sts_libs-0.1.8/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/iscsi.py` & `sts_libs-0.1.8/sts_libs/src/sts/iscsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,20 +119,20 @@
     def _run(
         self,
         mode: str = '',
         arguments: dict[str, str] | dict[str, str | None] | None = None,
     ) -> CommandResult:
         if mode is not None:
             self.validate_mode(mode)
-        if arguments is not None and self.disable_check is not True:
+        if arguments is not None and not self.disable_check:
             self.validate_arguments(mode, arguments)
 
         command_list: list[str] = [CLI_NAME, '--mode', mode]
         if arguments is not None:
-            command_list = command_list + [k if v is None else f'{k} {v}' for k, v in arguments.items()]
+            command_list += [k if v is None else f'{k} {v}' for k, v in arguments.items()]
         if self.debug_level:
             command_list = [*command_list, '--debug', str(self.debug_level)]
         command: str = ' '.join(command_list)
         return run(command)
 
     def iface(
         self,
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/linux.py` & `sts_libs-0.1.8/sts_libs/src/sts/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     Name of the service
     Returns:
     True: Service got enabled
     False: There was some problem.
     """
     cmd = f'systemctl enable {service_name}'
     if now:
-        cmd = cmd + ' --now'
+        cmd += ' --now'
 
     if run(cmd).rc != 0:
         logging.error(f'Could not enable {service_name}')
         run(f'systemctl status {service_name}')
         run('journalctl -xn')
         return False
     return True
@@ -1233,15 +1233,15 @@
     mount_flag = False
     if is_mounted('/var/crash'):
         logging.info('Unmounting /var/crash to avoid sosreport being hang there')
         umount('/var/crash')
         mount_flag = True
 
     if skip_plugins:
-        cmd = cmd + f' --skip-plugins {skip_plugins}'
+        cmd += f' --skip-plugins {skip_plugins}'
 
     ret_code, sosreport_ret = run_ret_out(cmd, return_output=True)
     if ret_code != 0:
         logging.error('sosreport command failed')
         if mount_flag:
             mount('/var/crash')
         return False
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/lio.py` & `sts_libs-0.1.8/sts_libs/src/sts/lio.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,15 +729,15 @@
         # Set default backend file name
         file_name = f'{lun_name}.img'
 
     # disable spare, to force targetcli to allocate the whole file to avoid problem
     # of running out of disk space and not have enough space to store data
     cmd = f'targetcli /backstores/fileio create {lun_name} {file_name} sparse=false'
     if lun_size:
-        cmd = cmd + f' {lun_size}'
+        cmd += f' {lun_size}'
 
     if run(cmd).rc != 0:
         logging.error(f'Could not create fileio {lun_name}')
         return False
     return True
 
 
@@ -768,15 +768,15 @@
     return None
 
 
 # ## PSCSI ###
 def _lio_create_backstore_pscsi(lun_name, device, lun_size=None):  # noqa: ANN001, ANN202
     cmd = f'targetcli /backstores/pscsi create {lun_name} {device}'
     if lun_size:
-        cmd = cmd + f' {lun_size}M'
+        cmd += f' {lun_size}M'
 
     if run(cmd).rc != 0:
         logging.error(f'Could not create pscsi {lun_name}')
         return False
     return True
 
 
@@ -1425,18 +1425,17 @@
     tgt_wwn:      Host WWN
     bs_type:      Backstore type
     lun_name:     Lun Name
     Returns:
     True: If LUN is created
     False: If some problem happened.
     """
-    cmd = 'targetcli /tcm_fc/{}/luns create /backstores/{}/{} add_mapped_luns=false'.format(
-        _wwn_2_tgt_wwn(tgt_wwn),
-        bs_type,
-        lun_name,
+    cmd = (
+        f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/luns create '
+        f'/backstores/{bs_type}/{lun_name} add_mapped_luns=false'
     )
 
     if run(cmd).rc != 0:
         logging.error(f'Could not add lun to FC target {tgt_wwn}')
         return False
 
     return True
@@ -1570,19 +1569,16 @@
     print('BRUNO lio_create_fc_target_map_lun')
     # print lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id)
 
     if lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id, lio_dict=lio_dict):
         logging.info(f'lun {tgt_lun_id} is already mapped to FC target {tgt_wwn}/{init_wwn}')
         return True
 
-    cmd = 'targetcli /tcm_fc/{}/acls/{} create {} {}'.format(
-        _wwn_2_tgt_wwn(tgt_wwn),
-        _wwn_2_tgt_wwn(init_wwn),
-        init_lun_id,
-        tgt_lun_id,
+    cmd = (
+        f'targetcli /tcm_fc/{_wwn_2_tgt_wwn(tgt_wwn)}/acls/{_wwn_2_tgt_wwn(init_wwn)} create {init_lun_id} {tgt_lun_id}'
     )
 
     if run(cmd).rc != 0:
         logging.error(f'Could not map lun to FC target {tgt_wwn}/{init_wwn}')
         return False
 
     if not lio_get_fc_target_map_lun(tgt_wwn, init_wwn, tgt_lun_id):
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/loopdev.py` & `sts_libs-0.1.8/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/lsm.py` & `sts_libs-0.1.8/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/lvm.py` & `sts_libs-0.1.8/sts_libs/src/sts/lvm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/md.py` & `sts_libs-0.1.8/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/mp.py` & `sts_libs-0.1.8/sts_libs/src/sts/mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     return linux.is_service_running(mp_service_name())
 
 
 def mpathconf_enable(find_mpaths: Literal['yes', 'no', 'strict', 'greedy', 'smart', None] = None) -> bool:
     """Runs 'mpathconf --enable' command."""
     cmd = 'mpathconf --enable'
     if find_mpaths:
-        cmd = cmd + f' --find_multipaths {find_mpaths}'
+        cmd += f' --find_multipaths {find_mpaths}'
     if run(cmd).rc != 0:
         return False
 
     return True
 
 
 def mp_enable() -> bool:
@@ -96,15 +96,15 @@
     cmd = 'pidof multipathd'
     retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         logging.error('For some reason multipathd is not running')
         print(output)
         return None
     fmt = '"%d %m"'
-    cmd = f"multipathd show paths format {fmt} | egrep \"^{disk}\" | awk '{{print$2}}'"
+    cmd = f'multipathd show paths format {fmt} | egrep "^{disk}" | awk \'{{print$2}}\''
     retcode, output = run_ret_out(cmd, return_output=True)
     if retcode != 0:
         logging.error(f'to find multipath of disk {disk}')
         print(output)
         return None
     mpath = output
 
@@ -233,19 +233,19 @@
     regex_mpath += r'([^ ]+?)\ +'  # 1. mpath_name
     regex_mpath += r'(?:\((\S+)\)\ +){0,1}'  # 2. wwid if different from #1
     regex_mpath += r'(?:(dm\-[0-9]+)\ +){0,1}'  # 3. dm_name if known
     regex_mpath += r'(?:([^,]+),){0,1}'  # 4. vendor, might not have
     regex_mpath += r'(?:([^,]+)){0,1}$'  # 5. product,  might not have
 
     regex_feature = r'size=([0-9\.]+[A-Z])\ +'  # 1. size
-    regex_feature += r"features=\'([^\']+)\'\ +"  # 2. features
-    regex_feature += r"hwhandler=\'([^\']+)\'\ +"  # 3. hardware handler
+    regex_feature += r'features=\'([^\']+)\'\ +'  # 2. features
+    regex_feature += r'hwhandler=\'([^\']+)\'\ +'  # 3. hardware handler
     regex_feature += r'(?:wp=([rw]+)){0,1}'  # 4. write permission if known
 
-    regex_pg = r"[^a-z]+policy=\'([^\`]+)\'\ +"  # 1. policy of this PG path_selector
+    regex_pg = r'[^a-z]+policy=\'([^\`]+)\'\ +'  # 1. policy of this PG path_selector
     regex_pg += r'(?:prio=([0-9\-]+)\ +){0,1}'  # 2. priority of this PG if known
     regex_pg += r'(?:status=([a-z]+)){0,1}'  # 3. status of this PG if known (active or enable, etc)
 
     regex_disk = r'[^0-9]+'
     regex_disk += r'([0-9]+:[0-9]+:[0-9]+:[0-9]+)\ +'  # 1. scsi_id
     regex_disk += r'([a-z]+)\ +'  # 2. dev_name
     regex_disk += r'([0-9]+:[0-9]+)\ +'  # 3. major:minor
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/net.py` & `sts_libs-0.1.8/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.1.8/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/rdma.py` & `sts_libs-0.1.8/sts_libs/src/sts/rdma.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/scsi.py` & `sts_libs-0.1.8/sts_libs/src/sts/scsi.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.1.8/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/vdo.py` & `sts_libs-0.1.8/sts_libs/src/sts/vdo.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,15 @@
         logging.warning(f'Device {device_name} not found using lsblk. Using default 2G size.')
         return '2G'
     size = device_size.split()[3]
     multipliers = ['M', 'G', 'T', 'P', 'E']
     device_size = int(float(size[:-1]) * (1024 ** multipliers.index(size[-1:])))
     max_number_of_slabs = 8192
     minimum_size = 2 ** int(device_size / max_number_of_slabs).bit_length()
-    if minimum_size < 128:
-        minimum_size = 128
+    minimum_size = max(minimum_size, 128)
     if default_to_2g and minimum_size < 2048:
         return '2G'
     return str(minimum_size) + 'M'
 
 
 def maximum_logical_size():  # noqa: ANN201
     """Returns maximum logical size based on memory.
@@ -67,16 +66,15 @@
       string max_size.
     """
     good_size = 4096
     memory = linux.get_memory()['mem']['free']
     size = f'{good_size}T'
     if memory < 10000:
         size = 2 ** (int((4096.0 / 10000) * float(memory)).bit_length() - 1)
-        if size > good_size:
-            size = good_size
+        size = min(size, good_size)
     return size
 
 
 def is_block_device(device):  # noqa: ANN001, ANN201
     try:
         mode = Path(device).stat().st_mode
     except OSError:
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/fixtures/rdma_fixtures.py` & `sts_libs-0.1.8/sts_libs/src/sts/fixtures/rdma_fixtures.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/cmdline.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,7 +62,11 @@
         return completed_command.rc, output.rstrip()  # type: ignore [return-value]
 
     return completed_command.rc
 
 
 def exists(cmd: str) -> bool:
     return host.exists(cmd)
+
+
+def check_output(cmd: str) -> str:
+    return host.check_output(cmd)
```

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/logchecker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/size.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.1.8/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/cmdline_test.py` & `sts_libs-0.1.8/sts_libs/tests/cmdline_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,20 @@
         ret_out = run(test_cmd)
         assert ret_out.rc == 0
         assert ret_out.stdout == f'{test_msg}\n'
 
     def test_run_return_output_legacy(self) -> None:
         test_msg = 'run test message'
         test_cmd = f'echo {test_msg}'
-        assert run_ret_out(test_cmd, return_output=True) == (0, f'{test_msg}')
+        assert run_ret_out(test_cmd, return_output=True) == (0, test_msg)
 
     def test_run_fail_return_output(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
         test_cmd = 'ls invalid_file'
         ret_out = run(test_cmd)
         assert ret_out.rc == 2
         assert ret_out.stderr == f'{failure_msg}\n'
 
     def test_run_fail_return_output_legacy(self) -> None:
         failure_msg = "ls: cannot access 'invalid_file': No such file or directory"
         test_cmd = 'ls invalid_file'
-        assert run_ret_out(test_cmd, return_output=True) == (2, f'{failure_msg}')
+        assert run_ret_out(test_cmd, return_output=True) == (2, failure_msg)
```

### Comparing `sts_libs-0.1.7/sts_libs/tests/fio_test.py` & `sts_libs-0.1.8/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/iscsi_test.py` & `sts_libs-0.1.8/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/linux_test.py` & `sts_libs-0.1.8/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/logchecker_test.py` & `sts_libs-0.1.8/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/lvm_test.py` & `sts_libs-0.1.8/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/md_test.py` & `sts_libs-0.1.8/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/net_test.py` & `sts_libs-0.1.8/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.1.8/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/sts_libs/tests/scsi_test.py` & `sts_libs-0.1.8/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/iscsi/_vars/template_iscsi_host.yaml` & `sts_libs-0.1.8/tests/iscsi/_vars/template_iscsi_host.yaml`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/iscsi/libiscsi/local/libiscsi-local.py` & `sts_libs-0.1.8/tests/iscsi/libiscsi/local/libiscsi-local.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/iscsi/login-logout-stress/login-logout-stress.py` & `sts_libs-0.1.8/tests/iscsi/login-logout-stress/login-logout-stress.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/iscsi/many-luns/many-luns-local.py` & `sts_libs-0.1.8/tests/iscsi/many-luns/many-luns-local.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     assert lio.Iscsi(target_wwn=t_iqn).create_target().succeeded
     assert lio.ACL(target_wwn=t_iqn, initiator_wwn=i_iqn).create_acl().succeeded
 
     for n in range(n_luns):
         backstore = lio.BackstoreFileio(name=f'backstore{n}')
         assert backstore.create_backstore(size=back_size, file_or_dev=f'backstore_file{n}').succeeded
-        assert lio.LUNs(target_wwn=t_iqn).create_lun(storage_object=f'{backstore.path}').succeeded
+        assert lio.LUNs(target_wwn=t_iqn).create_lun(storage_object=backstore.path).succeeded
 
     iscsi.set_initiatorname(i_iqn)
     iscsi.discovery_st('127.0.0.1', disc_db=True, ifaces='default')
     iscsiadm = iscsi.IscsiAdm()
     for _ in range(3):
         assert iscsiadm.node_login()
         wait_udev(sleeptime=1)
```

### Comparing `sts_libs-0.1.7/tests/iscsi/parameters/iscsi_params.py` & `sts_libs-0.1.8/tests/iscsi/parameters/iscsi_params.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/iscsi/parameters/main.fmf` & `sts_libs-0.1.8/tests/iscsi/parameters/main.fmf`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/rdma/bugs/others/reproducers.py` & `sts_libs-0.1.8/tests/rdma/bugs/others/reproducers.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/rdma/pyverbs-tests/core/pyverbs-tests.py` & `sts_libs-0.1.8/tests/rdma/pyverbs-tests/core/pyverbs-tests.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/tests/rdma/sriov/core/sriov.py` & `sts_libs-0.1.8/tests/rdma/sriov/core/sriov.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/.gitignore` & `sts_libs-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/LICENSE` & `sts_libs-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/pyproject.toml` & `sts_libs-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 [project]
 name = 'sts-libs'
 description = 'Library for pytest-based Linux storage tests'
 readme = 'sts_libs/README.md'
 requires-python = '>=3.9'
 dynamic = ['version']
 authors = [
-  {name = 'Bruno Goncalves', email = 'bgoncalv@redhat.com'},
-  {name = 'Filip Suba', email = 'fsuba@redhat.com'},
-  {name = 'Jakub Krysl', email = 'jkrysl@redhat.com'},
   {name = 'Martin Hoyer', email = 'mhoyer@redhat.com'},
+  {name = 'Filip Suba', email = 'fsuba@redhat.com'},
   {name = 'Zhaojuan Guo', email = 'zguo@redhat.com'},
+  {name = 'Bruno Goncalves', email = 'bgoncalv@redhat.com'},
+  {name = 'Jakub Krysl', email = 'jkrysl@redhat.com'},
 ]
 maintainers = [
   {name = 'Martin Hoyer', email = 'mhoyer@redhat.com'},
   {name = 'Filip Suba', email = 'fsuba@redhat.com'},
+  {name = 'Zhaojuan Guo', email = 'zguo@redhat.com'},
 ]
 license = 'GPL-3.0-or-later'
 license-files = {paths = ['LICENSE']}
 classifiers = [
   'Programming Language :: Python :: 3 :: Only',
   'Programming Language :: Python :: 3.9',
   'Topic :: Software Development :: Testing',
@@ -44,65 +45,55 @@
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.targets.wheel]
 packages = ['sts_libs/src/sts']
 
-[dirs.env]
-virtual = ".venv"
-
 [tool.hatch.envs.default]
 dependencies = [
-  "black",
   "ruff",
   "mypy",
+  "pre-commit",
 ]
 
 [tool.hatch.envs.default.scripts]
+# TODO use pytest-container
 container-prep = 'buildah from --name fedora-sts fedora && buildah run fedora-sts dnf install -y python3-pip'
 tests = 'buildah copy fedora-sts ../sts sts && buildah run fedora-sts pip install sts/ && buildah run fedora-sts pytest sts/sts_libs/tests/'
-format = ['ruff --fix {args:.}', 'black {args:.}']
-lint = ['ruff {args:.}', 'black --check {args:.}']
-check = ['mypy {args:.}']
+format = ['ruff check --fix', 'ruff format']
+lint = ['ruff check', 'ruff format --check']
+check = 'mypy {args:.}'
 all = ['format', 'lint', 'check', 'tests']
 
-[tool.black]
-line-length = 120
-target-version = ['py39', 'py312']
-skip-string-normalization = 'True'  # Preferring single quotes
-
 [tool.ruff]
 line-length = 120
 namespace-packages = ['sts_libs']
 src = ['sts_libs/src']
 
-[tool.ruff.lint]
-select = [
+lint.select = [
   'F',  # Pyflakes
-  'E',  # pycodestyle
-  'W',  # pycodestyle
+  'E',  # pycodestyle error
+  'W',  # pycodestyle warning
   'I',  # isort
   'N',  # pep8-naming
   'D',  # pydocstyle
   'UP',  # pyupgrade
   'YTT',  # flake8-2020
   'ANN',  # flake8-annotations
   'ASYNC', # flake8-async
   'BLE',  # flake8-blind-except
   #'FBT',  # flake8-boolean-trap
   'B',  # flake8-bugbear
   'A',  # flake8-builtins
-  'COM',  # flake8-commas
   'C4',  # flake8-comprehensions
   'DTZ',  # flake8-datetimez
   'T10',  # flake8-debugger
   'EM',  # flake8-errmsg
   'FA',  # flake8-future-annotations
-  'ISC',  # flake8-implicit-str-concat
   'ICN',  # flake8-import-conventions
   'G',  # flake8-logging-format
   'INP',  # flake8-no-pep420
   'PIE',  # flake8-pie
   #'T20',  # flake8-print -> TODO
   'PT',  # flake8-pytest-style
   'Q',  # flake8-quotes
@@ -121,25 +112,28 @@
   'TRY',  # tryceratops
   'FLY',  # flynt
   'PERF',  # perflint
   'FURB',  # refurb
   'LOG',  # flake8-logging
   'RUF',  # Ruff-specific rules
 ]
-ignore = [
+lint.ignore = [
   'D10',  # Missing docstring -> TODO
   'D205',  # 1 blank line required between summary line and description -> TODO
   'D417',  # Missing argument descriptions -> Do not use docstring description for well type-annotated args
   'PLR09',  # pylint-refactor too-many -> TODO
   'PLR1702',  # Too many nested blocks
   'PLR2004',  # magic value -> TODO
   'ANN101',  # Missing type annotation for `self` in method -> Not necessary
+  'ANN102',  # Missing type annotation for `cls` in method -> Not necessary
   'G004',  # Logging statement uses f-string -> Up for discussion
 ]
 
+format.quote-style = "single"
+
 [tool.ruff.lint.per-file-ignores]
 'tests/*' = ['INP001']
 'sts_libs/src/sts/lvm.py' = ['PLR6301']
 'sts_libs/tests/*' = ['PLR6301']
 
 [tool.ruff.lint.flake8-builtins]
 builtins-ignorelist = ['id']
```

### Comparing `sts_libs-0.1.7/sts_libs/README.md` & `sts_libs-0.1.8/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.1.7/PKG-INFO` & `sts_libs-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: sts-libs
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library for pytest-based Linux storage tests
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
-Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>, Zhaojuan Guo <zguo@redhat.com>
-Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>
+Author-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Zhaojuan Guo <zguo@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>, Jakub Krysl <jkrysl@redhat.com>
+Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Zhaojuan Guo <zguo@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
```

