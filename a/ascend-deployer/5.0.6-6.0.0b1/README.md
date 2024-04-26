# Comparing `tmp/ascend_deployer-5.0.6-py3-none-any.whl.zip` & `tmp/ascend_deployer-6.0.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,500 +1,421 @@
-Zip file size: 638575 bytes, number of entries: 498
--rw-rw-rw-  2.0 fat      769 b- defN 24-Mar-25 02:31 ascend_deployer/__init__.py
--rw-rw-rw-  2.0 fat      444 b- defN 24-Mar-25 02:31 ascend_deployer/ansible.cfg
--rw-rw-rw-  2.0 fat     7854 b- defN 24-Mar-25 02:31 ascend_deployer/ascend_deployer.py
--rw-rw-rw-  2.0 fat     2174 b- defN 24-Mar-25 02:31 ascend_deployer/ascend_download.py
--rw-rw-rw-  2.0 fat     6179 b- defN 24-Mar-25 02:31 ascend_deployer/downloader_ui.py
--rw-rw-rw-  2.0 fat      835 b- defN 24-Mar-25 07:43 ascend_deployer/install.sh
--rw-rw-rw-  2.0 fat      493 b- defN 24-Mar-25 02:31 ascend_deployer/inventory_file
--rw-rw-rw-  2.0 fat     7090 b- defN 24-Mar-25 02:31 ascend_deployer/jobs.py
--rw-rw-rw-  2.0 fat      475 b- defN 24-Mar-25 07:43 ascend_deployer/start_download.sh
--rw-rw-rw-  2.0 fat       69 b- defN 24-Mar-25 02:31 ascend_deployer/start_download_ui.bat
--rw-rw-rw-  2.0 fat     7852 b- defN 24-Mar-25 02:31 ascend_deployer/utils.py
--rw-rw-rw-  2.0 fat       54 b- defN 24-Mar-25 02:31 ascend_deployer/version.json
--rw-rw-rw-  2.0 fat    14692 b- defN 24-Mar-25 02:31 ascend_deployer/ansible_plugin/ansible_log.py
--rw-rw-rw-  2.0 fat     1123 b- defN 24-Mar-25 02:31 ascend_deployer/ansible_plugin/install_info.yaml
--rw-rw-rw-  2.0 fat      706 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/__init__.py
--rw-rw-rw-  2.0 fat      176 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config.ini
--rw-rw-rw-  2.0 fat    11086 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/deb_downloader.py
--rw-rw-rw-  2.0 fat     3855 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dl_mef_dependency_downloader.py
--rw-rw-rw-  2.0 fat     2197 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/download_data.py
--rw-rw-rw-  2.0 fat    16684 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/download_util.py
--rw-rw-rw-  2.0 fat    11892 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/downloader.py
--rw-rw-rw-  2.0 fat     4554 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/logger_config.py
--rw-rw-rw-  2.0 fat     2839 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/obs_downloader.py
--rw-rw-rw-  2.0 fat     1630 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/obs_resources.json
--rw-rw-rw-  2.0 fat     4685 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/os_dep_downloader.py
--rw-rw-rw-  2.0 fat     7197 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/other_downloader.py
--rw-rw-rw-  2.0 fat     3450 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/other_resources.json
--rw-rw-rw-  2.0 fat    14538 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/parallel_file_downloader.py
--rw-rw-rw-  2.0 fat    12446 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/pip_downloader.py
--rw-rw-rw-  2.0 fat     8754 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/python_version.json
--rw-rw-rw-  2.0 fat     1738 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/requirements.txt
--rw-rw-rw-  2.0 fat    20222 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/rpm_downloader.py
--rw-rw-rw-  2.0 fat    13421 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software_mgr.py
--rw-rw-rw-  2.0 fat      935 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/version_match.json
--rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      157 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/source.repo
--rw-rw-rw-  2.0 fat    65719 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3082 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      262 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/source.repo
--rw-rw-rw-  2.0 fat    66091 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     2844 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      251 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/source.repo
--rw-rw-rw-  2.0 fat    12476 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      234 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
--rw-rw-rw-  2.0 fat    13906 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      371 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
--rw-rw-rw-  2.0 fat    43257 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     5919 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      131 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
--rw-rw-rw-  2.0 fat    42707 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     5143 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat       65 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
--rw-rw-rw-  2.0 fat    65900 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     9517 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      130 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
--rw-rw-rw-  2.0 fat    42840 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     8566 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      130 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
--rw-rw-rw-  2.0 fat    42208 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     8108 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat       65 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
--rw-rw-rw-  2.0 fat    55524 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3888 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      263 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/source.repo
--rw-rw-rw-  2.0 fat    60396 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3388 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      264 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
--rw-rw-rw-  2.0 fat    60964 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     3201 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      253 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
--rw-rw-rw-  2.0 fat    60396 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3388 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Kylin_V10_aarch64/source.repo
--rw-rw-rw-  2.0 fat    51454 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3369 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      365 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
--rw-rw-rw-  2.0 fat    51932 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     3651 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      353 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
--rw-rw-rw-  2.0 fat    51351 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     5439 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      458 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
--rw-rw-rw-  2.0 fat    43010 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
--rw-rw-rw-  2.0 fat     3220 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      445 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
--rw-rw-rw-  2.0 fat    56970 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
--rw-rw-rw-  2.0 fat     3134 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      268 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
--rw-rw-rw-  2.0 fat     4234 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      370 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
--rw-rw-rw-  2.0 fat     5748 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      352 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
--rw-rw-rw-  2.0 fat     5202 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      366 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
--rw-rw-rw-  2.0 fat     6286 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      348 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
--rw-rw-rw-  2.0 fat     5921 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
--rw-rw-rw-  2.0 fat      366 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
--rw-rw-rw-  2.0 fat     6674 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
--rw-rw-rw-  2.0 fat      348 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3922 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3930 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
--rw-rw-rw-  2.0 fat     3914 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
--rw-rw-rw-  2.0 fat     4010 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3994 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     4010 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3994 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3715 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
--rw-rw-rw-  2.0 fat     3681 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
--rw-rw-rw-  2.0 fat     1185 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
--rw-rw-rw-  2.0 fat     1177 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
--rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3106 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3922 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3930 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
--rw-rw-rw-  2.0 fat     3914 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
--rw-rw-rw-  2.0 fat     4013 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3997 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     4010 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3994 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3939 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json
--rw-rw-rw-  2.0 fat     3911 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json
--rw-rw-rw-  2.0 fat      894 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json
--rw-rw-rw-  2.0 fat      888 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json
--rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3106 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3922 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3930 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
--rw-rw-rw-  2.0 fat     3914 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
--rw-rw-rw-  2.0 fat     4013 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3997 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     4010 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3994 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3954 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_aarch64/resource.json
--rw-rw-rw-  2.0 fat     3938 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_x86_64/resource.json
--rw-rw-rw-  2.0 fat     3975 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json
--rw-rw-rw-  2.0 fat     3947 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json
--rw-rw-rw-  2.0 fat     3619 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/CANN_6.0.1.json
--rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/CANN_6.0.RC1.json
--rw-rw-rw-  2.0 fat     3696 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/CANN_6.3.RC1.json
--rw-rw-rw-  2.0 fat     3987 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/CANN_6.3.RC2.json
--rw-rw-rw-  2.0 fat     3986 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/CANN_7.0.RC1.json
--rw-rw-rw-  2.0 fat      196 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/DL_5.0.RC1.json
--rw-rw-rw-  2.0 fat      196 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/DL_5.0.RC2.json
--rw-rw-rw-  2.0 fat      195 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/DL_5.0.RC3.json
--rw-rw-rw-  2.0 fat       86 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MEF_5.0.RC1.json
--rw-rw-rw-  2.0 fat       85 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MEF_5.0.RC2.json
--rw-rw-rw-  2.0 fat     2847 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindSpore_1.10.0.json
--rw-rw-rw-  2.0 fat     2828 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindSpore_1.9.0.json
--rw-rw-rw-  2.0 fat     2807 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
--rw-rw-rw-  2.0 fat     2750 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindSpore_2.1.0.json
--rw-rw-rw-  2.0 fat     2749 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindSpore_2.2.0.json
--rw-rw-rw-  2.0 fat    48361 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindStudio_5.0.0.json
--rw-rw-rw-  2.0 fat    25492 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
--rw-rw-rw-  2.0 fat    48369 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
--rw-rw-rw-  2.0 fat    48675 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/MindStudio_6.0.RC2.json
--rw-rw-rw-  2.0 fat     1461 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/NPU_23.0.RC1.json
--rw-rw-rw-  2.0 fat     1814 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/NPU_23.0.RC2.json
--rw-rw-rw-  2.0 fat     2152 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/NPU_23.0.RC3.json
--rw-rw-rw-  2.0 fat     2078 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/NPU_6.0.0.json
--rw-rw-rw-  2.0 fat     3408 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/NPU_6.0.RC1.json
--rw-rw-rw-  2.0 fat     1103 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/TensorFlow_1.15.0.json
--rw-rw-rw-  2.0 fat     1097 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/TensorFlow_2.6.5.json
--rw-rw-rw-  2.0 fat     2931 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.11.0.json
--rw-rw-rw-  2.0 fat     5649 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.11.0.post1.json
--rw-rw-rw-  2.0 fat     5654 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json
--rw-rw-rw-  2.0 fat     2946 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
--rw-rw-rw-  2.0 fat     2935 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.8.1.json
--rw-rw-rw-  2.0 fat     2960 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
--rw-rw-rw-  2.0 fat     5624 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/software/Torch-npu_1.8.1.post2.json
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/yum_metadata/__init__.py
--rw-rw-rw-  2.0 fat     1772 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
--rw-rw-rw-  2.0 fat    11352 b- defN 24-Mar-25 02:31 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
--rw-rw-rw-  2.0 fat     1897 b- defN 24-Mar-25 02:31 ascend_deployer/group_vars/all.yaml
--rw-rw-rw-  2.0 fat      807 b- defN 24-Mar-25 02:31 ascend_deployer/patch/selenium_firefox.patch
--rw-rw-rw-  2.0 fat     1127 b- defN 24-Mar-25 02:31 ascend_deployer/patch/selenium_firefox_profile.patch
--rw-rw-rw-  2.0 fat      236 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/basic.yaml
--rw-rw-rw-  2.0 fat      539 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/check.yaml
--rw-rw-rw-  2.0 fat      479 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/check_mef.yaml
--rw-rw-rw-  2.0 fat       94 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/check_pkgs.yml
--rw-rw-rw-  2.0 fat      451 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/clean_nexus.yml
--rw-rw-rw-  2.0 fat      611 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/create_nexus.yml
--rw-rw-rw-  2.0 fat      540 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/create_user.yml
--rw-rw-rw-  2.0 fat      663 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/distribution.yml
--rw-rw-rw-  2.0 fat     1003 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/docker.yaml
--rw-rw-rw-  2.0 fat     1021 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/gather_app_info.yml
--rw-rw-rw-  2.0 fat     3487 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/gather_facts.yaml
--rw-rw-rw-  2.0 fat     1254 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/gather_npu_fact.yml
--rw-rw-rw-  2.0 fat      121 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/harbor.yaml
--rw-rw-rw-  2.0 fat      193 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/hccn.yaml
--rw-rw-rw-  2.0 fat      133 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/image_load.yaml
--rw-rw-rw-  2.0 fat     2144 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/k8s.yaml
--rw-rw-rw-  2.0 fat       85 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/kubeedge.yaml
--rw-rw-rw-  2.0 fat     2742 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/mindxdl.yaml
--rw-rw-rw-  2.0 fat      491 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/modify_user_group.yml
--rw-rw-rw-  2.0 fat      264 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/os_map.yaml
--rw-rw-rw-  2.0 fat     2267 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/os_map.yml
--rw-rw-rw-  2.0 fat     1056 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
--rw-rw-rw-  2.0 fat     1056 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
--rw-rw-rw-  2.0 fat     1652 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_Kylin_V10Sword_aarch64.yml
--rw-rw-rw-  2.0 fat     1653 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml
--rw-rw-rw-  2.0 fat     1653 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml
--rw-rw-rw-  2.0 fat     1652 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
--rw-rw-rw-  2.0 fat     1652 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
--rw-rw-rw-  2.0 fat      575 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/report.yaml
--rw-rw-rw-  2.0 fat      139 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/set_facts_cache_permission.yml
--rw-rw-rw-  2.0 fat      349 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/sync_time.yml
--rw-rw-rw-  2.0 fat     6776 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/task_set_custom_fact.yml
--rw-rw-rw-  2.0 fat      155 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
--rw-rw-rw-  2.0 fat      246 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/uninstall_mef_releate.yaml
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/callback_plugins/__init__.py
--rw-rw-rw-  2.0 fat      464 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/callback_plugins/crop_columns.py
--rw-rw-rw-  2.0 fat     5199 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/facts/app_info.fact.j2
--rw-rw-rw-  2.0 fat     7171 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/facts/npu_info.fact.j2
--rw-rw-rw-  2.0 fat      107 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_ascend-device-plugin.yml
--rw-rw-rw-  2.0 fat      109 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml
--rw-rw-rw-  2.0 fat      110 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_ascend-operator.yml
--rw-rw-rw-  2.0 fat      584 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_atlasedge.yml
--rw-rw-rw-  2.0 fat      502 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_docker_images.yml
--rw-rw-rw-  2.0 fat     1299 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_driver.yml
--rw-rw-rw-  2.0 fat     1332 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_firmware.yml
--rw-rw-rw-  2.0 fat      896 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_gcc.yml
--rw-rw-rw-  2.0 fat      557 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_ha.yml
--rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_hccl-controller.yml
--rw-rw-rw-  2.0 fat      462 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_ief.yml
--rw-rw-rw-  2.0 fat      102 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_kernels.yml
--rw-rw-rw-  2.0 fat      101 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_mindio.yml
--rw-rw-rw-  2.0 fat      927 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_mindspore.yml
--rw-rw-rw-  2.0 fat     6464 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_mindstudio.yml
--rw-rw-rw-  2.0 fat       96 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_nnae.yml
--rw-rw-rw-  2.0 fat       96 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_nnrt.yml
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_noded.yml
--rw-rw-rw-  2.0 fat      107 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_npu-exporter.yml
--rw-rw-rw-  2.0 fat     1398 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_npu.yml
--rw-rw-rw-  2.0 fat      105 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_python.yml
--rw-rw-rw-  2.0 fat     2728 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_pytorch.yml
--rw-rw-rw-  2.0 fat      116 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_resilience-controller.yml
--rw-rw-rw-  2.0 fat      487 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_sys_pkg.yml
--rw-rw-rw-  2.0 fat     3278 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_tensorflow.yml
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_tfplugin.yml
--rw-rw-rw-  2.0 fat      102 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_toolbox.yml
--rw-rw-rw-  2.0 fat      102 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_toolkit.yml
--rw-rw-rw-  2.0 fat      115 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/install_volcano.yml
--rw-rw-rw-  2.0 fat     1490 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_atlasedge.yml
--rw-rw-rw-  2.0 fat      663 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_cmake.yml
--rw-rw-rw-  2.0 fat      995 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_dl.yml
--rw-rw-rw-  2.0 fat      818 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_docker_images.yml
--rw-rw-rw-  2.0 fat       81 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_driver.yml
--rw-rw-rw-  2.0 fat     6900 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_driver_common.yml
--rw-rw-rw-  2.0 fat     6419 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_firmware.yml
--rw-rw-rw-  2.0 fat     2210 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_gcc.yml
--rw-rw-rw-  2.0 fat     3055 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_get_npu_scene.yml
--rw-rw-rw-  2.0 fat     1253 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_ha.yml
--rw-rw-rw-  2.0 fat      670 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_ief.yml
--rw-rw-rw-  2.0 fat     2777 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_ief_a500.yml
--rw-rw-rw-  2.0 fat     1665 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_ief_a500pro.yml
--rw-rw-rw-  2.0 fat     1337 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_kernel.yml
--rw-rw-rw-  2.0 fat     1242 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_kernel_euleros.yml
--rw-rw-rw-  2.0 fat     8921 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_kernels.yml
--rw-rw-rw-  2.0 fat     1273 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_mindspore.yml
--rw-rw-rw-  2.0 fat     2155 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_mpi.yml
--rw-rw-rw-  2.0 fat     3226 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_nnae.yml
--rw-rw-rw-  2.0 fat     3232 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_nnrt.yml
--rw-rw-rw-  2.0 fat      709 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_protobuf.yml
--rw-rw-rw-  2.0 fat     3209 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_python.yml
--rw-rw-rw-  2.0 fat     1286 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_pytorch.yml
--rw-rw-rw-  2.0 fat     1812 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_sys_apt.yml
--rw-rw-rw-  2.0 fat     2467 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_sys_dnf.yml
--rw-rw-rw-  2.0 fat     3557 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_sys_pkg.yml
--rw-rw-rw-  2.0 fat     3113 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_sys_yum.yml
--rw-rw-rw-  2.0 fat     1073 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_tensorflow.yml
--rw-rw-rw-  2.0 fat     3436 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_tfplugin.yml
--rw-rw-rw-  2.0 fat     3329 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_toolbox.yml
--rw-rw-rw-  2.0 fat     6600 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/task_toolkit.yml
--rw-rw-rw-  2.0 fat      102 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/install_nnae.yml
--rw-rw-rw-  2.0 fat      102 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/install_nnrt.yml
--rw-rw-rw-  2.0 fat      110 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
--rw-rw-rw-  2.0 fat      108 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/install_toolkit.yml
--rw-rw-rw-  2.0 fat      106 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
--rw-rw-rw-  2.0 fat      106 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
--rw-rw-rw-  2.0 fat      114 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
--rw-rw-rw-  2.0 fat      112 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
--rw-rw-rw-  2.0 fat     1378 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_nnae.yml
--rw-rw-rw-  2.0 fat     1378 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_nnrt.yml
--rw-rw-rw-  2.0 fat      663 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
--rw-rw-rw-  2.0 fat     1680 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
--rw-rw-rw-  2.0 fat      726 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
--rw-rw-rw-  2.0 fat     1693 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
--rw-rw-rw-  2.0 fat     1445 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_tfplugin.yml
--rw-rw-rw-  2.0 fat     1285 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/install/patch/task_toolkit.yml
--rw-rw-rw-  2.0 fat      369 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_check.yml
--rw-rw-rw-  2.0 fat     3765 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_install.yml
--rw-rw-rw-  2.0 fat      783 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_patch.yml
--rw-rw-rw-  2.0 fat      787 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_patch_rollback.yml
--rw-rw-rw-  2.0 fat     2144 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_scene.yml
--rw-rw-rw-  2.0 fat     1049 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/process/process_test.yml
--rw-rw-rw-  2.0 fat      312 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
--rw-rw-rw-  2.0 fat     1258 b- defN 24-Mar-25 07:43 ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
--rw-rw-rw-  2.0 fat     2771 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
--rw-rw-rw-  2.0 fat     1378 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/check_driver.yml
--rw-rw-rw-  2.0 fat     1392 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml
--rw-rw-rw-  2.0 fat     2256 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
--rw-rw-rw-  2.0 fat     4784 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
--rw-rw-rw-  2.0 fat     4892 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
--rw-rw-rw-  2.0 fat    13754 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
--rw-rw-rw-  2.0 fat      335 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
--rw-rw-rw-  2.0 fat       76 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/README.md
--rw-rw-rw-  2.0 fat     1379 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
--rw-rw-rw-  2.0 fat      181 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
--rw-rw-rw-  2.0 fat     5474 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml
--rw-rw-rw-  2.0 fat    11032 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
--rw-rw-rw-  2.0 fat      675 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
--rw-rw-rw-  2.0 fat     9970 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
--rw-rw-rw-  2.0 fat     7728 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
--rw-rw-rw-  2.0 fat      510 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
--rw-rw-rw-  2.0 fat     1673 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
--rw-rw-rw-  2.0 fat     5087 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
--rw-rw-rw-  2.0 fat      324 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/label_master.yaml
--rw-rw-rw-  2.0 fat     5357 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/label_worker.yaml
--rw-rw-rw-  2.0 fat     3083 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/mindio.yaml
--rw-rw-rw-  2.0 fat     5118 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
--rw-rw-rw-  2.0 fat     4808 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
--rw-rw-rw-  2.0 fat     3874 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
--rw-rw-rw-  2.0 fat     5747 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml
--rw-rw-rw-  2.0 fat     5981 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
--rw-rw-rw-  2.0 fat     1259 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/templates/drc.conf
--rw-rw-rw-  2.0 fat     1038 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/templates/memfs.conf
--rw-rw-rw-  2.0 fat      110 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.dl/templates/ockiod.conf
--rw-rw-rw-  2.0 fat       67 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/README.md
--rw-rw-rw-  2.0 fat      171 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
--rw-rw-rw-  2.0 fat      347 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
--rw-rw-rw-  2.0 fat      418 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
--rw-rw-rw-  2.0 fat      474 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_nerdctl.yml
--rw-rw-rw-  2.0 fat     1135 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
--rw-rw-rw-  2.0 fat     1160 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
--rw-rw-rw-  2.0 fat       55 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
--rw-rw-rw-  2.0 fat       37 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
--rw-rw-rw-  2.0 fat      116 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
--rw-rw-rw-  2.0 fat      272 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
--rw-rw-rw-  2.0 fat     1314 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
--rw-rw-rw-  2.0 fat     1158 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
--rw-rw-rw-  2.0 fat      346 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
--rw-rw-rw-  2.0 fat     1382 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
--rw-rw-rw-  2.0 fat       42 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
--rw-rw-rw-  2.0 fat     1723 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
--rw-rw-rw-  2.0 fat      660 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
--rw-rw-rw-  2.0 fat      536 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/README.md
--rw-rw-rw-  2.0 fat      400 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
--rw-rw-rw-  2.0 fat      929 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
--rw-rw-rw-  2.0 fat      283 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
--rw-rw-rw-  2.0 fat      179 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
--rw-rw-rw-  2.0 fat      691 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
--rw-rw-rw-  2.0 fat     1008 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
--rw-rw-rw-  2.0 fat      774 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
--rw-rw-rw-  2.0 fat     1251 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
--rw-rw-rw-  2.0 fat     1237 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
--rw-rw-rw-  2.0 fat     1032 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
--rw-rw-rw-  2.0 fat     4329 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
--rw-rw-rw-  2.0 fat     2000 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
--rw-rw-rw-  2.0 fat     3854 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
--rw-rw-rw-  2.0 fat     1852 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
--rw-rw-rw-  2.0 fat      860 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
--rw-rw-rw-  2.0 fat   202740 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
--rw-rw-rw-  2.0 fat   237804 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.25.0.ipv6.yaml
--rw-rw-rw-  2.0 fat       55 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
--rw-rw-rw-  2.0 fat       37 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
--rw-rw-rw-  2.0 fat      116 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
--rw-rw-rw-  2.0 fat      539 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
--rw-rw-rw-  2.0 fat       78 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
--rw-rw-rw-  2.0 fat      243 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
--rw-rw-rw-  2.0 fat      162 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
--rw-rw-rw-  2.0 fat     1896 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
--rw-rw-rw-  2.0 fat     8715 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
--rw-rw-rw-  2.0 fat    10576 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
--rw-rw-rw-  2.0 fat     1877 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
--rw-rw-rw-  2.0 fat     2443 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
--rw-rw-rw-  2.0 fat     1355 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
--rw-rw-rw-  2.0 fat      176 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
--rw-rw-rw-  2.0 fat     4514 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
--rw-rw-rw-  2.0 fat      144 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
--rw-rw-rw-  2.0 fat      591 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
--rw-rw-rw-  2.0 fat     2537 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
--rw-rw-rw-  2.0 fat     2640 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
--rw-rw-rw-  2.0 fat     8253 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
--rw-rw-rw-  2.0 fat     1368 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
--rw-rw-rw-  2.0 fat     1012 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
--rw-rw-rw-  2.0 fat      786 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
--rw-rw-rw-  2.0 fat     2037 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
--rw-rw-rw-  2.0 fat      389 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
--rw-rw-rw-  2.0 fat      390 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
--rw-rw-rw-  2.0 fat      960 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_auto.yml
--rw-rw-rw-  2.0 fat      613 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_dl.yml
--rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_edge.yml
--rw-rw-rw-  2.0 fat      361 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_mef.yml
--rw-rw-rw-  2.0 fat      514 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_mindspore.yml
--rw-rw-rw-  2.0 fat      435 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_offline_dev.yml
--rw-rw-rw-  2.0 fat      354 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_offline_run.yml
--rw-rw-rw-  2.0 fat      510 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
--rw-rw-rw-  2.0 fat      504 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
--rw-rw-rw-  2.0 fat      593 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
--rw-rw-rw-  2.0 fat      587 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
--rw-rw-rw-  2.0 fat      273 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/scene/scene_vmhost.yml
--rw-rw-rw-  2.0 fat     2673 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_driver.yml
--rw-rw-rw-  2.0 fat     1169 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_firmware.yml
--rw-rw-rw-  2.0 fat     3166 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_mindspore.yml
--rw-rw-rw-  2.0 fat     1049 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_nnae.yml
--rw-rw-rw-  2.0 fat     1047 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_nnrt.yml
--rw-rw-rw-  2.0 fat     3619 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_pytorch.yml
--rw-rw-rw-  2.0 fat     7799 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_tensorflow.yml
--rw-rw-rw-  2.0 fat      545 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_tfplugin.yml
--rw-rw-rw-  2.0 fat     1473 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_toolbox.yml
--rw-rw-rw-  2.0 fat     1110 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/case_toolkit.yml
--rw-rw-rw-  2.0 fat      608 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_all.yml
--rw-rw-rw-  2.0 fat      284 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_driver.yml
--rw-rw-rw-  2.0 fat      114 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_exhibit.yml
--rw-rw-rw-  2.0 fat      284 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_firmware.yml
--rw-rw-rw-  2.0 fat       99 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_mindspore.yml
--rw-rw-rw-  2.0 fat       90 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_nnae.yml
--rw-rw-rw-  2.0 fat       89 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_nnrt.yml
--rw-rw-rw-  2.0 fat       96 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_pytorch.yml
--rw-rw-rw-  2.0 fat      101 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_tensorflow.yml
--rw-rw-rw-  2.0 fat       97 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_tfplugin.yml
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_toolbox.yml
--rw-rw-rw-  2.0 fat       95 b- defN 24-Mar-25 02:31 ascend_deployer/playbooks/test/test_toolkit.yml
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 02:31 ascend_deployer/scripts/__init__.py
--rw-rw-rw-  2.0 fat    21173 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/check_pkgs.sh
--rw-rw-rw-  2.0 fat    11154 b- defN 24-Mar-25 02:31 ascend_deployer/scripts/eula_cn.txt
--rw-rw-rw-  2.0 fat    12908 b- defN 24-Mar-25 02:31 ascend_deployer/scripts/eula_en.txt
--rw-rw-rw-  2.0 fat     1116 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/hccn_set.sh
--rw-rw-rw-  2.0 fat     1104 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/image_load.sh
--rw-rw-rw-  2.0 fat      969 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/install.sh
--rw-rw-rw-  2.0 fat     3587 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/install_ansible.sh
--rw-rw-rw-  2.0 fat    16509 b- defN 24-Mar-25 02:31 ascend_deployer/scripts/nexus.py
--rw-rw-rw-  2.0 fat     1380 b- defN 24-Mar-25 02:31 ascend_deployer/scripts/nexus_config.json
--rw-rw-rw-  2.0 fat    15205 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/prepare.sh
--rw-rw-rw-  2.0 fat      535 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/uninstall_k8s_docker.sh
--rw-rw-rw-  2.0 fat      643 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/uninstall_mef_kubeedge.sh
--rw-rw-rw-  2.0 fat      679 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/uninstall_mef_related.sh
--rw-rw-rw-  2.0 fat     5723 b- defN 24-Mar-25 07:43 ascend_deployer/scripts/utils.sh
--rw-rw-rw-  2.0 fat    10900 b- defN 24-Mar-25 07:43 ascend_deployer/tools/DeviceIP-conf.sh
--rw-rw-rw-  2.0 fat     4049 b- defN 24-Mar-25 02:31 ascend_deployer/tools/check.py
--rw-rw-rw-  2.0 fat     9718 b- defN 24-Mar-25 02:31 ascend_deployer/tools/hccn.py
--rw-rw-rw-  2.0 fat     9930 b- defN 24-Mar-25 07:43 ascend_deployer/tools/update_crl.sh
--rw-rw-rw-  2.0 fat       21 b- defN 24-Mar-25 02:31 ascend_deployer/tools/hccn/main/go.mod
--rw-rw-rw-  2.0 fat     6863 b- defN 24-Mar-25 02:31 ascend_deployer/tools/hccn/main/hccn.go
--rw-rw-rw-  2.0 fat     2373 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/README.rst
--rw-rw-rw-  2.0 fat      314 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/image/dockerfile
--rw-rw-rw-  2.0 fat      665 b- defN 24-Mar-25 07:43 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/driver-install.sh
--rw-rw-rw-  2.0 fat     1658 b- defN 24-Mar-25 07:43 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/exec.sh
--rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-arm-installer.yaml
--rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-x86-installer.yaml
--rw-rw-rw-  2.0 fat      703 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-arm-installer.yaml
--rw-rw-rw-  2.0 fat      703 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-x86-installer.yaml
--rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-arm-installer.yaml
--rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-25 02:31 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-x86-installer.yaml
--rw-rw-rw-  2.0 fat     4260 b- defN 24-Mar-25 02:31 ascend_deployer/tools/nexus/Dockerfile
--rw-rw-rw-  2.0 fat      142 b- defN 24-Mar-25 02:31 ascend_deployer/tools/report/main/go.mod
--rw-rw-rw-  2.0 fat    18729 b- defN 24-Mar-25 02:31 ascend_deployer/tools/report/main/main.go
--rw-rw-rw-  2.0 fat       21 b- defN 24-Mar-25 02:31 ascend_deployer/tools/unzip/main/go.mod
--rw-rw-rw-  2.0 fat     1587 b- defN 24-Mar-25 02:31 ascend_deployer/tools/unzip/main/unzip.go
--rw-rw-rw-  2.0 fat       46 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/basic.yaml
--rw-rw-rw-  2.0 fat       46 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/check.yaml
--rw-rw-rw-  2.0 fat      132 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/docker.yaml
--rw-rw-rw-  2.0 fat       53 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/gather_facts.yaml
--rw-rw-rw-  2.0 fat       72 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/harbor.yaml
--rw-rw-rw-  2.0 fat       45 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/hccn.yaml
--rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/image_load.yaml
--rw-rw-rw-  2.0 fat      126 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/k8s.yaml
--rw-rw-rw-  2.0 fat      351 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/k8s_reset.yaml
--rw-rw-rw-  2.0 fat       74 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/mindxdl.yaml
--rw-rw-rw-  2.0 fat       47 b- defN 24-Mar-25 02:31 ascend_deployer/yamls/report.yaml
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3227 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/NOTICE
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      128 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       16 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    57199 b- defN 24-Mar-25 07:43 ascend_deployer-5.0.6.dist-info/RECORD
-498 files, 2754053 bytes uncompressed, 542565 bytes compressed:  80.3%
+Zip file size: 559412 bytes, number of entries: 419
+-rw-rw-rw-  2.0 fat      769 b- defN 24-Mar-27 11:28 ascend_deployer/__init__.py
+-rw-rw-rw-  2.0 fat      516 b- defN 24-Mar-27 11:28 ascend_deployer/ansible.cfg
+-rw-rw-rw-  2.0 fat     8717 b- defN 24-Mar-27 11:28 ascend_deployer/ascend_deployer.py
+-rw-rw-rw-  2.0 fat     2174 b- defN 24-Mar-27 11:28 ascend_deployer/ascend_download.py
+-rw-rw-rw-  2.0 fat     6179 b- defN 24-Mar-27 11:28 ascend_deployer/downloader_ui.py
+-rw-rw-rw-  2.0 fat      409 b- defN 24-Apr-26 09:50 ascend_deployer/install.sh
+-rw-rw-rw-  2.0 fat      530 b- defN 24-Mar-27 11:28 ascend_deployer/inventory_file
+-rw-rw-rw-  2.0 fat    23290 b- defN 24-Mar-27 11:28 ascend_deployer/jobs.py
+-rw-rw-rw-  2.0 fat      475 b- defN 24-Apr-26 09:50 ascend_deployer/start_download.sh
+-rw-rw-rw-  2.0 fat       69 b- defN 24-Mar-27 11:28 ascend_deployer/start_download_ui.bat
+-rw-rw-rw-  2.0 fat     9686 b- defN 24-Mar-27 11:28 ascend_deployer/utils.py
+-rw-rw-rw-  2.0 fat       54 b- defN 24-Mar-27 11:28 ascend_deployer/version.json
+-rw-rw-rw-  2.0 fat    14692 b- defN 24-Mar-27 11:28 ascend_deployer/ansible_plugin/ansible_log.py
+-rw-rw-rw-  2.0 fat    23041 b- defN 24-Mar-27 11:28 ascend_deployer/ansible_plugin/deploy_info_output_plugin.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 24-Mar-27 11:28 ascend_deployer/ansible_plugin/install_info.yaml
+-rw-rw-rw-  2.0 fat     4478 b- defN 24-Mar-27 11:28 ascend_deployer/ansible_plugin/progress_config.json
+-rw-rw-rw-  2.0 fat     2002 b- defN 24-Mar-27 11:28 ascend_deployer/ansible_plugin/standard.py
+-rw-rw-rw-  2.0 fat      706 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/__init__.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/ansible_reqs.json
+-rw-rw-rw-  2.0 fat      176 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config.ini
+-rw-rw-rw-  2.0 fat    11086 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/deb_downloader.py
+-rw-rw-rw-  2.0 fat     5682 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dl_mef_dependency_downloader.py
+-rw-rw-rw-  2.0 fat     2225 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/download_data.py
+-rw-rw-rw-  2.0 fat    16037 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/download_util.py
+-rw-rw-rw-  2.0 fat    11656 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/downloader.py
+-rw-rw-rw-  2.0 fat     4536 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/logger_config.py
+-rw-rw-rw-  2.0 fat     2839 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/obs_downloader.py
+-rw-rw-rw-  2.0 fat     2132 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/obs_resources.json
+-rw-rw-rw-  2.0 fat     5177 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/os_dep_downloader.py
+-rw-rw-rw-  2.0 fat     7534 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/other_downloader.py
+-rw-rw-rw-  2.0 fat     1485 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/other_resources.json
+-rw-rw-rw-  2.0 fat    14990 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/parallel_file_downloader.py
+-rw-rw-rw-  2.0 fat     8153 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/pip_downloader.py
+-rw-rw-rw-  2.0 fat    11880 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/python_version.json
+-rw-rw-rw-  2.0 fat     1811 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/requirements.txt
+-rw-rw-rw-  2.0 fat    20222 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/rpm_downloader.py
+-rw-rw-rw-  2.0 fat    13898 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software_mgr.py
+-rw-rw-rw-  2.0 fat     1135 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/version_match.json
+-rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      157 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    65719 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     3627 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      262 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/source.repo
+-rw-rw-rw-  2.0 fat     8382 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      234 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
+-rw-rw-rw-  2.0 fat     8533 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      223 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
+-rw-rw-rw-  2.0 fat    43257 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     6521 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      131 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    42707 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
+-rw-rw-rw-  2.0 fat     5741 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat       65 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
+-rw-rw-rw-  2.0 fat    65900 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat    10119 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      130 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    42840 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     9168 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      130 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    42208 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
+-rw-rw-rw-  2.0 fat     8706 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat       65 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
+-rw-rw-rw-  2.0 fat    55524 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     4071 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      263 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    60396 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     3368 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    60964 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
+-rw-rw-rw-  2.0 fat     3181 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      248 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
+-rw-rw-rw-  2.0 fat    60396 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     3565 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Kylin_V10_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    51454 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     3546 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      365 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    51932 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
+-rw-rw-rw-  2.0 fat     3828 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      353 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
+-rw-rw-rw-  2.0 fat    51351 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat     5809 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      458 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
+-rw-rw-rw-  2.0 fat    43010 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
+-rw-rw-rw-  2.0 fat     3442 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      445 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1050e_aarch64/installed.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1050e_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/UOS_20-1050e_aarch64/source.repo
+-rw-rw-rw-  2.0 fat     5790 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      370 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
+-rw-rw-rw-  2.0 fat     7004 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      352 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
+-rw-rw-rw-  2.0 fat     5391 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      366 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
+-rw-rw-rw-  2.0 fat     6021 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      348 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
+-rw-rw-rw-  2.0 fat     6325 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
+-rw-rw-rw-  2.0 fat      366 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
+-rw-rw-rw-  2.0 fat     6764 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
+-rw-rw-rw-  2.0 fat      348 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
+-rw-rw-rw-  2.0 fat     3106 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_x86_64.json
+-rw-rw-rw-  2.0 fat      338 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat      336 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat     1429 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/UOS_20-1050e_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
+-rw-rw-rw-  2.0 fat     4761 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/DL/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     4727 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.0/DL/x86_64/resource.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
+-rw-rw-rw-  2.0 fat     4225 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     4191 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
+-rw-rw-rw-  2.0 fat     1695 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     1687 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
+-rw-rw-rw-  2.0 fat     3106 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_x86_64.json
+-rw-rw-rw-  2.0 fat      338 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat      336 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
+-rw-rw-rw-  2.0 fat     4449 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     4421 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json
+-rw-rw-rw-  2.0 fat     1404 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     1395 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
+-rw-rw-rw-  2.0 fat     3106 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_x86_64.json
+-rw-rw-rw-  2.0 fat      338 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat      336 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
+-rw-rw-rw-  2.0 fat     4485 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json
+-rw-rw-rw-  2.0 fat     4454 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json
+-rw-rw-rw-  2.0 fat     3428 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_aarch64.json
+-rw-rw-rw-  2.0 fat     3412 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_x86_64.json
+-rw-rw-rw-  2.0 fat     3500 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat     3484 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat     3500 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_aarch64.json
+-rw-rw-rw-  2.0 fat     3484 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_x86_64.json
+-rw-rw-rw-  2.0 fat     3444 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_aarch64.json
+-rw-rw-rw-  2.0 fat     3428 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_x86_64.json
+-rw-rw-rw-  2.0 fat     3444 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_aarch64.json
+-rw-rw-rw-  2.0 fat     3428 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_x86_64.json
+-rw-rw-rw-  2.0 fat     3444 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_aarch64.json
+-rw-rw-rw-  2.0 fat     3429 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_x86_64.json
+-rw-rw-rw-  2.0 fat     3619 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_6.0.1.json
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_6.0.RC1.json
+-rw-rw-rw-  2.0 fat     3696 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_6.3.RC1.json
+-rw-rw-rw-  2.0 fat     3987 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_6.3.RC2.json
+-rw-rw-rw-  2.0 fat     3904 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_7.0.0.json
+-rw-rw-rw-  2.0 fat     3987 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/CANN_7.0.RC1.json
+-rw-rw-rw-  2.0 fat      191 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/DL_5.0.0.json
+-rw-rw-rw-  2.0 fat      196 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/DL_5.0.RC1.json
+-rw-rw-rw-  2.0 fat      196 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/DL_5.0.RC2.json
+-rw-rw-rw-  2.0 fat      196 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/DL_5.0.RC3.json
+-rw-rw-rw-  2.0 fat       86 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MEF_5.0.RC1.json
+-rw-rw-rw-  2.0 fat       85 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MEF_5.0.RC2.json
+-rw-rw-rw-  2.0 fat     2847 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_1.10.0.json
+-rw-rw-rw-  2.0 fat     2828 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_1.9.0.json
+-rw-rw-rw-  2.0 fat     2807 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
+-rw-rw-rw-  2.0 fat     2750 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_2.1.0.json
+-rw-rw-rw-  2.0 fat     2750 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_2.2.0.json
+-rw-rw-rw-  2.0 fat     2768 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindSpore_2.2.10.json
+-rw-rw-rw-  2.0 fat    48361 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindStudio_5.0.0.json
+-rw-rw-rw-  2.0 fat    25492 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
+-rw-rw-rw-  2.0 fat    48369 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
+-rw-rw-rw-  2.0 fat    48675 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/MindStudio_6.0.RC2.json
+-rw-rw-rw-  2.0 fat     2114 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_23.0.0.json
+-rw-rw-rw-  2.0 fat     1461 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_23.0.RC1.json
+-rw-rw-rw-  2.0 fat     1814 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_23.0.RC2.json
+-rw-rw-rw-  2.0 fat     2153 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_23.0.RC3.json
+-rw-rw-rw-  2.0 fat     2078 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_6.0.0.json
+-rw-rw-rw-  2.0 fat     3408 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/NPU_6.0.RC1.json
+-rw-rw-rw-  2.0 fat     1103 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/TensorFlow_1.15.0.json
+-rw-rw-rw-  2.0 fat     2856 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/TensorFlow_2.6.5.json
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.11.0.json
+-rw-rw-rw-  2.0 fat     5649 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.11.0.post1.json
+-rw-rw-rw-  2.0 fat     5655 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json
+-rw-rw-rw-  2.0 fat     7559 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.11.0.post8.json
+-rw-rw-rw-  2.0 fat     2946 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
+-rw-rw-rw-  2.0 fat     2935 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.8.1.json
+-rw-rw-rw-  2.0 fat     2960 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
+-rw-rw-rw-  2.0 fat     5624 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_1.8.1.post2.json
+-rw-rw-rw-  2.0 fat     5756 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_2.0.1.post1.json
+-rw-rw-rw-  2.0 fat     6181 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/software/Torch-npu_2.1.0.json
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/yum_metadata/__init__.py
+-rw-rw-rw-  2.0 fat     1772 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
+-rw-rw-rw-  2.0 fat    11352 b- defN 24-Mar-27 11:28 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
+-rw-rw-rw-  2.0 fat     2036 b- defN 24-Mar-27 11:28 ascend_deployer/group_vars/all.yaml
+-rw-rw-rw-  2.0 fat     5293 b- defN 24-Mar-27 11:28 ascend_deployer/library/check_compatibility.py
+-rw-rw-rw-  2.0 fat     2521 b- defN 24-Mar-27 11:28 ascend_deployer/library/check_nexus_status.py
+-rw-rw-rw-  2.0 fat     9223 b- defN 24-Mar-27 11:28 ascend_deployer/library/check_status.py
+-rw-rw-rw-  2.0 fat     2847 b- defN 24-Mar-27 11:28 ascend_deployer/library/collect_info.py
+-rw-rw-rw-  2.0 fat     1637 b- defN 24-Mar-27 11:28 ascend_deployer/library/create_user.py
+-rw-rw-rw-  2.0 fat     1499 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_ascend_operator.py
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_cann.py
+-rw-rw-rw-  2.0 fat     6689 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_device_plugin.py
+-rw-rw-rw-  2.0 fat     3506 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_docker_runtime.py
+-rw-rw-rw-  2.0 fat     1543 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_hccl_controller.py
+-rw-rw-rw-  2.0 fat     2636 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_mindio.py
+-rw-rw-rw-  2.0 fat     1497 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_noded.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_npu_exporter.py
+-rw-rw-rw-  2.0 fat     4748 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_python.py
+-rw-rw-rw-  2.0 fat     1589 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_resilience_controller.py
+-rw-rw-rw-  2.0 fat     9563 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_sys_pkg.py
+-rw-rw-rw-  2.0 fat     3554 b- defN 24-Mar-27 11:28 ascend_deployer/library/install_volcano.py
+-rw-rw-rw-  2.0 fat     4642 b- defN 24-Mar-27 11:28 ascend_deployer/library/login_harbor.py
+-rw-rw-rw-  2.0 fat    13435 b- defN 24-Mar-27 11:28 ascend_deployer/library/process_framework.py
+-rw-rw-rw-  2.0 fat    11726 b- defN 24-Mar-27 11:28 ascend_deployer/library/process_npu.py
+-rw-rw-rw-  2.0 fat    11157 b- defN 24-Mar-27 11:28 ascend_deployer/library/process_test.py
+-rw-rw-rw-  2.0 fat     6341 b- defN 24-Mar-27 11:28 ascend_deployer/library/push_image.py
+-rw-rw-rw-  2.0 fat     3976 b- defN 24-Mar-27 11:28 ascend_deployer/library/scp.py
+-rw-rw-rw-  2.0 fat     7956 b- defN 24-Mar-27 11:28 ascend_deployer/library/system_report.py
+-rw-rw-rw-  2.0 fat     4230 b- defN 24-Mar-27 11:28 ascend_deployer/library/uncompress_resources.py
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/__init__.py
+-rw-rw-rw-  2.0 fat     5499 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/check_output_manager.py
+-rw-rw-rw-  2.0 fat    13373 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/common_info.py
+-rw-rw-rw-  2.0 fat     4184 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/common_utils.py
+-rw-rw-rw-  2.0 fat    21172 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/compatibility_config.py
+-rw-rw-rw-  2.0 fat    15802 b- defN 24-Mar-27 11:28 ascend_deployer/module_utils/dl.py
+-rw-rw-rw-  2.0 fat      607 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/check.yaml
+-rw-rw-rw-  2.0 fat      665 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/distribution.yml
+-rw-rw-rw-  2.0 fat     1095 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/docker.yaml
+-rw-rw-rw-  2.0 fat      591 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/gather_installation_facts.yml
+-rw-rw-rw-  2.0 fat      506 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/gather_npu_fact.yml
+-rw-rw-rw-  2.0 fat      398 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/harbor.yaml
+-rw-rw-rw-  2.0 fat      193 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/hccn.yaml
+-rw-rw-rw-  2.0 fat      133 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/image_load.yaml
+-rw-rw-rw-  2.0 fat     2284 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/k8s.yaml
+-rw-rw-rw-  2.0 fat       85 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/kubeedge.yaml
+-rw-rw-rw-  2.0 fat     1785 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/report.yaml
+-rw-rw-rw-  2.0 fat      349 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/sync_time.yml
+-rw-rw-rw-  2.0 fat      155 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+-rw-rw-rw-  2.0 fat      246 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/uninstall_mef_releate.yaml
+-rw-rw-rw-  2.0 fat     2262 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_ascend-device-plugin.yml
+-rw-rw-rw-  2.0 fat      172 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml
+-rw-rw-rw-  2.0 fat     2273 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_ascend-operator.yml
+-rw-rw-rw-  2.0 fat      646 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_atlasedge.yml
+-rw-rw-rw-  2.0 fat      532 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_docker_images.yml
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_driver.yml
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_firmware.yml
+-rw-rw-rw-  2.0 fat      612 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_ha.yml
+-rw-rw-rw-  2.0 fat     2273 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_hccl-controller.yml
+-rw-rw-rw-  2.0 fat      482 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_ief.yml
+-rw-rw-rw-  2.0 fat      476 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_kernels.yml
+-rw-rw-rw-  2.0 fat      649 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_mindio.yml
+-rw-rw-rw-  2.0 fat      284 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_mindspore.yml
+-rw-rw-rw-  2.0 fat     6672 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_mindstudio.yml
+-rw-rw-rw-  2.0 fat      441 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_nnae.yml
+-rw-rw-rw-  2.0 fat      441 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_nnrt.yml
+-rw-rw-rw-  2.0 fat     2113 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_noded.yml
+-rw-rw-rw-  2.0 fat     2225 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_npu-exporter.yml
+-rw-rw-rw-  2.0 fat      430 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_npu.yml
+-rw-rw-rw-  2.0 fat      238 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_python.yml
+-rw-rw-rw-  2.0 fat      279 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_pytorch.yml
+-rw-rw-rw-  2.0 fat     2369 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_resilience-controller.yml
+-rw-rw-rw-  2.0 fat     1225 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_sys_pkg.yml
+-rw-rw-rw-  2.0 fat      287 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_tensorflow.yml
+-rw-rw-rw-  2.0 fat      465 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_tfplugin.yml
+-rw-rw-rw-  2.0 fat      459 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_toolbox.yml
+-rw-rw-rw-  2.0 fat      498 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_toolkit.yml
+-rw-rw-rw-  2.0 fat     2158 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/install_volcano.yml
+-rw-rw-rw-  2.0 fat     1527 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_atlasedge.yml
+-rw-rw-rw-  2.0 fat      140 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_dl.yml
+-rw-rw-rw-  2.0 fat      733 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_docker_images.yml
+-rw-rw-rw-  2.0 fat     1343 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_ha.yml
+-rw-rw-rw-  2.0 fat      670 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_ief.yml
+-rw-rw-rw-  2.0 fat     2777 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_ief_a500.yml
+-rw-rw-rw-  2.0 fat     1665 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/task_ief_a500pro.yml
+-rw-rw-rw-  2.0 fat      477 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/install_nnae.yml
+-rw-rw-rw-  2.0 fat      477 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/install_nnrt.yml
+-rw-rw-rw-  2.0 fat      501 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
+-rw-rw-rw-  2.0 fat      495 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/install_toolkit.yml
+-rw-rw-rw-  2.0 fat      470 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
+-rw-rw-rw-  2.0 fat      470 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
+-rw-rw-rw-  2.0 fat      494 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
+-rw-rw-rw-  2.0 fat      488 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
+-rw-rw-rw-  2.0 fat      135 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_check.yml
+-rw-rw-rw-  2.0 fat     3004 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_install.yml
+-rw-rw-rw-  2.0 fat      647 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_patch.yml
+-rw-rw-rw-  2.0 fat      651 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_patch_rollback.yml
+-rw-rw-rw-  2.0 fat     1401 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_scene.yml
+-rw-rw-rw-  2.0 fat      265 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/process/process_test.yml
+-rw-rw-rw-  2.0 fat       67 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/README.md
+-rw-rw-rw-  2.0 fat      171 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
+-rw-rw-rw-  2.0 fat      347 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
+-rw-rw-rw-  2.0 fat      422 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
+-rw-rw-rw-  2.0 fat     1217 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_nerdctl.yml
+-rw-rw-rw-  2.0 fat     1382 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
+-rw-rw-rw-  2.0 fat     1160 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
+-rw-rw-rw-  2.0 fat       55 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
+-rw-rw-rw-  2.0 fat       37 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
+-rw-rw-rw-  2.0 fat      116 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
+-rw-rw-rw-  2.0 fat      272 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
+-rw-rw-rw-  2.0 fat      979 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
+-rw-rw-rw-  2.0 fat      660 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
+-rw-rw-rw-  2.0 fat      536 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/README.md
+-rw-rw-rw-  2.0 fat      400 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
+-rw-rw-rw-  2.0 fat      929 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
+-rw-rw-rw-  2.0 fat      283 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
+-rw-rw-rw-  2.0 fat      179 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
+-rw-rw-rw-  2.0 fat     1119 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
+-rw-rw-rw-  2.0 fat      882 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
+-rw-rw-rw-  2.0 fat     1309 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
+-rw-rw-rw-  2.0 fat     1119 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
+-rw-rw-rw-  2.0 fat     1032 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
+-rw-rw-rw-  2.0 fat     4329 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
+-rw-rw-rw-  2.0 fat     2002 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
+-rw-rw-rw-  2.0 fat     4102 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
+-rw-rw-rw-  2.0 fat     1856 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
+-rw-rw-rw-  2.0 fat      860 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
+-rw-rw-rw-  2.0 fat   202740 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
+-rw-rw-rw-  2.0 fat   237804 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.25.0.ipv6.yaml
+-rw-rw-rw-  2.0 fat       55 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
+-rw-rw-rw-  2.0 fat       37 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
+-rw-rw-rw-  2.0 fat      116 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
+-rw-rw-rw-  2.0 fat      539 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
+-rw-rw-rw-  2.0 fat       78 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
+-rw-rw-rw-  2.0 fat      243 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
+-rw-rw-rw-  2.0 fat      162 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
+-rw-rw-rw-  2.0 fat     1896 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
+-rw-rw-rw-  2.0 fat     8715 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
+-rw-rw-rw-  2.0 fat    10576 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
+-rw-rw-rw-  2.0 fat     1877 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
+-rw-rw-rw-  2.0 fat     2443 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
+-rw-rw-rw-  2.0 fat     1355 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
+-rw-rw-rw-  2.0 fat      176 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
+-rw-rw-rw-  2.0 fat     4530 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
+-rw-rw-rw-  2.0 fat      389 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
+-rw-rw-rw-  2.0 fat      390 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
+-rw-rw-rw-  2.0 fat      960 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_auto.yml
+-rw-rw-rw-  2.0 fat     1303 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_dl.yml
+-rw-rw-rw-  2.0 fat      259 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_edge.yml
+-rw-rw-rw-  2.0 fat      306 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_mef.yml
+-rw-rw-rw-  2.0 fat      514 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_mindspore.yml
+-rw-rw-rw-  2.0 fat      435 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_offline_dev.yml
+-rw-rw-rw-  2.0 fat      354 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_offline_run.yml
+-rw-rw-rw-  2.0 fat      510 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
+-rw-rw-rw-  2.0 fat      504 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
+-rw-rw-rw-  2.0 fat      593 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
+-rw-rw-rw-  2.0 fat      587 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
+-rw-rw-rw-  2.0 fat      273 b- defN 24-Mar-27 11:28 ascend_deployer/playbooks/scene/scene_vmhost.yml
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/Huawei_Integrity_Root_CA_G2.pem
+-rw-rw-rw-  2.0 fat     1902 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/Huawei_Software_Integriry_Protection_Root_CA.pem
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/__init__.py
+-rw-rw-rw-  2.0 fat     4096 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/create_report.py
+-rw-rw-rw-  2.0 fat    11154 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/eula_cn.txt
+-rw-rw-rw-  2.0 fat    12908 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/eula_en.txt
+-rw-rw-rw-  2.0 fat     1104 b- defN 24-Apr-26 09:50 ascend_deployer/scripts/image_load.sh
+-rw-rw-rw-  2.0 fat     8938 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/k8s_rep.py
+-rw-rw-rw-  2.0 fat    15500 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/nexus.py
+-rw-rw-rw-  2.0 fat     1350 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/nexus_config.json
+-rw-rw-rw-  2.0 fat     8712 b- defN 24-Mar-27 11:28 ascend_deployer/scripts/pkg_utils.py
+-rw-rw-rw-  2.0 fat      535 b- defN 24-Apr-26 09:50 ascend_deployer/scripts/uninstall_k8s_docker.sh
+-rw-rw-rw-  2.0 fat      643 b- defN 24-Apr-26 09:50 ascend_deployer/scripts/uninstall_mef_kubeedge.sh
+-rw-rw-rw-  2.0 fat      679 b- defN 24-Apr-26 09:50 ascend_deployer/scripts/uninstall_mef_related.sh
+-rw-rw-rw-  2.0 fat     1259 b- defN 24-Mar-27 11:28 ascend_deployer/templates/mindio/drc.conf
+-rw-rw-rw-  2.0 fat     1038 b- defN 24-Mar-27 11:28 ascend_deployer/templates/mindio/memfs.conf
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Mar-27 11:28 ascend_deployer/templates/mindio/ockiod.conf
+-rw-rw-rw-  2.0 fat     9719 b- defN 24-Mar-27 11:28 ascend_deployer/tools/hccn.py
+-rw-rw-rw-  2.0 fat     2373 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/README.rst
+-rw-rw-rw-  2.0 fat      314 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/image/dockerfile
+-rw-rw-rw-  2.0 fat      665 b- defN 24-Apr-26 09:50 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/driver-install.sh
+-rw-rw-rw-  2.0 fat     1658 b- defN 24-Apr-26 09:50 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/exec.sh
+-rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-arm-installer.yaml
+-rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-x86-installer.yaml
+-rw-rw-rw-  2.0 fat      703 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-arm-installer.yaml
+-rw-rw-rw-  2.0 fat      703 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-x86-installer.yaml
+-rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-arm-installer.yaml
+-rw-rw-rw-  2.0 fat      697 b- defN 24-Mar-27 11:28 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-x86-installer.yaml
+-rw-rw-rw-  2.0 fat     4260 b- defN 24-Mar-27 11:28 ascend_deployer/tools/nexus/Dockerfile
+-rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-27 11:28 ascend_deployer/yamls/image_load.yaml
+-rw-rw-rw-  2.0 fat      351 b- defN 24-Mar-27 11:28 ascend_deployer/yamls/k8s_reset.yaml
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2876 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/NOTICE
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      129 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       16 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    48712 b- defN 24-Apr-26 09:50 ascend_deployer-6.0.0b1.dist-info/RECORD
+419 files, 2436306 bytes uncompressed, 477240 bytes compressed:  80.4%
```

## zipnote {}

```diff
@@ -33,20 +33,32 @@
 
 Filename: ascend_deployer/version.json
 Comment: 
 
 Filename: ascend_deployer/ansible_plugin/ansible_log.py
 Comment: 
 
+Filename: ascend_deployer/ansible_plugin/deploy_info_output_plugin.py
+Comment: 
+
 Filename: ascend_deployer/ansible_plugin/install_info.yaml
 Comment: 
 
+Filename: ascend_deployer/ansible_plugin/progress_config.json
+Comment: 
+
+Filename: ascend_deployer/ansible_plugin/standard.py
+Comment: 
+
 Filename: ascend_deployer/downloader/__init__.py
 Comment: 
 
+Filename: ascend_deployer/downloader/ansible_reqs.json
+Comment: 
+
 Filename: ascend_deployer/downloader/config.ini
 Comment: 
 
 Filename: ascend_deployer/downloader/deb_downloader.py
 Comment: 
 
 Filename: ascend_deployer/downloader/dl_mef_dependency_downloader.py
@@ -111,23 +123,14 @@
 
 Filename: ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/installed.txt
-Comment: 
-
-Filename: ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/source.repo
-Comment: 
-
 Filename: ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
@@ -258,14 +261,23 @@
 
 Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
 Comment: 
 
+Filename: ascend_deployer/downloader/config/UOS_20-1050e_aarch64/installed.txt
+Comment: 
+
+Filename: ascend_deployer/downloader/config/UOS_20-1050e_aarch64/pkg_info.json
+Comment: 
+
+Filename: ascend_deployer/downloader/config/UOS_20-1050e_aarch64/source.repo
+Comment: 
+
 Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
 Comment: 
 
 Filename: ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
@@ -294,197 +306,272 @@
 
 Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/UOS_20-1050e_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/DL/aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.0/DL/x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
 Comment: 
 
 Filename: ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json
 Comment: 
 
 Filename: ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json
 Comment: 
 
 Filename: ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json
 Comment: 
 
 Filename: ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_x86_64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json
+Filename: ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_aarch64.json
 Comment: 
 
-Filename: ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json
+Filename: ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_x86_64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_aarch64.json
+Comment: 
+
+Filename: ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_x86_64.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.0.1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.0.RC1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.3.RC1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.3.RC2.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/CANN_7.0.0.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/CANN_7.0.RC1.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/DL_5.0.0.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/DL_5.0.RC1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/DL_5.0.RC2.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/DL_5.0.RC3.json
@@ -507,26 +594,32 @@
 
 Filename: ascend_deployer/downloader/software/MindSpore_2.1.0.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindSpore_2.2.0.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/MindSpore_2.2.10.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/MindStudio_5.0.0.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_6.0.RC2.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/NPU_23.0.0.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/NPU_23.0.RC1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/NPU_23.0.RC2.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/NPU_23.0.RC3.json
@@ -549,156 +642,180 @@
 
 Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0.post1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0.post8.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/Torch-npu_1.8.1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/Torch-npu_1.8.1.post2.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/Torch-npu_2.0.1.post1.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/Torch-npu_2.1.0.json
+Comment: 
+
 Filename: ascend_deployer/downloader/yum_metadata/__init__.py
 Comment: 
 
 Filename: ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
 Comment: 
 
 Filename: ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
 Comment: 
 
 Filename: ascend_deployer/group_vars/all.yaml
 Comment: 
 
-Filename: ascend_deployer/patch/selenium_firefox.patch
+Filename: ascend_deployer/library/check_compatibility.py
 Comment: 
 
-Filename: ascend_deployer/patch/selenium_firefox_profile.patch
+Filename: ascend_deployer/library/check_nexus_status.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/basic.yaml
+Filename: ascend_deployer/library/check_status.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/check.yaml
+Filename: ascend_deployer/library/collect_info.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/check_mef.yaml
+Filename: ascend_deployer/library/create_user.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/check_pkgs.yml
+Filename: ascend_deployer/library/install_ascend_operator.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/clean_nexus.yml
+Filename: ascend_deployer/library/install_cann.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/create_nexus.yml
+Filename: ascend_deployer/library/install_device_plugin.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/create_user.yml
+Filename: ascend_deployer/library/install_docker_runtime.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/distribution.yml
+Filename: ascend_deployer/library/install_hccl_controller.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/docker.yaml
+Filename: ascend_deployer/library/install_mindio.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/gather_app_info.yml
+Filename: ascend_deployer/library/install_noded.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/gather_facts.yaml
+Filename: ascend_deployer/library/install_npu_exporter.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/gather_npu_fact.yml
+Filename: ascend_deployer/library/install_python.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/harbor.yaml
+Filename: ascend_deployer/library/install_resilience_controller.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/hccn.yaml
+Filename: ascend_deployer/library/install_sys_pkg.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/image_load.yaml
+Filename: ascend_deployer/library/install_volcano.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/k8s.yaml
+Filename: ascend_deployer/library/login_harbor.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/kubeedge.yaml
+Filename: ascend_deployer/library/process_framework.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/mindxdl.yaml
+Filename: ascend_deployer/library/process_npu.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/modify_user_group.yml
+Filename: ascend_deployer/library/process_test.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/os_map.yaml
+Filename: ascend_deployer/library/push_image.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/os_map.yml
+Filename: ascend_deployer/library/scp.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
+Filename: ascend_deployer/library/system_report.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
+Filename: ascend_deployer/library/uncompress_resources.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_Kylin_V10Sword_aarch64.yml
+Filename: ascend_deployer/module_utils/__init__.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml
+Filename: ascend_deployer/module_utils/check_output_manager.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml
+Filename: ascend_deployer/module_utils/common_info.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
+Filename: ascend_deployer/module_utils/common_utils.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
+Filename: ascend_deployer/module_utils/compatibility_config.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/report.yaml
+Filename: ascend_deployer/module_utils/dl.py
 Comment: 
 
-Filename: ascend_deployer/playbooks/set_facts_cache_permission.yml
+Filename: ascend_deployer/playbooks/check.yaml
 Comment: 
 
-Filename: ascend_deployer/playbooks/sync_time.yml
+Filename: ascend_deployer/playbooks/distribution.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/task_set_custom_fact.yml
+Filename: ascend_deployer/playbooks/docker.yaml
 Comment: 
 
-Filename: ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+Filename: ascend_deployer/playbooks/gather_installation_facts.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/uninstall_mef_releate.yaml
+Filename: ascend_deployer/playbooks/gather_npu_fact.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/harbor.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/hccn.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/image_load.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/k8s.yaml
 Comment: 
 
-Filename: ascend_deployer/playbooks/callback_plugins/__init__.py
+Filename: ascend_deployer/playbooks/kubeedge.yaml
 Comment: 
 
-Filename: ascend_deployer/playbooks/callback_plugins/crop_columns.py
+Filename: ascend_deployer/playbooks/report.yaml
 Comment: 
 
-Filename: ascend_deployer/playbooks/facts/app_info.fact.j2
+Filename: ascend_deployer/playbooks/sync_time.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/facts/npu_info.fact.j2
+Filename: ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/uninstall_mef_releate.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_ascend-device-plugin.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml
 Comment: 
@@ -714,17 +831,14 @@
 
 Filename: ascend_deployer/playbooks/install/install_driver.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_firmware.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_gcc.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/install/install_ha.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_hccl-controller.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_ief.yml
@@ -783,104 +897,32 @@
 
 Filename: ascend_deployer/playbooks/install/install_volcano.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_atlasedge.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/task_cmake.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/install/task_dl.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_docker_images.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/task_driver.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_driver_common.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_firmware.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_gcc.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_get_npu_scene.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/install/task_ha.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_ief.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_ief_a500.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_ief_a500pro.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/task_kernel.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_kernel_euleros.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_kernels.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_mindspore.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_mpi.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_nnae.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_nnrt.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_protobuf.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_python.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_pytorch.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_sys_apt.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_sys_dnf.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_sys_pkg.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_sys_yum.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_tensorflow.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_tfplugin.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_toolbox.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/task_toolkit.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/install/patch/install_nnae.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/patch/install_nnrt.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/patch/install_tfplugin.yml
@@ -897,38 +939,14 @@
 
 Filename: ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/patch/task_nnae.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_nnrt.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_tfplugin.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/install/patch/task_toolkit.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/process/process_check.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/process/process_install.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/process/process_patch.yml
@@ -939,110 +957,14 @@
 
 Filename: ascend_deployer/playbooks/process/process_scene.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/process/process_test.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/check_driver.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/README.md
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/label_master.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/label_worker.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/mindio.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/templates/drc.conf
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/templates/memfs.conf
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.dl/templates/ockiod.conf
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.docker/README.md
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
@@ -1071,29 +993,14 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/README.md
@@ -1107,17 +1014,14 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
@@ -1191,41 +1095,14 @@
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
-Comment: 
-
-Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
-Comment: 
-
 Filename: ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
 Comment: 
 
 Filename: ascend_deployer/playbooks/scene/scene_auto.yml
@@ -1260,143 +1137,68 @@
 
 Filename: ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/scene/scene_vmhost.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/test/case_driver.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_firmware.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_mindspore.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_nnae.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_nnrt.yml
+Filename: ascend_deployer/scripts/Huawei_Integrity_Root_CA_G2.pem
 Comment: 
 
-Filename: ascend_deployer/playbooks/test/case_pytorch.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_tensorflow.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_tfplugin.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_toolbox.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/case_toolkit.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_all.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_driver.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_exhibit.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_firmware.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_mindspore.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_nnae.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_nnrt.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_pytorch.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_tensorflow.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_tfplugin.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_toolbox.yml
-Comment: 
-
-Filename: ascend_deployer/playbooks/test/test_toolkit.yml
+Filename: ascend_deployer/scripts/Huawei_Software_Integriry_Protection_Root_CA.pem
 Comment: 
 
 Filename: ascend_deployer/scripts/__init__.py
 Comment: 
 
-Filename: ascend_deployer/scripts/check_pkgs.sh
+Filename: ascend_deployer/scripts/create_report.py
 Comment: 
 
 Filename: ascend_deployer/scripts/eula_cn.txt
 Comment: 
 
 Filename: ascend_deployer/scripts/eula_en.txt
 Comment: 
 
-Filename: ascend_deployer/scripts/hccn_set.sh
-Comment: 
-
 Filename: ascend_deployer/scripts/image_load.sh
 Comment: 
 
-Filename: ascend_deployer/scripts/install.sh
-Comment: 
-
-Filename: ascend_deployer/scripts/install_ansible.sh
+Filename: ascend_deployer/scripts/k8s_rep.py
 Comment: 
 
 Filename: ascend_deployer/scripts/nexus.py
 Comment: 
 
 Filename: ascend_deployer/scripts/nexus_config.json
 Comment: 
 
-Filename: ascend_deployer/scripts/prepare.sh
+Filename: ascend_deployer/scripts/pkg_utils.py
 Comment: 
 
 Filename: ascend_deployer/scripts/uninstall_k8s_docker.sh
 Comment: 
 
 Filename: ascend_deployer/scripts/uninstall_mef_kubeedge.sh
 Comment: 
 
 Filename: ascend_deployer/scripts/uninstall_mef_related.sh
 Comment: 
 
-Filename: ascend_deployer/scripts/utils.sh
+Filename: ascend_deployer/templates/mindio/drc.conf
 Comment: 
 
-Filename: ascend_deployer/tools/DeviceIP-conf.sh
+Filename: ascend_deployer/templates/mindio/memfs.conf
 Comment: 
 
-Filename: ascend_deployer/tools/check.py
+Filename: ascend_deployer/templates/mindio/ockiod.conf
 Comment: 
 
 Filename: ascend_deployer/tools/hccn.py
 Comment: 
 
-Filename: ascend_deployer/tools/update_crl.sh
-Comment: 
-
-Filename: ascend_deployer/tools/hccn/main/go.mod
-Comment: 
-
-Filename: ascend_deployer/tools/hccn/main/hccn.go
-Comment: 
-
 Filename: ascend_deployer/tools/kubernetes/driver_installer/README.rst
 Comment: 
 
 Filename: ascend_deployer/tools/kubernetes/driver_installer/image/dockerfile
 Comment: 
 
 Filename: ascend_deployer/tools/kubernetes/driver_installer/install_scripts/driver-install.sh
@@ -1422,74 +1224,35 @@
 
 Filename: ascend_deployer/tools/kubernetes/driver_installer/yaml/910-x86-installer.yaml
 Comment: 
 
 Filename: ascend_deployer/tools/nexus/Dockerfile
 Comment: 
 
-Filename: ascend_deployer/tools/report/main/go.mod
-Comment: 
-
-Filename: ascend_deployer/tools/report/main/main.go
-Comment: 
-
-Filename: ascend_deployer/tools/unzip/main/go.mod
-Comment: 
-
-Filename: ascend_deployer/tools/unzip/main/unzip.go
-Comment: 
-
-Filename: ascend_deployer/yamls/basic.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/check.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/docker.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/gather_facts.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/harbor.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/hccn.yaml
-Comment: 
-
 Filename: ascend_deployer/yamls/image_load.yaml
 Comment: 
 
-Filename: ascend_deployer/yamls/k8s.yaml
-Comment: 
-
 Filename: ascend_deployer/yamls/k8s_reset.yaml
 Comment: 
 
-Filename: ascend_deployer/yamls/mindxdl.yaml
-Comment: 
-
-Filename: ascend_deployer/yamls/report.yaml
-Comment: 
-
-Filename: ascend_deployer-5.0.6.dist-info/LICENSE
+Filename: ascend_deployer-6.0.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/METADATA
+Filename: ascend_deployer-6.0.0b1.dist-info/METADATA
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/NOTICE
+Filename: ascend_deployer-6.0.0b1.dist-info/NOTICE
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/WHEEL
+Filename: ascend_deployer-6.0.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/entry_points.txt
+Filename: ascend_deployer-6.0.0b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/top_level.txt
+Filename: ascend_deployer-6.0.0b1.dist-info/top_level.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.6.dist-info/RECORD
+Filename: ascend_deployer-6.0.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ascend_deployer/ansible.cfg

```diff
@@ -1,21 +1,23 @@
 [defaults]
 forks=50
+pipelining=True
 command_warnings=False
 host_key_checking=False
-callback_plugins   = ./ansible_plugin
+callback_plugins=./ansible_plugin
 bin_ansible_callbacks=True
 log_path=./install.log
+library=./library
+module_utils=./module_utils
+stdout_callback=standard
 
 gathering=explicit
-fact_caching=jsonfile
 deprecation_warnings=False
 interpreter_python=auto_legacy_silent
-fact_caching_connection=./facts-cache
+fact_caching_connection=./facts_cache
 
 [inventory]
 unparsed_is_failed=True
 
 [ssh_connection]
 scp_if_ssh=True
-pipelining=True
-ssh_args = -o ControlMaster=auto -o ControlPersist=3600s
+ssh_args = -o ControlMaster=auto -o ControlPersist=3600s -o GSSAPIAuthentication=no
```

## ascend_deployer/ascend_deployer.py

```diff
@@ -19,40 +19,43 @@
 import argparse
 import logging
 import logging.config
 from functools import wraps
 
 import utils
 
-LOG = logging.getLogger('install')
+__cached__ = 'ignore'  # fix bug for site.py in ubuntu_18.04_aarch64
+
+LOG = logging.getLogger('ascend_deployer')
 LOG_OP = logging.getLogger('install_operation')
 
 
 def add_log(f):
     @wraps(f)
     def wrap(*args, **kwargs):
         cmd = ' '.join(sys.argv[1:])
         dl_scene = False
         if 'dl' in cmd:  # only for support XX ugly implementation
             dl_scene = True
         reason = ''
         try:
-            result = f(*args, **kwargs)
+            f(*args, **kwargs)
             if dl_scene:
                 LOG.info("[INFO] Ascend DL deployed success --ascend-deployer")
-            return result
+            return 0
         except SystemExit as e:
             if e.code == 0:
                 return 0
             reason = 'exit code: {}'.format(e.code)
             return -1
         except KeyboardInterrupt:  # handle KeyboardInterrupt
             reason = "User interrupted the program by Keyboard"
             return -1
         except BaseException as e:  # handle other exceptions
+            LOG.exception(e)
             reason = str(e)
             return -1
         finally:
             msg = "run cmd: {} successfully".format(cmd)
             if reason:
                 msg = "run cmd: {} failed, reason: {}".format(cmd, reason)
             print(msg)
@@ -109,58 +112,74 @@
         if args.install and args.scene:
             raise Exception("Unsupported --install and --install-scene at same time")
 
         if args.stdout_callback:
             os.environ['ANSIBLE_STDOUT_CALLBACK'] = args.stdout_callback
         os.environ['ANSIBLE_CACHE_PLUGIN_CONNECTION'] = os.path.join(utils.ROOT_PATH, 'facts_cache')
         os.environ['ANSIBLE_CONFIG'] = os.path.join(utils.ROOT_PATH, 'ansible.cfg')
+        os.environ['PYTHONWARNINGS'] = 'ignore::UserWarning'
 
         import jobs
         if any([args.install, args.scene, args.patch]) and not args.check:
             if not jobs.accept_eula():
                 LOG_OP.error('reject EULA, quit to install')
                 raise Exception('reject EULA, quit to install')
             LOG_OP.info("accept EULA, start to install")
-        jobs.prepare_install()
+        jobs.PrepareJob().run()
         ansible_args = ['-v'] if args.verbose else []
         if args.check:
             check_tags = args.install if args.install else []
             if args.scene:
                 check_tags.append(args.scene)
             return jobs.process_check(check_tags, no_copy=True, ansible_args=ansible_args)
         for handler, tags in (
                 (jobs.process_install, args.install),
                 (jobs.process_scene, args.scene),
                 (jobs.process_patch, args.patch),
                 (jobs.process_patch_rollback, args.patch_rollback)):
             if not tags:
                 continue
+            ip = jobs.get_localhost_ip()
+            job = jobs.ResourcePkg(tags)
+            nexus_url = job.start_nexus_daemon(ip)
+            if not args.no_copy:
+                job.handle_pkgs()
             envs = {
-                'hosts_name': 'worker',
+                'hosts_name': utils.get_hosts_name(tags),
                 'force_upgrade_npu': 'true' if args.force_upgrade_npu else 'false',
                 'do_upgrade': 'true',
+                'working_on_ipv6': 'true' if ':' in ip else 'false',
+                'use_k8s_version': os.environ.get('USE_K8S_VERSION', '1.25.3')
             }
-            return handler(tags, no_copy=args.no_copy, envs=envs, ansible_args=ansible_args)
+            if nexus_url:
+                envs['nexus_url'] = nexus_url
+            result = handler(tags, no_copy=args.no_copy, envs=envs, ansible_args=ansible_args)
+            job.clean(ip)
+            return result
         if args.test:
             envs = {'hosts_name': 'worker'}
+            if '-v' not in ansible_args:    # test always detail output
+                ansible_args.append('-v')
             return jobs.process_test(args.test, envs=envs, ansible_args=ansible_args)
         if args.clean:
-            run_args = ['worker', '-m', 'shell', '-a', 'rm -rf ~/resources.tar ~/resources']
+            run_args = ['worker', '-m', 'shell', '-a', 'rm -rf ~/resources*.tar ~/resources']
             run_args.extend(ansible_args)
             return jobs.process_clean(run_args)
         if args.ls:
             envs = {'only_package': 'true'}
+            if '-v' not in ansible_args:    # ls always detail output
+                ansible_args.append('-v')
             return jobs.process_ls(None, envs=envs, ansible_args=ansible_args)
         if args.hccn:
             return jobs.process_hccn(None, ansible_args=ansible_args)
 
 
 def main():
+    os.umask(0o022)
     logging.config.dictConfig(utils.LOGGING_CONFIG)
-    utils.update_permissions()
     cli = CLI(
         "ascend-deployer",
         "Manage Ascend Packages and dependence packages for specified OS"
     )
     return cli.run()
```

## ascend_deployer/install.sh

```diff
@@ -1,29 +1,17 @@
 #!/bin/bash
 readonly BASE_DIR=$(
     cd "$(dirname $0)" >/dev/null 2>&1
     pwd -P
 )
 
-function get_specified_python() {
-    if [ ! -z ${ASCEND_PYTHON_VERSION} ]; then
-        echo ${ASCEND_PYTHON_VERSION}
-    else
-        echo $(grep -oP "^ascend_python_version=\K.*" ${BASE_DIR}/downloader/config.ini | sed 's/\r$//')
-    fi
-}
-
-readonly specified_python=$(get_specified_python)
-readonly PYTHON_VERSION=$(echo ${specified_python} | sed 's/P/p/;s/-//')
-readonly PYTHON_PREFIX=${HOME}/.local/${PYTHON_VERSION}
-export PATH=${PYTHON_PREFIX}/bin:$PATH
-export LD_LIBRARY_PATH=${PYTHON_PREFIX}/lib:$LD_LIBRARY_PATH
-
-
 main() {
+    if [[ -f ~/.local/ascend_deployer_rc ]]; then
+      source ~/.local/ascend_deployer_rc
+    fi
     python3 -V > /dev/null 2>&1
     if [[ $? != 0 ]]; then
       python ${BASE_DIR}/ascend_deployer.py $*
     else
       python3 ${BASE_DIR}/ascend_deployer.py $*
     fi
 }
```

## ascend_deployer/inventory_file

```diff
@@ -8,20 +8,21 @@
 dscp_tc=""
 common_network="0.0.0.0/0"
 
 [master]
 #10.10.10.10 ansible_ssh_user="root" ansible_ssh_pass="test1234" k8s_api_server_ip=10.10.10.10
 
 [worker]
-localhost ansible_connection='local'
+localhost ansible_connection='local' ansible_ssh_user='root'
 
 [other_build_image]
 
 [all:vars]
 POD_NETWORK_CIDR="192.168.0.0/16"
 KUBE_SERVICE_CIDR="10.96.0.0/12"
 KUBE_VIP=""
 HARBOR_SERVER=""
 HARBOR_ADMIN_USER=""
 HARBOR_ADMIN_PASSWORD=""
 HARBOR_PUBLIC_PROJECT="false"
-HARBOR_CA_FILE=""
+HARBOR_CA_FILE=""
+RUNNER_IP=""
```

## ascend_deployer/jobs.py

```diff
@@ -11,58 +11,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import os
+import atexit
+import codecs
+import shutil
 import sys
+import glob
+import json
+import getpass
 import platform
-from subprocess import PIPE, Popen, CalledProcessError, STDOUT
+import logging
+import importlib
+import subprocess
+import tempfile
+import tarfile
+from threading import Thread
+from zipfile import ZipFile, BadZipfile
 
 import utils
+from module_utils.common_info import get_os_and_arch
+from scripts.pkg_utils import filter_pkg, search_paths, get_run_dir, get_config_dir, need_nexus
+from scripts import nexus
 
-CURSOR_UPWARD = u'\u001b[1A'
-MAX_LEN = 80
-
-
-def process_run_cmd_and_check(*popenargs, **kwargs):
-    process = Popen(*popenargs, **kwargs)
-    process.communicate()
-    ret_code = process.returncode
-    if ret_code:
-        cmd = kwargs.get("args")
-        if cmd is None:
-            cmd = popenargs[0]
-        raise CalledProcessError(ret_code, cmd)
-    return 0
-
-
-def prepare_install():
-    prepare_sh = os.path.join(utils.ROOT_PATH, 'scripts', 'prepare.sh')
-    process = Popen(["bash", prepare_sh], shell=False, env=os.environ, stderr=STDOUT, stdout=PIPE)
-
-    sys.stdout.write("\n")  # prevents the first line from being overwritten
-    for line in iter(process.stdout.readline, b''):
-        line = line.decode('utf-8').strip()
-        if line.startswith('[ERROR]'):
-            pass
-        elif len(line) <= MAX_LEN:
-            line += (MAX_LEN - len(line)) * " "
-        else:
-            # if the line too long(> MAX_LEN), only print first (MAX_LEN -3) characters and '...'
-            line = line[0:MAX_LEN - 4] + "..."
-        sys.stdout.write(CURSOR_UPWARD)
-        sys.stdout.write("\r" + line + "\n")
-
-    process.wait()
-    ret_code = process.returncode
-    if ret_code:
-        raise CalledProcessError(ret_code, ["ascend_deployer/scripts/prepare.sh"])
-    return 0
+LOG = logging.getLogger("ascend_deployer.jobs")
 
 
 def prompt(tip):
     sys.stdout.write(tip)
     sys.stdout.flush()
     if platform.system() == 'Windows':
         import msvcrt
@@ -90,20 +68,87 @@
 
 
 def accept_eula():
     eula_file = 'eula_en.txt'
     if 'zh_CN' in os.environ.get('LANG', ''):
         eula_file = 'eula_cn.txt'
     eula_file_path = os.path.join(utils.ROOT_PATH, 'scripts', eula_file)
-    with open(eula_file_path, 'rb') as f:
-        print(f.read().decode('utf-8'))
+    with codecs.open(eula_file_path, encoding='utf-8') as f:
+        content = f.read()
+        print(content if isinstance(content, str) else codecs.encode(content, 'utf-8'))
     answer = prompt("Do you accept the EULA to use Ascend-deployer?[y/N]")
     return len(answer) == 1 and answer.lower() == 'y'
 
 
+def start_nexus(ip, port):
+    if os.path.exists(utils.NEXUS_SENTINEL_FILE):
+        os.unlink(utils.NEXUS_SENTINEL_FILE)
+        LOG.info('unlink existed sentinel file: {}'.format(utils.NEXUS_SENTINEL_FILE))
+    try:
+        nexus.main(ip, port)
+        LOG.info('start nexus({}:{}) successfully'.format(ip, port))
+        dir_path = os.path.dirname(utils.NEXUS_SENTINEL_FILE)
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path, 0o700)
+        with open(utils.NEXUS_SENTINEL_FILE, 'w'):
+            pass
+        LOG.info('set sentinel file: {}'.format(utils.NEXUS_SENTINEL_FILE))
+    except Exception as e:
+        LOG.error('start nexus failed: {}'.format(e))
+
+
+def get_localhost_ip():
+    host_file = os.path.join(utils.ROOT_PATH, 'inventory_file')
+    host_lines = []
+    with open(host_file) as f:
+        host_lines = f.readlines()
+
+    for line in host_lines:
+        if line.startswith("RUNNER_IP="):
+            host_ip = line.replace("RUNNER_IP=", '').replace('"', '').strip()
+            if host_ip:
+                return host_ip
+
+    ssh_connection_info = os.environ.get("SSH_CONNECTION", '').split()
+    if len(ssh_connection_info) > 2:
+        return ssh_connection_info[2]
+
+    first_ip = ''
+    for line in host_lines:
+        line = line.strip()
+        if line.startswith('#') or 'ansible_' not in line:
+            continue
+        host = line.split()[0]
+        if host != 'localhost':
+            first_ip = host
+            break
+    if not first_ip:
+        return '127.0.0.1'
+    if ':' in first_ip:
+        net_prefix = first_ip.split(':')[0]
+        ver = '-6'
+    else:
+        net_prefix = first_ip.split('.')[0]
+        ver = '-4'
+    lines = utils.run_cmd('ip {} address'.format(ver), stdout=subprocess.PIPE)
+    for line in lines:
+        line = line.strip()
+        if 'inet' not in line or ' ' not in line:
+            continue
+        ip = line.split()[1].split('/')[0]
+        if ip.startswith(net_prefix):
+            return ip
+    return '127.0.0.1'
+
+
+def get_nexus_url(ip, port):
+    host = '[{}]'.format(ip) if ':' in ip else ip
+    return 'http://{}:{}'.format(host, port)
+
+
 class AnsibleJob(object):
     def __init__(self, yaml_file):
         self.yaml_file = yaml_file
 
     @staticmethod
     def get_inventory_file():
         return os.path.join(utils.ROOT_PATH, 'inventory_file')
@@ -126,19 +171,19 @@
             raise Exception("ASCEND_PYTHON_VERSION is not available, "
                             "available python version list is {}".format(version_list))
         version = ascend_python_version.replace('P', 'p').replace('-', '')
         args.extend([
             '-e', 'python_tar={}'.format(ascend_python_version),
             '-e', 'python_version={}'.format(version),
         ])
-        install_path = os.path.expanduser('~/.local/{}'.format(version))
-        os.environ['PATH'] = '{}/bin:{}'.format(install_path, os.environ.get('PATH', ''))
-        os.environ['LD_LIBRARY_PATH'] = '{}/lib:{}'.format(install_path, os.environ.get('LD_LIBRARY_PATH', ''))
 
     def run_playbook(self, tags, no_copy=False, envs=None, ansible_args=None):
+        facts_path = os.path.join(utils.ROOT_PATH, 'facts_cache')
+        if os.path.exists(facts_path):
+            shutil.rmtree(facts_path)
         args = self.build_args(envs)
         skip_tags = []
         if tags:
             if not isinstance(tags, list):
                 tags = [tags]
             if 'all' in tags:
                 tags[tags.index('all')] = 'whole'  # all is ansible reserved tag
@@ -147,15 +192,15 @@
             else:
                 tags.append('copy')
             args.extend(['--tags', ','.join(tags)])
             if skip_tags:
                 args.extend(['--skip-tags', ','.join(skip_tags)])
         if ansible_args:
             args.extend(ansible_args)
-        return process_run_cmd_and_check(args, shell=False, env=os.environ)
+        return utils.run_cmd(args)
 
     def build_args(self, envs):
         inventory_file = self.get_inventory_file()
         args = ['ansible-playbook', '-i', inventory_file, self.yaml_file]
         if not envs:
             envs = {}
         self.handle_python_env(args)
@@ -163,20 +208,383 @@
             args.extend(['-e', '{}={}'.format(k, v)])
         return args
 
     def run_ansible(self, run_args):
         inventory_file = self.get_inventory_file()
         args = ['ansible', '-i', inventory_file]
         args.extend(run_args)
-        return process_run_cmd_and_check(args, shell=False, env=os.environ)
+        return utils.run_cmd(args)
 
 
 process_path = os.path.join(utils.ROOT_PATH, 'playbooks', 'process')
 process_install = AnsibleJob(os.path.join(process_path, 'process_install.yml')).run_playbook
 process_scene = AnsibleJob(os.path.join(process_path, 'process_scene.yml')).run_playbook
 process_patch = AnsibleJob(os.path.join(process_path, 'process_patch.yml')).run_playbook
 process_patch_rollback = AnsibleJob(os.path.join(process_path, 'process_patch_rollback.yml')).run_playbook
 process_test = AnsibleJob(os.path.join(process_path, 'process_test.yml')).run_playbook
 process_check = AnsibleJob(os.path.join(process_path, 'process_check.yml')).run_playbook
 process_clean = AnsibleJob(None).run_ansible
 process_ls = AnsibleJob(os.path.join(utils.ROOT_PATH, 'playbooks', 'report.yaml')).run_playbook
 process_hccn = AnsibleJob(os.path.join(utils.ROOT_PATH, 'playbooks', 'hccn.yaml')).run_playbook
+
+
+class PrepareJob(object):
+    def __init__(self):
+        self.pip_path = os.path.join(utils.ROOT_PATH, 'resources', 'pylibs', 'pip*.whl')
+        self.cache_dir = os.path.join(utils.ROOT_PATH, 'resources', 'pylibs')
+        self.rc_file = os.path.expanduser('~/.local/ascend_deployer_rc')
+        self.os_ver_arch = get_os_and_arch()
+
+    def pip_install(self, pkg):
+        cmd_args = [sys.executable]
+        cmd_args.extend(['-m', 'pip', 'install', '-U', pkg])
+        cmd_args.extend(['--no-index', '--find-links', self.cache_dir])
+        return utils.run_cmd(cmd_args, oneline=True)
+
+    def update_env_file(self):
+        bin_path = os.path.dirname(sys.executable)
+        lib_path = os.path.dirname(os.path.dirname(os.__file__))
+        lines = [
+            "export ANSIBLE_CONFIG={}\n".format(os.path.join(utils.ROOT_PATH, 'ansible.cfg')),
+            "export PYTHONWARNINGS=ignore::UserWarning\n",
+            "export PATH={}:~/.local/bin:$PATH\n".format(bin_path),
+            "export LD_LIBRARY_PATH={}:~/.local/lib:$LD_LIBRARY_PATH\n".format(lib_path)
+        ]
+        rc_dir = os.path.dirname(self.rc_file)
+        if not os.path.exists(rc_dir):
+            os.makedirs(rc_dir, mode=0o750)
+        with open(self.rc_file, 'w') as f:
+            f.writelines(lines)
+
+    @staticmethod
+    def find_first(pattern):
+        files = glob.glob(pattern)
+        if not files:
+            raise Exception("no {} found, forget to download firstly?".format(pattern))
+        return files[0]
+
+    def install_distutils(self):
+        try:
+            importlib.import_module('distutils.util')
+        except ImportError:  # exist on Ubuntu 18.04
+            pkg_path = os.path.join(utils.ROOT_PATH, 'resources', self.os_ver_arch, 'python*-distutils*')
+            cmd = 'dpkg --force-all -i {}'.format(self.find_first(pkg_path))
+            utils.run_cmd(cmd, oneline=True)
+
+    def install_pip(self):
+        need_install = False
+        try:
+            pip = importlib.import_module('pip')
+        except ImportError:
+            need_install = True
+        else:
+            major_version = int(getattr(pip, '__version__', '9.0.0').split('.')[0])
+            if major_version < 20:
+                need_install = True
+        if not need_install:
+            return
+        pip_file = self.find_first(self.pip_path)
+        install_pip_cmd_args = [sys.executable, '{}/pip'.format(pip_file), 'install', '-U', pip_file]
+        utils.run_cmd(install_pip_cmd_args, oneline=True)
+
+    def install_ansible(self):
+        try:
+            import ansible
+            return
+        except ImportError:
+            self.pip_install('setuptools')
+            self.pip_install('cryptography')
+            self.pip_install('ansible-core')
+            self.update_env_file()
+        site = importlib.import_module('site')
+        try:
+            reload(site)
+        except NameError:
+            importlib.reload(site)
+
+    def ensure_docker_daemon_exist(self):
+        docker_daemon = "/etc/docker/daemon.json"
+        if os.path.exists(docker_daemon):
+            return
+        content_dict = dict()
+        from distutils.spawn import find_executable
+        if not find_executable('rpm'):
+            content_dict.update({
+                "exec-opts": ["native.cgroupdriver=systemd"],
+                "live-restore": True
+            })
+        elif self.os_ver_arch.startswith('OpenEuler'):
+            content_dict.update({
+                "live-restore": True
+            })
+        docker_config_path = os.path.dirname(docker_daemon)
+        if not os.path.exists(docker_config_path):
+            os.makedirs(docker_config_path, mode=0o750)
+        with open(docker_daemon, 'w') as f:
+            json.dump(content_dict, f, indent=4)
+
+    def install_docker(self):
+        utils.install_pkg('docker', self.os_ver_arch, 'docker', '*')
+        if getpass.getuser() == 'root':
+            self.ensure_docker_daemon_exist()
+            utils.run_cmd("systemctl enable docker")
+            utils.run_cmd("systemctl daemon-reload")
+            utils.run_cmd("systemctl restart docker")
+
+    def install_selinux(self):
+        if not self.os_ver_arch.startswith(('CentOS', 'OpenEuler', 'Kylin')):
+            return
+        try:
+            importlib.import_module('selinux')
+        except ImportError:
+            utils.install_pkg('selinux', self.os_ver_arch, 'libselinux*')
+
+    def install_openssl(self):
+        if self.os_ver_arch.startswith('CentOS'):
+            utils.install_pkg('openssl11', self.os_ver_arch, 'openssl*')
+
+    def install_haveged(self):
+        if utils.install_pkg('haveged', self.os_ver_arch, '*havege*') is not None:
+            utils.run_cmd('systemctl enable haveged')
+            utils.run_cmd('systemctl restart haveged')
+
+    def install_basic_dependencies(self):
+        utils.install_pkg('bzip2', self.os_ver_arch, 'bzip2*')
+        utils.install_pkg('unzip', self.os_ver_arch, 'unzip*')
+        utils.install_pkg('tar', self.os_ver_arch, 'tar*')
+        utils.install_pkg('sshpass', self.os_ver_arch, 'sshpass*')
+        self.install_haveged()
+        self.install_docker()
+        self.install_selinux()
+        self.install_openssl()
+
+    def run(self):
+        self.install_distutils()
+        self.install_pip()
+        self.install_ansible()
+        self.install_basic_dependencies()
+
+
+class TempDir(object):
+    def __init__(self, **kwargs):
+        dir_path = kwargs.get('dir')
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path, 0o700)
+        self.name = tempfile.mkdtemp(**kwargs)
+
+    def __enter__(self):
+        return self.name
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        shutil.rmtree(self.name)
+
+
+class ResourcePkg(object):
+    def __init__(self, tags=None):
+        self.tags = []
+        if tags:
+            self.tags = [tags] if isinstance(tags, str) else tags
+        self.resource_path = os.path.join(utils.ROOT_PATH, 'resources')
+        self.root_ca = os.path.join(utils.ROOT_PATH, 'scripts', 'Huawei_Software_Integriry_Protection_Root_CA.pem')
+        self.root_ca_g2 = os.path.join(utils.ROOT_PATH, 'scripts', 'Huawei_Integrity_Root_CA_G2.pem')
+        self.tmp_dir = os.path.expanduser('~/.tmp')
+        if getpass.getuser() == 'root':
+            self.ascend_cert = '/usr/local/Ascend/toolbox/latest/Ascend-DMI/bin/ascend-cert'
+            self.sys_crl_file = '/etc/hwsipcrl/ascendsip.crl'
+            self.sys_g2_crl_file = '/etc/hwsipcrl/ascendsip_g2.crl'
+        else:
+            self.ascend_cert = os.path.expanduser('~/Ascend/toolbox/latest/Ascend-DMI/bin/ascend-cert')
+            self.sys_crl_file = os.path.expanduser('~/.local/hwsipcrl/ascendsip.crl')
+            self.sys_g2_crl_file = os.path.expanduser('~/.local/hwsipcrl/ascendsip_g2.crl')
+        self.arches = set()
+
+    def handle_run_pkg(self, file):
+        run_dir = get_run_dir(self.resource_path, file)
+        config_dir, config_source_dir = get_config_dir(self.resource_path, file)
+        if config_dir:
+            shutil.copytree(config_source_dir, config_dir)
+        if run_dir:
+            if not os.path.exists(run_dir):
+                os.makedirs(run_dir, 0o750)
+            shutil.copy(file, os.path.join(run_dir, os.path.basename(file)))
+
+    @staticmethod
+    def extract_zip(file, path):
+        filename = os.path.splitext(os.path.basename(file))[0]
+        try:
+            with ZipFile(file) as z:
+                members = z.namelist()
+                if any(p for p in z.namelist() if p.endswith('.cms')):
+                    members = [p for p in z.namelist() if p.startswith(filename)]
+                z.extractall(path, members)
+                return members
+        except BadZipfile:
+            raise Exception('{} is corrupted'.format(file))
+
+    @staticmethod
+    def extract_tar(file, path):
+        try:
+            with tarfile.open(file) as f:
+                members = f.getmembers()
+                f.extractall(path, members)
+                return members
+        except tarfile.TarError:
+            raise Exception('{} is corrupted'.format(file))
+
+    def extract(self, file, path):
+        if not os.path.exists(path):
+            os.makedirs(path, 0o750)
+        if file.endswith('.zip'):
+            return self.extract_zip(file, path)
+        elif file.endswith('.tar.gz'):
+            return self.extract_tar(file, path)
+        else:
+            raise Exception('Unsupported to extract file: {}'.format(file))
+
+    @staticmethod
+    def update_crl(old_crl, new_crl):
+        dir_path = os.path.dirname(new_crl)
+        if not os.path.exists(dir_path):
+            LOG.info('create sys crl dir: {}'.format(dir_path))
+            os.makedirs(dir_path, 0o700)
+        LOG.info('create sys crl file: {}'.format(new_crl))
+        shutil.copy(old_crl, new_crl)
+
+    @staticmethod
+    def verify_crl(crl_file, ca_file):
+        x509 = importlib.import_module('cryptography.x509')
+        backends = importlib.import_module('cryptography.hazmat.backends')
+        crl = x509.load_der_x509_crl(open(crl_file, 'rb').read(), backends.default_backend())
+        ca = x509.load_pem_x509_certificate(open(ca_file, 'rb').read(), backends.default_backend())
+        if not crl.is_signature_valid(ca.public_key()):
+            raise Exception('invalid signature for crl: {}'.format(crl_file))
+        if crl.get_revoked_certificate_by_serial_number(ca.serial_number):
+            raise Exception('ca_file: {} is revoked'.format(ca_file))
+        return crl
+
+    @staticmethod
+    def clean(ip):
+        try:
+            if os.path.exists(utils.NEXUS_SENTINEL_FILE):
+                os.unlink(utils.NEXUS_SENTINEL_FILE)
+                LOG.info('clean sentinel file: {}'.format(utils.NEXUS_SENTINEL_FILE))
+            utils.run_cmd('docker rm -f nexus', stdout=subprocess.PIPE)
+            nexus_data_path = '/tmp/nexus-data'
+            if os.path.exists(nexus_data_path):
+                utils.run_cmd('umount {}'.format(nexus_data_path))
+                shutil.rmtree(nexus_data_path)
+            if ':' in ip:
+                utils.run_cmd('docker network rm ip6net_nexus', stdout=subprocess.PIPE)
+        except Exception as e:
+            LOG.warning('clean nexus meet issue: {}'.format(e))
+
+    def compare_crl(self, crl_file, sys_crl_file, ca_file):
+        zip_crl = self.verify_crl(crl_file, ca_file)
+        if os.path.exists(sys_crl_file):
+            sys_crl = self.verify_crl(sys_crl_file, ca_file)
+            return zip_crl.last_update > sys_crl.last_update
+        return True
+
+    def verify_cms(self, crl_file, sys_crl_file, ca_file, cms_file, data_file):
+        if self.compare_crl(crl_file, sys_crl_file, ca_file):
+            self.update_crl(crl_file, sys_crl_file)
+        from distutils.spawn import find_executable
+        openssl = find_executable('openssl11') or 'openssl'
+        cmd = '{} cms -verify --no_check_time -in {} -inform DER -CAfile {} -binary -content {}' \
+              ' -purpose any -out {}'.format(openssl, cms_file, ca_file, data_file, os.devnull)
+        utils.run_cmd(cmd, stderr=os.open(os.devnull, os.O_RDWR))
+
+    def verify_hmac(self, data_file):
+        cms_file = data_file + '.cms'
+        crl_file = data_file + '.crl'
+        for item in (cms_file, data_file, crl_file):
+            os.chmod(item, 0o600)
+        if os.path.exists(self.ascend_cert):
+            update_crl_cmd = '{} -u {}'.format(self.ascend_cert, crl_file)
+            utils.run_cmd(update_crl_cmd, stdout=os.open(os.devnull, os.O_RDWR), stderr=os.open(os.devnull, os.O_RDWR))
+            verify_cmd = '{} {} {} {}'.format(self.ascend_cert, cms_file, data_file, crl_file)
+            utils.run_cmd(verify_cmd, stdout=os.open(os.devnull, os.O_RDWR), stderr=os.open(os.devnull, os.O_RDWR))
+            return
+        try:
+            self.verify_cms(crl_file, self.sys_g2_crl_file, self.root_ca_g2, cms_file, data_file)
+        except Exception as e:
+            LOG.warning(e)
+            self.verify_cms(crl_file, self.sys_crl_file, self.root_ca, cms_file, data_file)
+
+    def handle_zip_pkg(self, file):
+        with TempDir(dir=self.tmp_dir) as tmp_path:
+            # first unzip
+            members = self.extract(file, tmp_path)
+            cms_files = [x for x in members if x.endswith('.cms')]
+            if not cms_files:
+                LOG.info('no .cms found, skip to handle {}'.format(file))
+                return
+
+            tmp_file = os.path.join(tmp_path, os.path.splitext(cms_files[0])[0])
+
+            # verify hmac
+            self.verify_hmac(tmp_file)
+
+            # second unzip
+            run_dir = get_run_dir(self.resource_path, tmp_file)
+            self.extract(tmp_file, run_dir)
+
+    def iter_files(self, suffix):
+        for root, dirs, files in os.walk(self.resource_path):
+            for file in files:
+                for keyword in ('x86_64', 'amd64'):
+                    if keyword in file:
+                        self.arches.add('x86_64')
+                if 'aarch64' in file:
+                    self.arches.add('aarch64')
+                src_file = os.path.join(root, file)
+                if src_file.endswith(suffix) and filter_pkg(src_file, self.tags):
+                    yield src_file
+
+    def extract_pkgs(self):
+        if os.path.exists(self.tmp_dir):
+            shutil.rmtree(self.tmp_dir)
+        for cache_dir in glob.glob(os.path.join(self.resource_path, 'run_from_*_zip')):
+            shutil.rmtree(cache_dir)
+        for src_file in self.iter_files('.run'):
+            self.handle_run_pkg(src_file)
+        for src_file in self.iter_files('.zip'):
+            self.handle_zip_pkg(src_file)
+
+    def iter_need_pack_files(self, arch):
+        exclude_arch = 'aarch64' if arch == 'x86_64' else 'x86_64'
+        for dir_path in search_paths(self.resource_path, self.tags):
+            if os.path.isfile(dir_path):
+                yield dir_path
+            for root, dirs, files in os.walk(dir_path):
+                for file in files:
+                    if exclude_arch not in file:
+                        yield os.path.join(root, file)
+
+    def pack(self, tar_file, arch):
+        with tarfile.open(tar_file, 'w') as tar:
+            for file in self.iter_need_pack_files(arch):
+                tar.add(file, arcname=file.replace(utils.ROOT_PATH, ''))
+
+    def pack_pkgs(self):
+        for arch in self.arches:
+            tar_file = os.path.join(os.path.expanduser('~/resources_{}.tar'.format(arch)))
+            if os.path.exists(tar_file):
+                os.unlink(tar_file)
+            self.pack(tar_file, arch)
+
+    def handle_pkgs(self):
+        print("Extracting and repacking packages...")
+        self.extract_pkgs()
+        self.pack_pkgs()
+
+    def start_nexus_daemon(self, ip, port=58081):
+        if not need_nexus(self.tags):
+            return
+
+        if getpass.getuser() != 'root':
+            LOG.warning('not support to start nexus for by non-root user, please switch to root user')
+            return
+        thread = Thread(target=start_nexus, args=(ip, port))
+        thread.daemon = True
+        thread.start()
+        return get_nexus_url(ip, port)
```

## ascend_deployer/utils.py

```diff
@@ -11,45 +11,52 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import os
-import re
 import json
+import shlex
 import stat
+import sys
 import argparse
 import getpass
 import logging
 import logging.handlers
 import platform
 import shutil
+from subprocess import PIPE, Popen
 
 ROOT_PATH = SRC_PATH = os.path.dirname(__file__)
+NEXUS_SENTINEL_FILE = os.path.expanduser('~/.local/nexus.sentinel')
 MODE_700 = stat.S_IRWXU
 MODE_600 = stat.S_IRUSR | stat.S_IWUSR
 MODE_400 = stat.S_IRUSR
 
-dir_list = ['downloader', 'playbooks', 'tools', 'ansible_plugin', 'group_vars', 'patch', 'scripts', 'yamls']
+LOG = logging.getLogger('ascend_deployer.utils')
+MAX_LEN = 120
+
+dir_list = ['downloader', 'playbooks', 'tools', 'ansible_plugin', 'group_vars', 'patch', 'scripts', 'yamls',
+            'library', 'module_utils', 'templates']
 file_list = ['install.sh', 'inventory_file', 'ansible.cfg',
              '__init__.py', 'ascend_deployer.py', 'jobs.py', 'utils.py',
              'version.json']
 
 
 def copy_scripts():
     """
     copy scripts from library to ASCEND_DEPLOY_HOME
     the default ASCEND_DEPLOYER_HOME is HOME
     """
     if SRC_PATH == ROOT_PATH:
         return
 
     if not os.path.exists(ROOT_PATH):
-        os.makedirs(ROOT_PATH, mode=0o750, exist_ok=True)
+        os.makedirs(ROOT_PATH, mode=0o750)
     for dir_name in dir_list:
         src = os.path.join(SRC_PATH, dir_name)
         dst = os.path.join(ROOT_PATH, dir_name)
         if os.path.exists(src) and not os.path.exists(dst):
             shutil.copytree(src, dst)
 
     for filename in file_list:
@@ -125,18 +132,21 @@
     for file_name in os.listdir(dir_path):
         if file_name.startswith(prefix) and file_name.endswith(suffix):
             item = file_name.replace(prefix, '').replace(suffix, '')
             items.append(item)
     return sorted(items)
 
 
+dl_items = ['ascend-device-plugin', 'ascend-docker-runtime', 'ascend-operator', 'hccl-controller', 'mindio', 'noded',
+            'npu-exporter', 'resilience-controller', 'volcano', 'dl']
 install_items = get_name_list(os.path.join(ROOT_PATH, "playbooks", "install"), 'install_', '.yml')
 scene_items = get_name_list(os.path.join(ROOT_PATH, "playbooks", "scene"), 'scene_', '.yml')
 patch_items = get_name_list(os.path.join(ROOT_PATH, "playbooks", "install", "patch"), "install_", ".yml")
-test_items = get_name_list(os.path.join(ROOT_PATH, "playbooks", "test"), "test_", ".yml")
+test_items = ['all', 'firmware', 'driver', 'nnrt', 'nnae', 'toolkit', 'toolbox', 'mindspore', 'pytorch',
+              'tensorflow', 'tfplugin']
 
 LOG_MAX_BACKUP_COUNT = 5
 LOG_MAX_SIZE = 20 * 1024 * 1024
 LOG_FILE = os.path.join(ROOT_PATH, 'install.log')
 LOG_OPERATION_FILE = os.path.join(ROOT_PATH, 'install_operation.log')
 
 
@@ -149,20 +159,20 @@
         record.host = self.host
         return True
 
 
 class RotatingFileHandler(logging.handlers.RotatingFileHandler):
     def doRollover(self):
         try:
-            os.chmod(self.baseFilename, mode=0o400)
-        except PermissionError:
-            os.chmod('{}.{}'.format(self.baseFilename, LOG_MAX_BACKUP_COUNT), mode=0o600)
+            os.chmod(self.baseFilename, 0o400)
+        except OSError:
+            os.chmod('{}.{}'.format(self.baseFilename, LOG_MAX_BACKUP_COUNT), 0o600)
         finally:
             logging.handlers.RotatingFileHandler.doRollover(self)
-            os.chmod(self.baseFilename, mode=0o600)
+            os.chmod(self.baseFilename, 0o600)
 
 
 LOGGING_CONFIG = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         'extra': {
@@ -173,72 +183,101 @@
     "filters": {
         "user_host": {
             '()': UserHostFilter
         }
     },
     "handlers": {
         "install": {
-            "level": "INFO",
+            "level": "DEBUG",
             "formatter": "extra",
             "class": 'utils.RotatingFileHandler',
             "filename": LOG_FILE,
             'maxBytes': LOG_MAX_SIZE,
             'backupCount': LOG_MAX_BACKUP_COUNT,
-            'encoding': "UTF-8"
+            'encoding': "UTF-8",
+            "filters": ["user_host"],
         },
         "install_operation": {
             "level": "INFO",
             "formatter": "extra",
             "class": 'utils.RotatingFileHandler',
             "filename": LOG_OPERATION_FILE,
             'maxBytes': LOG_MAX_SIZE,
             'backupCount': LOG_MAX_BACKUP_COUNT,
-            'encoding': "UTF-8"
+            'encoding': "UTF-8",
+            "filters": ["user_host"],
         },
     },
     "loggers": {
-        "install": {
+        "ascend_deployer": {
             "handlers": ["install"],
             "level": "INFO",
-            "propagate": False,
-            "filters": ["user_host"]
+            "propagate": True,
         },
         "install_operation": {
             "handlers": ["install_operation"],
             "level": "INFO",
-            "propagate": False,
-            "filters": ["user_host"]
+            "propagate": True,
         },
     }
 }
 
 
-def ignore_permission(dir_path, name):
-    return dir_path.endswith('__pycache__') or \
-        name.startswith(('__pycache__', '.git'))
-
-
-def update_folder_permission(dir_path, dir_name):
-    if ignore_permission(dir_path, dir_name):
-        return
-    os.chmod(os.path.join(dir_path, dir_name), MODE_700)
+def run_cmd(args, oneline=False, **kwargs):
+    if not kwargs.get('shell') and isinstance(args, str):
+        args = shlex.split(args, posix=platform.system() == 'Linux')
+    cmd = args if isinstance(args, str) else ' '.join(args)
+    LOG.info(cmd.center(MAX_LEN, '-'))
+    stdout = kwargs.pop('stdout', PIPE if oneline else None)
+    stderr = kwargs.pop('stderr', PIPE)
+    text = kwargs.pop('universal_newlines', True)
+    output = []
+    process = Popen(args, stdout=stdout, stderr=stderr, universal_newlines=text, **kwargs)
+    if oneline:
+        for line in iter(process.stdout.readline, ''):
+            line = line.strip()
+            output.append(line)
+            LOG.info(line)
+            if len(line) <= MAX_LEN:
+                line += (MAX_LEN - len(line)) * " "
+            else:
+                # if the line too long(> MAX_LEN), only print first (MAX_LEN -3) characters and '...'
+                line = line[0:MAX_LEN - 4] + "..."
+            sys.stdout.write("\r{}".format(line))
+        err = process.stderr.read()
+        process.wait()
+    else:
+        out, err = process.communicate()
+        if isinstance(out, str):
+            output = out.splitlines()
+            for line in output:
+                LOG.info(line)
+    if process.returncode:
+        err = err or "returned non-zero exit status {}".format(process.returncode)
+        raise Exception(err)
+    return output
 
 
-def update_file_permission(dir_path, file_name):
-    if ignore_permission(dir_path, file_name):
+def install_pkg(name, *paths):
+    from distutils.spawn import find_executable
+    if find_executable(name):
+        LOG.info('{} is already installed, skip'.format(name))
         return
-    if file_name.endswith(('.log', '.ini', '.cfg', '.json', '.yml', '.yaml',
-                           '.txt', 'inventory_file')):
-        mode = MODE_600
-    elif re.search(r'\.log\.\d{1,2}$', file_name):
-        mode = MODE_400
+    if find_executable('dpkg'):
+        prefix_cmd = "dpkg --force-all -i"
+        suffix_cmd = '.deb'
     else:
-        mode = MODE_700
-    os.chmod(os.path.join(dir_path, file_name), mode)
+        prefix_cmd = "rpm -ivUh --force --nodeps --replacepkgs"
+        suffix_cmd = '.rpm'
+    pkg_path = os.path.join(ROOT_PATH, 'resources', *paths)
+    if not pkg_path.endswith(('.deb', '.rpm')):
+        pkg_path += suffix_cmd
+    cmd = "{} {}".format(prefix_cmd, pkg_path)
+    if getpass.getuser() != 'root':
+        raise Exception('no permission to run cmd: {}, please run command with root user firstly'.format(cmd))
+    return run_cmd(cmd, oneline=True, shell=True)
 
 
-def update_permissions():
-    for base, dirs, files in os.walk(ROOT_PATH):
-        for dir_name in dirs:
-            update_folder_permission(base, dir_name)
-        for file_name in files:
-            update_file_permission(base, file_name)
+def get_hosts_name(tags):
+    if (isinstance(tags, str) and tags in dl_items) or (isinstance(tags, list) and set(tags) & set(dl_items)):
+        return 'master,worker'
+    return 'worker'
```

## ascend_deployer/downloader/dl_mef_dependency_downloader.py

```diff
@@ -12,38 +12,73 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import json
 import os
+from functools import reduce
 from typing import List
 
 from . import logger_config
 from .download_data import DownloadData
 from .parallel_file_downloader import DownloadFileInfo
 from .software_mgr import PkgInfo
 
 LOG = logger_config.LOG
 
 
 class DlMefDependencyDownloader:
+    DELETE = "Delete"
+    UPDATE = "Update"
 
     def __init__(self, download_data: DownloadData):
         self._download_data = download_data
         self._software_mgr = download_data.software_mgr
         self._software_list = download_data.selected_soft_list
         self._os_list = download_data.selected_os_list
 
     @staticmethod
     def _get_pkg_info_from_json(resources_json) -> List[PkgInfo]:
         with open(resources_json, 'r', encoding='utf-8') as json_file:
             data = json.load(json_file)
         return [PkgInfo(**item) for item in data]
 
+    def _update_or_del_pkg(self, pkg_list: List[PkgInfo], pkg: PkgInfo) -> List[PkgInfo]:
+        """
+        Delete or update COMMON pkg based on COMMON_UPDATE json configuration.
+        :param pkg_list: the list of origin PkgInfo from COMMON
+        :param pkg: PkgInfo from COMMON_UPDATE
+        :eg. {
+             "filename": "aarch64.tar.gz",
+             "dest": "resources/docker/OpenEuler_20.03_LTS",
+             "remark": "Update"
+           }
+        :return: PkgInfo list
+        """
+        if pkg.remark == self.DELETE:
+            return [p for p in pkg_list if not (p.filename == pkg.filename and p.dest == pkg.dest)]
+        elif pkg.remark == self.UPDATE:
+            return [p for p in pkg_list if not (p.filename == pkg.filename and p.dest == pkg.dest)] + [pkg]
+        else:
+            return pkg_list + [pkg]
+
+    def _collect_common_resources(self, os_item: str, version: str) -> List[PkgInfo]:
+        pkg_list: List[PkgInfo] = []
+        common_os_resources = os.path.join(self._download_data.base_dir,
+                                           f'downloader/dependency/COMMON/{os_item}.json')
+        if os.path.exists(common_os_resources):
+            pkg_list.extend(self._get_pkg_info_from_json(common_os_resources))
+        resources_json = os.path.join(self._download_data.base_dir,
+                                      f'downloader/dependency/{version}/COMMON_UPDATE/{os_item}.json')
+        if not os.path.getsize(resources_json):
+            return pkg_list
+        resources = self._get_pkg_info_from_json(resources_json)
+        return reduce(self._update_or_del_pkg, resources, pkg_list)
+
     def _has_dl_or_mef(self):
         for soft in self._download_data.selected_soft_list:
             if "DL" in soft or "MEF" in soft:
                 return True
         return False
 
     def collect_dl_mef_dependency(self):
@@ -52,31 +87,36 @@
             return result
         download_dl = any("DL" in pkg_name for pkg_name in self._software_list)
         download_mef = any("MEF" in pkg_name for pkg_name in self._software_list)
         download_aarch64 = any("aarch64" in os_item for os_item in self._os_list)
         download_x86_64 = any("x86_64" in os_item for os_item in self._os_list)
         software_with_version_list = [self._software_mgr.get_name_version(item, std_out=False) for item in
                                       self._software_list]
-        version = next((pkg_name.split("_")[1] for pkg_name in software_with_version_list
-                        if "DL" in pkg_name or "MEF" in pkg_name), "")
+        dl_version = mef_version = ""
+        for pkg_name in software_with_version_list:
+            if "DL" in pkg_name and "_" in pkg_name:
+                dl_version = pkg_name.split("_")[1]
+            if "MEF" in pkg_name and "_" in pkg_name:
+                mef_version = pkg_name.split("_")[1]
         pkg_info_list: List[PkgInfo] = []
         for os_item in self._os_list:
-            resources_json = os.path.join(self._download_data.base_dir,
-                                          f'downloader/dependency/{version}/COMMON/{os_item}/resource.json')
-            pkg_info_list.extend(self._get_pkg_info_from_json(resources_json))
+            if dl_version:
+                pkg_info_list.extend(self._collect_common_resources(os_item, dl_version))
+            if mef_version:
+                pkg_info_list.extend(self._collect_common_resources(os_item, mef_version))
         for arch, is_download in (('aarch64', download_aarch64), ('x86_64', download_x86_64)):
             if not is_download:
                 continue
             if download_dl:
                 resources_json = os.path.join(self._download_data.base_dir,
-                                              f'downloader/dependency/{version}/DL/{arch}/resource.json')
+                                              f'downloader/dependency/{dl_version}/DL/{arch}/resource.json')
                 pkg_info_list.extend(self._get_pkg_info_from_json(resources_json))
             if download_mef:
                 resources_json = os.path.join(self._download_data.base_dir,
-                                              f'downloader/dependency/{version}/MEF/{arch}/resource.json')
+                                              f'downloader/dependency/{mef_version}/MEF/{arch}/resource.json')
                 pkg_info_list.extend(self._get_pkg_info_from_json(resources_json))
 
         for pkg in pkg_info_list:
             dest_file_path = os.path.join(self._download_data.base_dir, pkg.dest, pkg.filename)
             result.append(DownloadFileInfo(filename=pkg.filename, url=pkg.url, sha256=pkg.sha256,
                                            dst_file_path=dest_file_path))
         return result
```

## ascend_deployer/downloader/download_data.py

```diff
@@ -20,15 +20,16 @@
 
 from .download_util import get_arch, get_specified_python
 from .software_mgr import SoftwareMgr, SoftwareVersion
 
 _PYTHON_MAPPING = {
     "Python-3.7": "cp37",
     "Python-3.8": "cp38",
-    "Python-3.9": "cp39"
+    "Python-3.9": "cp39",
+    "Python-3.10": "cp310"
 }
 
 CUR_DIR = os.path.dirname(os.path.realpath(__file__))
 PROJECT_DIR = os.path.dirname(CUR_DIR)
 
 
 class DownloadData:
```

## ascend_deployer/downloader/download_util.py

```diff
@@ -20,14 +20,15 @@
 import json
 import os
 import platform
 import socket
 import ssl
 import sys
 import time
+import http
 from http.client import IncompleteRead, HTTPException
 from urllib import request
 from urllib.error import ContentTooShortError, URLError
 
 try:
     from . import obs_downloader
 except ImportError:
@@ -278,38 +279,38 @@
             print('please wait for a moment...')
             LOG.info('please wait for a moment...')
             time.sleep(retry * 2)
         return False
 
     @classmethod
     def urlopen(cls, url: str, retry_times=5):
-        ret_buffer = b''
+        res_buffer = b''
         for retry in [x + 1 for x in range(retry_times)]:
             try:
-                cls.proxy_inst.build_proxy_handler(len(ret_buffer))
+                cls.proxy_inst.build_proxy_handler(len(res_buffer))
                 resp = request.urlopen(url)
-                ret_buffer += resp.read()
-                return ret_buffer
+                res_buffer += resp.read()
+                return res_buffer
             except IncompleteRead as err:
                 print(err)
                 LOG.error(err)
-                ret_buffer += err.partial
+                res_buffer += err.partial
             except (ContentTooShortError, URLError, HTTPException) as ex:
                 print(ex)
                 LOG.error(ex)
             except socket.timeout as timeout:
                 socket.setdefaulttimeout(retry * 60)
                 print(timeout)
                 LOG.error(timeout)
             finally:
                 pass
             print('please wait for a moment...')
             LOG.info('please wait for a moment...')
             time.sleep(2)
-        raise UrlOpenError("url open failed,please check the network")
+        raise UrlOpenError("url open failed, please check the network")
 
     @classmethod
     def download_to_tmp(cls, url: str, retry_times=5):
         for retry in [x + 1 for x in range(retry_times)]:
             try:
                 cls.proxy_inst.build_proxy_handler()
                 tmp_file, _ = request.urlretrieve(url)
@@ -371,15 +372,15 @@
         specified_python = CONFIG_INST.get_python_version()
     resources_json = os.path.join(CUR_DIR, 'downloader', 'python_version.json')
     with open(resources_json, 'r', encoding='utf-8') as json_file:
         data = json.load(json_file)
         available_python_list = [item['filename'].rstrip('.tar.xz') for item in data]
         if specified_python not in available_python_list:
             tips = "ascend_python_version is not available, " \
-                   "available Python-x.x.x is in 3.7.0~3.7.11 and 3.8.0~3.8.11 and 3.9.0~3.9.9"
+                   "available Python-x.x.x is in 3.7.0~3.7.11 and 3.8.0~3.8.11 and 3.9.0~3.9.9 and 3.10.0~3.10.11"
             print(tips)
             LOG.error(tips)
             raise PythonVersionError(tips)
     return specified_python
 
 
 def delete_if_exist(dst_file_name: str):
@@ -432,34 +433,14 @@
         :param dst_file: 下载文件文件
         :param sha256:  hash
         :return:
         """
         file_hash = calc_sha256(dst_file)
         return sha256 == file_hash
 
-    @classmethod
-    def check_download_hash(cls, dst_file, url_with_hash):
-        """
-        check_download_hash
-        校验下载文件的hash值与url中的hash值是否相等
-
-        :param dst_file: 下载文件文件
-        :param url_with_hash:  带hash值的URL
-        :return:
-        """
-        if 'sha256=' in url_with_hash:
-            key_word = 'sha256='
-            file_hash = calc_sha256(dst_file)
-        else:
-            key_word = 'md5='
-            file_hash = calc_md5(dst_file)
-        index_of_hash = str(url_with_hash).index(key_word) + len(key_word)
-        target_hash = url_with_hash[index_of_hash:]
-        return target_hash == file_hash
-
 
 CH = CheckHash()
 
 
 class State(object):
     NONE = 0
     EXIT = 1
```

## ascend_deployer/downloader/downloader.py

```diff
@@ -51,15 +51,14 @@
         self.origin_download = None
         self.origin_cann_download = None
         self.progress = 0
         self.download_items = []
         self.res_dir = os.path.join(self.dst, "resources")
         self.finished_items = []
         self.extra_schedule = None
-        self.origin_check_download_hash = None
         self.origin_check_hash = None
         self.origin_print = print
         self.download_path = download_path
         if check and software_list:
             self.check_software_list(os_list, software_list)
         if os.name == 'nt':
             os.system('chcp 65001')
@@ -132,14 +131,16 @@
         return print(str_args, **kwargs, end='')
 
     def mock_download(self, url: str, dst_file_name: str, sha256=""):
         # mock other_downloader.DOWNLOAD_INST.download
         if dst_file_name.endswith(".xml") or dst_file_name.endswith("sqlite.bz2") or dst_file_name.endswith(
                 "sqlite.xz"):
             return self.origin_download(url, dst_file_name, sha256)
+        if not sha256 and 'sha256=' in url:
+            sha256 = url.rsplit('sha256=')[-1]
         self.download_items.append(
             DownloadFileInfo(url=url, dst_file_path=dst_file_name, filename=os.path.basename(dst_file_name),
                              sha256=sha256))
         return True
 
     def mock_check_hash(self, *args, **kwargs):
         return True
@@ -148,16 +149,14 @@
     def collect_python_and_os_pkgs_info(self, os_list, software_list, download_path) -> List[DownloadFileInfo]:
         self.check_space(self.download_path)
         msg = Color.info('start analyzing the amount of packages to be downloaded ...')
         self.origin_print(msg)
         LOG.info(msg, extra=logger_config.LOG_CONF.EXTRA)
         self.origin_download = DOWNLOAD_INST.download
         DOWNLOAD_INST.download = self.mock_download
-        self.origin_check_download_hash = download_util.CH.check_download_hash
-        download_util.CH.check_download_hash = self.mock_check_hash
         self.origin_check_hash = download_util.CH.check_hash
         download_util.CH.check_hash = self.mock_check_hash
         pip_downloader.print = self.mock_print
         download_util.print = self.mock_print
         os_dep_downloader.print = self.mock_print
         deb_downloader.print = self.mock_print
         rpm_downloader.print = self.mock_print
@@ -176,17 +175,15 @@
             sys.stdout = origin_output
             LOG.disabled = False
             pip_downloader.LOG.disabled = False
             os_dep_downloader.LOG.disabled = False
             deb_downloader.LOG.disabled = False
             rpm_downloader.LOG.disabled = False
             print = self.origin_print
-            download_util.CH.check_download_hash = self.origin_check_download_hash
             download_util.CH.check_hash = self.origin_check_hash
-            pip_downloader.my_pip.downloaded = []
             DOWNLOAD_INST.download = self.origin_download
         msg = f'finish analyzing ...'
         print(msg)
         LOG.info(msg, extra=logger_config.LOG_CONF.EXTRA)
         return self.download_items
 
     def download_python_and_os_pkgs(self, os_list, software_list, dst):
```

## ascend_deployer/downloader/logger_config.py

```diff
@@ -74,15 +74,15 @@
     CLIENT_IP = os.getenv('SSH_CLIENT', 'localhost').split()[0]
     EXTRA = {'user_name': USER_NAME, 'client_ip': CLIENT_IP}
     LOG_DATE_FORMAT = '%Y-%m-%d %H:%M:%S'
     LOG_FORMAT_STRING = \
             "%(asctime)s downloader [%(levelname)s] " \
             "[%(filename)s:%(lineno)d %(funcName)s] %(message)s"
     LOG_FORMAT_STRING_OPERATION = \
-            "%(asctime)s %(user_name)s@%(client_ip)s [%(levelname)s] " \
+            "%(asctime)s localhost [%(levelname)s] " \
             "[%(filename)s:%(lineno)d %(funcName)s] %(message)s"
     LOG_LEVEL = logging.INFO
 
     ROTATING_CONF = dict(
         mode='a',
         maxBytes=20 * 1024 * 1024,
         backupCount=5,
```

## ascend_deployer/downloader/obs_resources.json

### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'cffi-1.15.1-cp27-cp27mu-linux_aarch64.whl'": "'https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/cffi-1.15.1-cp27-cp27mu-linux_aarch64.whl#sha256=2a0d64defe58d04a50ff7ab8085e3d5203db16d699b49a0ffe0bea29901bb07a'",*

 * * "'cryptography-3.3.2-cp27-cp27mu-linux_aarch64.whl'": "'https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/cryptography-3.3.2-cp27-cp27mu-linux_aarch64.whl#sha256=413cf0d9cb6395fa5acb04e25a1c0730903fb065ca1c00d9d8a3ec09242132a4'"}*

```diff
@@ -1,8 +1,10 @@
 {
+    "cffi-1.15.1-cp27-cp27mu-linux_aarch64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/cffi-1.15.1-cp27-cp27mu-linux_aarch64.whl#sha256=2a0d64defe58d04a50ff7ab8085e3d5203db16d699b49a0ffe0bea29901bb07a",
+    "cryptography-3.3.2-cp27-cp27mu-linux_aarch64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/cryptography-3.3.2-cp27-cp27mu-linux_aarch64.whl#sha256=413cf0d9cb6395fa5acb04e25a1c0730903fb065ca1c00d9d8a3ec09242132a4",
     "h5py-3.1.0-cp37-cp37m-manylinux1_x86_64.whl": "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/packages/9d/74/9eae2bedd8201ab464308f42c601a12d79727a1c87f0c867fdefb212c6cf/h5py-3.1.0-cp37-cp37m-manylinux1_x86_64.whl#sha256=236ac8d943be30b617ab615c3d4a4bf4a438add2be87e54af3687ab721a18fac",
     "h5py-3.1.0-cp37-cp37m-manylinux2014_aarch64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/h5py-3.1.0-cp37-cp37m-manylinux2014_aarch64.whl#sha256=40dd06dce42fdb004b54a8f357ab6c181579320d410ad6ab0b0921f26df34f55",
     "numpy-1.17.5-cp37-cp37m-manylinux1_x86_64.whl": "https://repo.huaweicloud.com/repository/pypi/packages/b1/51/20098150b6108061cb7542af3de7bfcfe0182bca21613697153e49dc4adc/numpy-1.17.5-cp37-cp37m-manylinux1_x86_64.whl#sha256=31db2f9604afbf897b23478942074bbbb2513467d2b4b4ac573a7b65c63c073c",
     "numpy-1.17.5-cp37-cp37m-manylinux2014_aarch64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/numpy-1.17.5-cp37-cp37m-manylinux2014_aarch64.whl#sha256=91536ef98e66153975117715839317a882dd949113be6a884665c08de0ea407c",
     "psutil-5.9.4-cp37-abi3-manylinux1_x86_64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/psutil-5.9.4-cp37-abi3-manylinux1_x86_64.whl#sha256=233d367200e3ca46be03a49c414a8a64755360ef8cf6e0d197d42b7f848b9b1f",
     "psutil-5.9.4-cp37-abi3-manylinux_2_17_aarch64.whl": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/psutil-5.9.4-cp37-abi3-manylinux_2_17_aarch64.whl#sha256=de114240860fca58c281ea5960b0d9d7c9f90412cdd4578fbc3cc4ae18a7eff6"
 }
```

## ascend_deployer/downloader/os_dep_downloader.py

```diff
@@ -47,40 +47,53 @@
         docker_pkg_list = [
             "docker-ce-cli",
             "containerd.io",
             "docker-ce",
             "docker-ce-rootless-extras",
             "docker-scan-plugin",
             "docker-engine",
+            "libseccomp2",
+            "libseccomp"
         ]
+
+        if "EulerOS" in os_item:
+            docker_pkg_list.append("libtool-ltdl")
         dst_dir = os.path.join(dst, os_item)
         if not os.path.exists(dst_dir):
             os.makedirs(dst_dir, mode=0o750, exist_ok=True)
         docker_dir = os.path.join(dst_dir, 'docker')
         if not os.path.exists(docker_dir):
             os.makedirs(docker_dir, mode=0o750, exist_ok=True)
         LOG.info('item:{} save dir: {}'.format(os_item, os.path.basename(dst_dir)))
 
         config_file = os.path.join(self.project_dir, 'downloader/config/{0}/pkg_info.json'.format(os_item))
         source_list_file = os.path.join(self.project_dir, 'downloader/config/{0}/source.list'.format(os_item))
         downloader = None
+        res = {'ok': [], 'failed': []}
+        with open(config_file, 'r', encoding='utf-8') as fid:
+            content = json.load(fid)
+            if isinstance(content, list):
+                package_count = len(content)
+            else:
+                package_count = 0
+            if not package_count:  # skip empty pkg_info.json, for user installed by self
+                return res
 
         if os.path.exists(source_list_file):
             if 'aarch64' in os_item:
                 downloader = Apt(source_list_file, 'aarch64')
             else:
                 downloader = Apt(source_list_file, 'x86_64')
         else:
             source_repo_file = os.path.join(self.project_dir, 'downloader/config/{0}/source.repo'.format(os_item))
             if 'aarch64' in os_item:
                 downloader = Yum(source_repo_file, 'aarch64')
             else:
                 downloader = Yum(source_repo_file, 'x86_64')
 
-        res = {'ok': [], 'failed': []}
         if downloader is not None:
             if downloader.make_cache() is False:
                 LOG.error('downloader make_cache failed')
                 res.get('failed', []).append(os_item)
                 raise RuntimeError
 
         with open(config_file, 'r', encoding='utf-8') as f:
```

## ascend_deployer/downloader/other_downloader.py

```diff
@@ -38,14 +38,15 @@
         self._software_list = download_data.selected_soft_list
         self._selected_soft_ver_list = download_data.selected_soft_ver_list
         self._base_dir = download_data.base_dir
         self._software_mgr = download_data.software_mgr
         self._non_ai_frame_list = [soft_ver for soft_ver in self._selected_soft_ver_list if
                                    not self._is_ai_frame(soft_ver)]
         self._ai_frame_list = [soft_ver for soft_ver in self._selected_soft_ver_list if self._is_ai_frame(soft_ver)]
+        self._warning_message = set()
 
     @staticmethod
     def _is_ai_frame(soft_ver: SoftwareVersion):
         return any(soft in soft_ver.name for soft in OtherDownloader._AI_FRAMES)
 
     @staticmethod
     def _unsupported_arch_mind_studio_file(filename, arch):
@@ -79,14 +80,16 @@
     def _collect_download_software(self, soft_ver: SoftwareVersion, arch) -> List[DownloadFileInfo]:
         """
         下载软件的其他资源
         """
         other_pkgs = self._software_mgr.get_software_other(soft_ver.name, soft_ver.version)
         other_pkgs = [pkg for pkg in other_pkgs if
                       not self._unsupported_arch_mind_studio_file(pkg.filename, self._arch)]
+        if "CANN" in soft_ver.name and "3.10." in self._download_data.specified_python:
+            other_pkgs = [pkg for pkg in other_pkgs if "tfplugin" not in pkg.filename]
         download_dir = os.path.join(self._base_dir, "resources", "{0}_{1}".format(soft_ver.name, soft_ver.version))
         self._mk_download_dir(other_pkgs, download_dir, soft_ver)
         if soft_ver.name in ("CANN", "NPU"):
             results = self._collect_pkgs_by_arch(arch, download_dir, self._base_dir, other_pkgs)
         else:
             results = [DownloadFileInfo(filename=item.filename, url=item.url, sha256=item.sha256,
                                         dst_file_path=os.path.join(download_dir, item.filename))
@@ -131,21 +134,24 @@
         download_dir = os.path.join(self._base_dir, "resources")
         os_item_split = os_item.split("_")
         os_name, arch = "_".join(os_item_split[:2]), "_".join(os_item_split[2:])
         whl_list = self._software_mgr.get_software_framework(soft_ver.name, "linux_{}".format(arch), soft_ver.version)
         result = []
         for item in whl_list:
             if item.python != self._download_data.py_implement_flag:
-                print("Try to get {} on {}, but it does not match {}".format
-                      (item.filename, item.python, self._download_data.py_implement_flag))
                 continue
             dest_file = os.path.join(download_dir, item.dest, os.path.basename(item.url))
             result.append(
                 DownloadFileInfo(filename=item.filename, url=item.url, sha256=item.sha256, dst_file_path=dest_file))
+        if not result:
+            self._warning_message.add("No {} {} found for {} on {}, skipping...".format(
+                soft_ver.name, soft_ver.version, self._download_data.specified_python, arch))
         return result
 
     def collect_ai_framework(self):
         result = []
         for os_item in self._download_data.selected_os_list:
             for framework_soft_ver in self._ai_frame_list:
                 result.extend(self._collect_framework_whl(os_item, framework_soft_ver))
+        if self._warning_message:
+            print("\n".join(self._warning_message))
         return result
```

## ascend_deployer/downloader/other_resources.json

### Pretty-printed

 * *Similarity: 0.4166666666666667%*

 * *Differences: {'delete': '[9, 8, 7, 6, 5, 4, 3]'}*

```diff
@@ -15,56 +15,14 @@
         "dest": "resources/nexus",
         "filename": "nexus_3.53.1_x86_64.tar",
         "sha256": "8886381c3a65f13970e91d828fc4ebbfdf53904c6c86f0e9feb19d369a127475",
         "url": "https://ascend-repo-modelzoo.obs.cn-east-2.myhuaweicloud.com/MindXDL/5.0.RC1/resources/nexus_3.53.1_x86_64.tar"
     },
     {
         "dest": "resources/sources",
-        "filename": "gcc-7.3.0.tar.gz",
-        "sha256": "fa06e455ca198ddc11ea4ddf2a394cf7cfb66aa7e0ab98cc1184189f1d405870",
-        "url": "https://mirrors.huaweicloud.com/gnu/gcc/gcc-7.3.0/gcc-7.3.0.tar.gz"
-    },
-    {
-        "dest": "resources/sources",
-        "filename": "gmp-6.1.0.tar.bz2",
-        "sha256": "498449a994efeba527885c10405993427995d3f86b8768d8cdf8d9dd7c6b73e8",
-        "url": "https://mirrors.huaweicloud.com/gnu/gmp/gmp-6.1.0.tar.bz2"
-    },
-    {
-        "dest": "resources/sources",
-        "filename": "mpfr-3.1.4.tar.bz2",
-        "sha256": "d3103a80cdad2407ed581f3618c4bed04e0c92d1cf771a65ead662cc397f7775",
-        "url": "https://mirrors.huaweicloud.com/gnu/mpfr/mpfr-3.1.4.tar.bz2"
-    },
-    {
-        "dest": "resources/sources",
-        "filename": "mpc-1.0.3.tar.gz",
-        "sha256": "617decc6ea09889fb08ede330917a00b16809b8db88c29c31bfbb49cbf88ecc3",
-        "url": "https://mirrors.huaweicloud.com/gnu/mpc/mpc-1.0.3.tar.gz"
-    },
-    {
-        "dest": "resources/sources",
-        "filename": "isl-0.16.1.tar.bz2",
-        "sha256": "412538bb65c799ac98e17e8cfcdacbb257a57362acfaaff254b0fcae970126d2",
-        "url": "https://mindx.obs.cn-south-1.myhuaweicloud.com/opensource/isl-0.16.1.tar.bz2"
-    },
-    {
-        "dest": "resources/sources",
-        "filename": "cmake-3.20.5.tar.gz",
-        "sha256": "12c8040ef5c6f1bc5b8868cede16bb7926c18980f59779e299ab52cbc6f15bb0",
-        "url": "https://mindx.obs.cn-south-1.myhuaweicloud.com/opensource/cmake-3.20.5.tar.gz"
-    },
-    {
-        "dest": "resources/pylibs",
-        "filename": "PyQt5-5.14.0-5.14.0-cp35.cp36.cp37.cp38-abi3-manylinux1_x86_64.whl",
-        "sha256": "a757ba71c51f428b52ba404e781e2f19b4436b2c31298b8313339d5817781b65",
-        "url": "https://repo.huaweicloud.com/repository/pypi/packages/88/d0/4572492d633e311c0143ba20596cb5c090d37442d1cd431082193f3bbb3a/PyQt5-5.14.0-5.14.0-cp35.cp36.cp37.cp38-abi3-manylinux1_x86_64.whl"
-    },
-    {
-        "dest": "resources/sources",
         "filename": "mpich-3.2.1.tar.gz",
         "sha256": "5db53bf2edfaa2238eb6a0a5bc3d2c2ccbfbb1badd79b664a1a919d2ce2330f1",
         "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/mpich-3.2.1.tar.gz"
     },
     {
         "dest": "resources/sources",
         "filename": "openmpi-4.1.5.tar.gz",
```

## ascend_deployer/downloader/parallel_file_downloader.py

```diff
@@ -121,15 +121,15 @@
             return 0
         return block_num * 1.0 / total_size
 
     def get_percent(self, block_info: DownloadingBlockInfo):
         if block_info.total_size == 0:
             return 0
         if self.obs_check:
-            percent = block_info.block_num / block_info.total_size
+            percent = block_info.block_num / block_info.block_size
         else:
             percent = block_info.block_num * block_info.block_size / block_info.total_size
         if percent > 1:
             return 1
         return percent
 
     def build_downloading_status(self, block_info: DownloadingBlockInfo):
@@ -223,14 +223,21 @@
             raise DownloadError(file_info.url, file_info.dst_file_path)
         else:
             LOG.info('download %s successfully', file_info.url)
             return True
 
     def _download_with_retry(self, file_info: DownloadFileInfo, retry_times=5):
         socket.setdefaulttimeout(20)
+        need_change_item = ["libtool-ltdl"]
+        file_name = os.path.basename(file_info.dst_file_path)
+        file_name_dir = os.path.basename(os.path.dirname(file_info.dst_file_path))
+        for item in need_change_item:
+            if "EulerOS" in file_info.dst_file_path and "docker" != file_name_dir and item in file_name:
+                file_info.dst_file_path = '/docker/'.join(file_info.dst_file_path.rsplit('/', 1))
+                break
         for retry in range(1, retry_times + 1):
             try:
                 LOG.info('downloading try: %s from %s', retry, file_info.url)
                 DownloadUtil.proxy_inst.build_proxy_handler()
                 is_use_obs = HAS_OBS_CLIENT and DownloadUtil.use_obs(file_info.url)
                 status_builder = DownloadingStatusBuilder(file_info.filename, is_use_obs)
                 if is_use_obs:
```

## ascend_deployer/downloader/pip_downloader.py

```diff
@@ -1,383 +1,213 @@
 #!/usr/bin/env python3
 # coding: utf-8
-# Copyright 2020 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
-
-import http.client
 import os
 import json
-import time
 import urllib.parse
 from html.parser import HTMLParser
+from typing import List, Dict
 
 from . import logger_config
-from .download_util import CONFIG_INST, DOWNLOAD_INST, CheckHash
-from .download_util import calc_sha256, get_arch, get_specified_python, CH, DownloadCheckError, UrlOpenError
+from .download_util import CONFIG_INST, DOWNLOAD_INST, get_specified_python
 
-LOG = logger_config.LOG
+__all__ = ('LinkParser', 'Package', 'Pip', 'download', 'pip')
 
+DOWNLOADER_PATH = os.path.dirname(__file__)
+LOG = logger_config.LOG
+UNIQUE_PYTHON_DEPENDENCIES = {
+    "cp310": ["matplotlib==3.7.1", "pandas==2.0.3", "cycler==0.11.0", "kiwisolver==1.3.2", "numpy==1.21.3",
+              "Pillow==8.3.2", "setuptools_scm==4.1.1", "cppy==1.2.0", "pybind11==2.6.1", "scipy==1.7.2",
+              "contourpy==1.0.1", "fonttools==4.22.1", ]
+}
 
-class SimpleIndexParser(HTMLParser):
-    """
-    解析simple index
-    """
 
-    def __init__(self):
+class LinkParser(HTMLParser):
+    def __init__(self, base_url):
         super().__init__()
-        self.index = {}
-        self.tmp_attrs = None
-
-    def get_index(self):
-        """
-        get_index  获取解析到的软件包的索引
-
-        :return:  索引
-        """
-        return self.index
+        self.base_url = base_url
+        self.links = {}
+        self.last_link = {}
 
     def handle_starttag(self, tag, attrs):
-        """
-        handle_starttag  解析tag开始
-        """
-        if tag == 'a':
-            self.tmp_attrs = attrs
+        if tag != 'a':
+            return
+        self.last_link = urllib.parse.urljoin(self.base_url, dict(attrs).get('href'))
 
     def handle_data(self, data):
-        """
-        handle_starttag  解析tag中的数据
-        """
-        if self.tmp_attrs is not None:
-            self.index[data] = self.tmp_attrs[0][1]
-
-
-class MyPip(object):
-    """
-    downloader for pip
-    """
-
-    def __init__(self):
-        self.cache = {}
-        self.downloaded = []
-        # 读取配置
-        script = os.path.realpath(__file__)
-        self.pypi_url = CONFIG_INST.get_pypi_url()
-        self.require_file = os.path.join(os.path.dirname(script), 'requirements.txt')
-        self.obs_resources_file = os.path.join(os.path.dirname(script), 'obs_resources.json')
-        self.repo_path = os.path.join(os.path.dirname(script), '../resources/pylibs')
-
-    @staticmethod
-    def file_download(url, dest):
-        """
-        file_download
-
-        :param url:  待下载文件的url
-        :param dest: 下载时本地文件名,带路径
-        :return:
-        """
-        if os.path.exists(dest):
-            LOG.info('[{0}] exist'.format(os.path.basename(dest)))
-            os.remove(dest)
-            LOG.info('[{0}] deleted'.format(os.path.basename(dest)))
-        DOWNLOAD_INST.download(url, dest)
-
-    @staticmethod
-    def is_wheel_match(full_name, version, platform, implement):
-        """
-        is_wheel_match
-
-        :param full_name:
-        :param version:
-        :param platform:
-        :param implement:
-        :return:
-        """
-        try:
-            elements = full_name.split('-')
-            wheel_version = elements[1]
-            wheel_impl = elements[2]
-            wheel_platform = elements[4].split('.')[0]
-            if wheel_version != version:
-                return False
-
-            if wheel_impl not in ('py3', 'py2.py3', implement):
-                return False
-
-            if wheel_platform not in ('any', platform):
-                return False
-
-        except IndexError as err:
-            print(err)
-            LOG.error(err)
-            return False
-        finally:
-            pass
-
-        return True
-
-    @staticmethod
-    def source_filter(index, version):
-        """
-        source_filter
-
-        :param index:
-        :param version:
-        :return:
-        """
-        pkg = ''
-        url = ''
-        for name, href in index.items():
-            if 'tar' in name or 'zip' in name:
-                if version in name:
-                    pkg = name
-                    url = href
-            else:
-                continue
-        return pkg, url
-
-    @staticmethod
-    def need_download_again(dst_file, url_with_hash):
-        """
-        need_download_again
-        校验目的文件的hash值与url中的hash值是否相等，来决定是否重新下载
-
-        :param dst_file: 目的文件
-        :param url_with_hash:  带hash值的URL
-        :return:
-        """
-        if url_with_hash is None or len(url_with_hash) == 0:
-            return True
-        if not os.path.exists(dst_file):
-            return True
+        if self.lasttag != 'a':
+            return
+        self.links[data] = self.last_link
+
+
+class Package(object):
+    def __init__(self, name, version, url, style, filename, cp='', abi='', arch=''):
+        self.name = name
+        self.version = version
+        self.url = url
+        self.style = style
+        self.filename = filename
+        self.cp = cp
+        self.abi = abi
+        self.arch = arch
+
+    def __str__(self):
+        return f'Package(name={self.name}, version={self.version}, style={self.style}, cp={self.cp}, ' \
+               f'abi={self.abi}, arch={self.arch})'
+
+    @classmethod
+    def parse_source(cls, tar_name, pkg, version, url):
+        pkg_name, ver = tar_name.replace('.tar.gz', '').replace('.zip', '').rsplit('-', 1)
+        if ver == version:
+            return cls(pkg, version, url, 'source', tar_name)
+        return None
+
+    @classmethod
+    def parse_wheel(cls, whl_name, pkg, version, url):
+        pkg_name, ver, cp, abi, arch = whl_name.rstrip('.whl').rsplit('-', 4)
+        if ver == version:
+            return cls(pkg, version, url, 'wheel', whl_name, cp, abi, arch)
+        return None
+
+    @classmethod
+    def parse(cls, name, pkg, version, url):
+        if name.endswith(('.tar.gz', '.zip')):
+            return cls.parse_source(name, pkg, version, url)
+        elif name.endswith('.whl'):
+            return cls.parse_wheel(name, pkg, version, url)
+        else:
+            return None
 
-        return not CheckHash.check_download_hash(dst_file, url_with_hash)
+    def download(self, save_dir):
+        file_path = os.path.join(save_dir, self.filename)
+        DOWNLOAD_INST.download(self.url, file_path)
+        LOG.info(f'download {self.filename} successfully')
 
-    def get_simple_index(self, distribution):
-        """
-        get_simple_index
 
-        :param distribution:
-        :return:
-        """
-        if distribution in self.cache.keys():
-            index = self.cache.get(distribution)
-        else:
-            url = '{0}/{1}/'.format(self.pypi_url, distribution.lower())
-            LOG.info('pypi URL = [{0}]'.format(url))
-            index = DOWNLOAD_INST.urlopen(url)
-            self.cache[distribution] = index
-
-        parser = SimpleIndexParser()
-        parser.feed(index.decode())
-        idx = parser.get_index()
-        return idx
+class Pip(object):
+    arch_map = {
+        'x86_64': ('linux_x86_64', 'manylinux1_x86_64', 'manylinux2010_x86_64', 'manylinux2014_x86_64', 'any'),
+        'aarch64': ('linux_aarch64', 'manylinux_2_17_aarch64', 'manylinux2014_aarch64', 'any')
+    }
 
-    def wheel_filter(self, index, version, platform, implement):
-        """
-        wheel_filter
+    def __init__(self, pypi_url: str, link_cache: Dict[str, str] = None):
+        self.cache = {}
+        self.pypi_url = pypi_url
+        self.url_cache = link_cache or {}
 
-        :param index:
-        :param version:
-        :param platform:
-        :param implement:
-        :return:
+    def filter(self, pkgs: List[Package], cp: str, arch: str) -> List[Package]:
         """
-        pkg = ''
-        url = ''
-        for name, href in index.items():
-            if 'whl' in name:
-                if self.is_wheel_match(name, version, platform, implement):
-                    pkg = name
-                    url = href
-            else:
+        available pkgs must meet below requirements:
+            1.whl(or):
+                1. pkg.abi == abi3 and pkg.abi <= target_cp
+                2. pkg.arch match target arch
+            2.source
+        choice order:
+            1. whl > source
+            2. pkg.filename
+        """
+        results = []
+        available_cp_set = {cp, 'py{}'.format(cp[2:3])}
+        for pkg in pkgs:
+            if pkg.cp:
+                if pkg.abi == 'abi3':
+                    cps = [int(x.strip('cp')) for x in pkg.cp.split('.')]
+                    target_cp = int(cp.strip('cp'))
+                    if pkg.cp.startswith('cp') and not any(filter(lambda x: x <= target_cp, cps)):
+                        continue
+                elif not (set(pkg.cp.split('.')) & available_cp_set):
+                    continue
+            if pkg.arch and not (set(pkg.arch.split('.')) & set(self.arch_map.get(arch, []))):
                 continue
-        return pkg, url
+            results.append(pkg)
+        results.sort(key=lambda x: (x.style, x.filename), reverse=True)
+        return results
+
+    def update_cache_url(self, pkg_name: str, links: Dict[str, str]):
+        for name, link in self.url_cache.items():
+            if pkg_name in name:
+                links[name] = link
+                LOG.info('update {} link to {}'.format(name, link))
+
+    def get_links(self, pkg_name: str):
+        dist_name = pkg_name.lower()
+        if dist_name not in self.cache:
+            if not self.pypi_url.endswith('/'):
+                self.pypi_url += '/'
+            dist_url = urllib.parse.urljoin(self.pypi_url, dist_name + '/')
+            res_buffer = DOWNLOAD_INST.urlopen(dist_url)
+            parser = LinkParser(dist_url)
+            parser.feed(res_buffer.decode())
+            self.update_cache_url(pkg_name, parser.links)
+            self.cache[dist_name] = parser.links
+            LOG.info(f'save {pkg_name}({dist_name}) links to cache')
+        return self.cache.get(dist_name)
+
+    def filter_pkg(self, links: Dict[str, str], pkg_name: str, version: str, cp: str, arch: str) -> Package:
+        choices = []
+        for name, link in links.items():
+            pkg = Package.parse(name, pkg_name, version, link)
+            if pkg:
+                choices.append(pkg)
+        filter_choices = self.filter(choices, cp, arch)
+        if filter_choices:
+            LOG.info(f'for {pkg_name}=={version}, available choices: {[p.filename for p in filter_choices]}')
+            return filter_choices[0]
+        LOG.error(f'no available package found for {pkg_name}=={version}')
+
+    def download_pkg(self, save_dir: str, name: str, cp: str, arch: str):
+        pkg_name, version = name.split('==')
+        links = self.get_links(pkg_name)
+        pkg = self.filter_pkg(links, pkg_name, version, cp, arch)
+        if not pkg:
+            raise Exception(f'no available package found for {name}')
+        pkg.download(save_dir)
 
-    def get_url_from_obs(self, name, platform, implement):
-        if platform == 'none':
-            return "", ""
-        distribution, version = name.split('==')
-        with open(self.obs_resources_file) as file_content:
-            index = json.load(file_content)
-            for file_name, href in index.items():
-                elements = file_name.split('-')
-                try:
-                    wheel_name = elements[0]
-                    wheel_version = elements[1].split('+')[0]
-                    wheel_impl = elements[2]
-                    wheel_platform = elements[4].split('.')[0]
-                except IndexError as err:
-                    print(err)
-                    LOG.error(err)
-                if wheel_name != distribution:
-                    continue
-                if wheel_version != version:
-                    continue
-                if wheel_impl not in ('py3', 'py2.py3', implement):
-                    continue
-                if wheel_platform not in ('any', platform):
-                    continue
-                return file_name, href
-            return "", ""
 
-    def download_wheel(self, name, platform, implement, dest_path):
-        """
-        下载软件包
-        """
-        # get url from pypi
-        distribution, version = name.split('==')
-        index = self.get_simple_index(distribution)
-        file_name, url = self.wheel_filter(index, version, platform, implement)
-        if len(url) == 0:
-            # get url from obs
-            file_name, download_url = self.get_url_from_obs(name, platform, implement)
-            if not download_url:
-                LOG.info('can not find {0} for {1} {2}'.format(name, platform, implement))
-                return False
+def download(os_list, res_dir):
+    """download ansible and requirement base on os_list"""
+    arches = set()
+    for os_item in os_list:
+        if 'x86_64' in os_item:
+            arches.add('x86_64')
         else:
-            download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
-
-        if file_name in self.downloaded:
-            return True
-        LOG.info("Download {0} from [{1}]".format(file_name, download_url))
-        file_path = os.path.join(dest_path, file_name)
-        if not self.need_download_again(file_path, download_url):
-            print(file_name.ljust(60), "exists")
-            LOG.info('{0} no need download again'.format(file_name))
-            self.downloaded.append(file_name)
-            return True
-        self.file_download(download_url, file_path)
-        if not CH.check_download_hash(file_path, download_url):
-            LOG.info('the downloaded file：{} hash is not equal to the hash in the url'.format(file_path))
-            raise DownloadCheckError(f"file_path: {file_path}, download_url: {download_url}")
-        print(file_name.ljust(60), "download success")
-        self.downloaded.append(file_name)
-        return True
-
-    def download_source(self, name, dest_path):
-        """
-        下载源码包
-        """
-        distribution, version = name.split('==')
-        index = self.get_simple_index(distribution)
-        file_name, url = self.source_filter(index, version)
-        if len(url) == 0:
-            return False
-        if file_name in self.downloaded:
-            return True
-        download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
-        LOG.info("Download {0} from [{1}]".format(file_name, download_url))
-        file_path = os.path.join(dest_path, file_name)
-        if not self.need_download_again(file_path, url):
-            print(file_name.ljust(60), "exists")
-            LOG.info('{0} no need download again'.format(file_name))
-            self.downloaded.append(file_name)
-            return True
-        self.file_download(download_url, file_path)
-        if not CH.check_download_hash(file_path, url):
-            LOG.info('the downloaded file：{} hash is not equal to the hash in the url'.format(file_path))
-            raise DownloadCheckError(file_path)
-        print(file_name.ljust(60), "download success")
-        self.downloaded.append(file_name)
-        return True
+            arches.add('aarch64')
+    save_dir = os.path.join(res_dir, 'pylibs')
 
-    def download_x86(self, name, implement_flag, dest_path):
-        """
-        download_x86
-
-        :param name:
-        :param implement_flag:
-        :param dest_path:
-        :return:
-        """
-        platform_list = ('linux_x86_64', 'manylinux1_x86_64', 'manylinux2010_x86_64',
-                         'manylinux2014_x86_64')
-        for platform in platform_list:
-            if self.download_wheel(name, platform, implement_flag, dest_path):
-                return True
-        return False
-
-    def download_arm(self, name, implement_flag, dest_path):
-        """
-        download_arm
-
-        :param name:
-        :param implement_flag:
-        :param dest_path:
-        :return:
-        """
-        platform_list = ('linux_aarch64', 'manylinux_2_17_aarch64', 'manylinux2014_aarch64')
-        for platform in platform_list:
-            if self.download_wheel(name, platform, implement_flag, dest_path):
-                return True
-        return False
-
-    def download(self, name, dest_path, arch):
-        """
-        download
-
-        :param name:
-        :param dest_path:
-        :return:
-        """
-        try:
-            specified_python = get_specified_python()
-            if "Python-3.7" in specified_python:
-                implement_flag = "cp37"
-            if "Python-3.8" in specified_python:
-                implement_flag = "cp38"
-            if "Python-3.9" in specified_python:
-                implement_flag = "cp39"
-
-            if not os.path.exists(dest_path):
-                os.makedirs(dest_path, mode=0o750, exist_ok=True)
-
-            if self.download_wheel(name, "none", implement_flag, dest_path):
-                return True
-
-            if "x86_64" in arch and not self.download_x86(name, implement_flag, dest_path):
-                self.download_source(name, dest_path)
-
-            if "aarch64" in arch and not self.download_arm(name, implement_flag, dest_path):
-                self.download_source(name, dest_path)
-            return True
-        except Exception:
-            print(name.ljust(60), "download failed")
-            raise
-        finally:
-            pass
-
-
-my_pip = MyPip()
-
-
-def download(os_list, res_dir):
-    """
-    按软件列表下载其他部分
-    """
-    if os_list is None:
-        os_list = []
-    arch = get_arch(os_list)
-    repo_path = os.path.join(res_dir, 'pylibs')
-    LOG.info('pip arch is {0}'.format(arch))
-
-    results = {'ok': [], 'failed': []}
-    with open(my_pip.require_file) as file_content:
-        for line in file_content:
-            LOG.info('[{0}]'.format(line.strip()))
-            if my_pip.download(line.strip(), repo_path, arch):
-                results.get('ok', []).append(line.strip())
-                continue
-            results.get('failed', []).append(line.strip())
-    return results
+    ansible_require_file = os.path.join(DOWNLOADER_PATH, 'ansible_reqs.json')
+    with open(ansible_require_file) as f:
+        reqs = json.load(f)
+    for cp, lines in reqs.items():
+        for arch in arches:
+            for line in lines:
+                pip.download_pkg(save_dir, line, cp, arch)
+
+    require_file = os.path.join(DOWNLOADER_PATH, 'requirements.txt')
+    specified_python = get_specified_python()
+    cp = ''.join(specified_python.replace('Python-', 'cp').split('.')[:2])
+    requirements_packages = []
+    with open(require_file) as f:
+        requirements_packages = f.readlines()
+
+    unique_dependencies = UNIQUE_PYTHON_DEPENDENCIES.get(cp, [])
+    requirements_packages.extend(unique_dependencies)
+    for package_info in requirements_packages:
+        for arch in arches:
+            pip.download_pkg(save_dir, package_info.strip(), cp, arch)
+
+
+with open(os.path.join(DOWNLOADER_PATH, 'obs_resources.json')) as cache_file:
+    url_cache = json.load(cache_file)
+pip = Pip(CONFIG_INST.get_pypi_url(), link_cache=url_cache)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## ascend_deployer/downloader/python_version.json

### Pretty-printed

 * *Similarity: 0.7391304347826086%*

 * *Differences: {'insert': "[(34, OrderedDict([('filename', 'Python-3.10.0.tar.xz'), ('url', "*

 * *           "'https://mirrors.huaweicloud.com/python/3.10.0/Python-3.10.0.tar.xz'), ('sha256', "*

 * *           "'5a99f8e7a6a11a7b98b4e75e0d1303d3832cada5534068f69c7b6222a7b1b002'), ('dest', "*

 * *           "'resources/sources')])), (35, OrderedDict([('filename', 'Python-3.10.1.tar.xz'), "*

 * *           "('url', 'https://mirrors.huaweicloud.com/python/3.10.1/Python-3.10.1.tar.xz'), "*

 * *           "('sha256', 'a7f1265b6e1a5de1ec5c3ec7019ab5341 […]*

```diff
@@ -198,9 +198,81 @@
         "url": "https://mirrors.huaweicloud.com/python/3.8.10/Python-3.8.10.tar.xz"
     },
     {
         "dest": "resources/sources",
         "filename": "Python-3.8.11.tar.xz",
         "sha256": "fb1a1114ebfe9e97199603c6083e20b236a0e007a2c51f29283ffb50c1420fb2",
         "url": "https://mirrors.huaweicloud.com/python/3.8.11/Python-3.8.11.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.0.tar.xz",
+        "sha256": "5a99f8e7a6a11a7b98b4e75e0d1303d3832cada5534068f69c7b6222a7b1b002",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.0/Python-3.10.0.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.1.tar.xz",
+        "sha256": "a7f1265b6e1a5de1ec5c3ec7019ab53413469934758311e9d240c46e5ae6e177",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.1/Python-3.10.1.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.2.tar.xz",
+        "sha256": "17de3ac7da9f2519aa9d64378c603a73a0e9ad58dffa8812e45160c086de64c7",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.2/Python-3.10.2.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.3.tar.xz",
+        "sha256": "596c72de998dc39205bc4f70ef0dbf7edec740a306d09b49a9bd0a77806730dc",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.3/Python-3.10.3.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.4.tar.xz",
+        "sha256": "80bf925f571da436b35210886cf79f6eb5fa5d6c571316b73568343451f77a19",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.4/Python-3.10.4.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.5.tar.xz",
+        "sha256": "8437efd5b106ef0a75aabfbf23d880625120a73a86a22ade4d2e2e68d7b74486",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.5/Python-3.10.5.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.6.tar.xz",
+        "sha256": "f795ff87d11d4b0c7c33bc8851b0c28648d8a4583aa2100a98c22b4326b6d3f3",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.6/Python-3.10.6.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.7.tar.xz",
+        "sha256": "6eed8415b7516fb2f260906db5d48dd4c06acc0cb24a7d6cc15296a604dcdc48",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.7/Python-3.10.7.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.8.tar.xz",
+        "sha256": "6a30ecde59c47048013eb5a658c9b5dec277203d2793667f578df7671f7f03f3",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.8/Python-3.10.8.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.9.tar.xz",
+        "sha256": "5ae03e308260164baba39921fdb4dbf8e6d03d8235a939d4582b33f0b5e46a83",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.9/Python-3.10.9.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.10.tar.xz",
+        "sha256": "0419e9085bf51b7a672009b3f50dbf1859acdf18ba725d0ec19aa5c8503f0ea3",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.10/Python-3.10.10.tar.xz"
+    },
+    {
+        "dest": "resources/sources",
+        "filename": "Python-3.10.11.tar.xz",
+        "sha256": "3c3bc3048303721c904a03eb8326b631e921f11cc3be2988456a42f115daf04c",
+        "url": "https://mirrors.huaweicloud.com/python/3.10.11/Python-3.10.11.tar.xz"
     }
 ]
```

## ascend_deployer/downloader/requirements.txt

```diff
@@ -20,32 +20,29 @@
 decorator==4.4.2
 distro==1.5.0
 easydict==1.9
 flatbuffers==1.12
 future==0.18.2
 gast==0.2.2
 gast==0.4.0
-gnureadline==8.0.0
+gnureadline==8.1.2
 google-auth-oauthlib==0.4.6
 google-auth==1.35.0
 google-pasta==0.2.0
-grpcio-tools==1.32.0
 grpcio==1.46.1
 h5py==3.1.0
 idna==2.10
 importlib-metadata==4.12.0
 isort==5.8.0
-jinja2==2.11.3
 keras==2.6.0
 keras-applications==1.0.8
 Keras-Preprocessing==1.1.2
 kiwisolver==1.3.1
 lazy-object-proxy==1.6.0
 markdown==3.3.2
-markupsafe==1.1.1
 matplotlib==3.4.0
 mccabe==0.6.1
 mpmath==1.1.0
 numpy==1.14.5
 numpy==1.17.5
 numpy==1.19.2
 numpy==1.19.3
@@ -72,14 +69,15 @@
 pyyaml==5.4.1
 requests-oauthlib==1.3.0
 requests==2.24.0
 rsa==4.7.2
 scipy==1.3.3
 scipy==1.5.4
 selinux==0.2.1
+setuptools==44.1.1
 setuptools==50.3.2
 six==1.15.0
 sympy==1.4
 tensorboard-plugin-wit==1.8.0
 tensorboard==1.15.0
 tensorboard==2.6.0
 tensorboard-data-server==0.6.1
@@ -97,7 +95,13 @@
 zipp==3.4.1
 pytest==6.2.5
 iniconfig==1.1.1
 pluggy==1.0.0
 py==1.10.0
 xlwt==1.3.0
 xlutils==2.0.0
+filelock==3.12.2
+fsspec==2023.12.2
+Jinja2==3.1.2
+MarkupSafe==2.1.3
+networkx==3.0rc1
+typing_extensions==4.8.0
```

## ascend_deployer/downloader/software_mgr.py

```diff
@@ -37,20 +37,21 @@
     @staticmethod
     def _to_type_list(clazz, dict_list: List[Dict]):
         return [clazz(**dic) for dic in (dict_list or [])]
 
 
 class PkgInfo(BaseModel):
 
-    def __init__(self, filename="", url="", sha256="", dest="", python="cp37", *args, **kwargs):
+    def __init__(self, filename="", url="", sha256="", dest="", remark="", python="cp37", *args, **kwargs):
         self.filename = filename
         self.url = url
         self.sha256 = sha256
         self.dest = dest
         self.python = python
+        self.remark = remark
 
 
 class FrameworkWhl(BaseModel):
 
     def __init__(self, system="", whl: List[Dict] = None, *args, **kwargs):
         self.system = system
         self.whl: List[PkgInfo] = self._to_type_list(PkgInfo, whl)
@@ -107,14 +108,15 @@
 
     def __init__(self, unmatch_software_pair: SoftwareMatchPair, support_match_software: SoftwareMatchPair):
         self.unmatch_software = unmatch_software_pair
         self.match_software_pair = support_match_software
 
 
 class SoftwareMgr:
+    DOWNLOADER_PATH = os.path.dirname(os.path.realpath(__file__))
 
     def __init__(self):
         self.all_software_config = self._software_init()
         self.sys_software_list = [software for software in self.all_software_config if software.systems]
         self.framework_whl_list = [software for software in self.all_software_config if software.framework_whl]
         self.other_software_list = [software for software in self.all_software_config if software.other]
 
@@ -194,32 +196,39 @@
         """
         check version matched between CANN and MindSpore
         :param soft_list:download package list
         :return:err_with_exit msg, err_with_ask msg
         """
         item_counter = collections.defaultdict(int)
         version_dict = collections.defaultdict(lambda: "")
+        AI_FRAMEWORK = ("MindSpore", "Torch-npu", "TensorFlow")
+        frameworks = set()
         for soft in soft_list:
             for item in ("DL", "MindSpore", "MindStudio", "Torch-npu", "CANN", "MEF", "TensorFlow", "NPU"):
                 if item not in soft:
                     continue
+                if item in AI_FRAMEWORK:
+                    frameworks.add(item)
                 name_version = self.get_name_version(soft)
                 item_counter[item] += 1
                 version_dict[item] = name_version
                 if item_counter.get(item, 0) > 1:
                     return State.EXIT, "Only one {} is allowed, Please reselect and try again".format(item)
+        if len(frameworks) > 1:
+            return State.EXIT, ("Only one ai framework(MindSpore/Torch/TensorFlow) is allowed due to dependency "
+                                "conflict, Please reselect and try again")
 
         warning_messages = ''
         for name, version in version_dict.items():
             if "CANN" not in version:
                 warning_messages += self.check_cann_matching(version_dict.get("CANN", ""), version)
         versions = [v.split("_")[1] for k, v in version_dict.items() if k in ["DL", "MEF"]]
         for version in versions:
-            support_os_list = os.listdir(
-                os.path.join(os.path.dirname(os.path.realpath(__file__)), f'dependency/{version}/COMMON'))
+            support_os_list = [i.strip(".json") for i in os.listdir(
+                os.path.join(self.DOWNLOADER_PATH, f'dependency/{version}/COMMON_UPDATE'))]
             mef_support_list = ['Ubuntu_20.04_aarch64', 'Ubuntu_20.04_x86_64', 'OpenEuler_22.03LTS_aarch64',
                                 'OpenEuler_22.03LTS_x86_64']
             not_support_list = [i for i in os_list if i.replace('==', '_') not in support_os_list]
             if not_support_list:
                 if item_counter.get('DL', 0) > 0:
                     return State.EXIT, "ascend-deployer do not support install DL on {}".format(not_support_list)
             for os_item in os_list:
@@ -228,18 +237,17 @@
                         mef_support_list)
 
         if warning_messages:
             return State.ASK, warning_messages
 
         return State.NONE, ""
 
-    @staticmethod
-    def check_cann_matching(cann_version, name_version):
+    def check_cann_matching(self, cann_version, name_version):
         warning_message = ""
-        version_match_json = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'version_match.json')
+        version_match_json = os.path.join(self.DOWNLOADER_PATH, 'version_match.json')
         with open(version_match_json, 'r', encoding='utf-8') as json_file:
             version_match_data = json.load(json_file)
         matching_cann = version_match_data.get(name_version)
         if "DL" in name_version and cann_version == "":
             return warning_message
 
         if not cann_version and name_version not in version_match_data.get("NoneMatched", []):
```

## ascend_deployer/downloader/version_match.json

### Pretty-printed

 * *Similarity: 0.7979999999999999%*

 * *Differences: {"'DL_5.0.0'": "'CANN_7.0.0'",*

 * * "'MindSpore_2.2.10'": "'CANN_7.0.0'",*

 * * "'NoneMatched'": "{insert: [(9, 'NPU_23.0.0')]}",*

 * * "'Torch-npu_1.11.0.post8'": "'CANN_7.0.0'",*

 * * "'Torch-npu_2.0.1.post1'": "'CANN_7.0.0'",*

 * * "'Torch-npu_2.1.0'": "'CANN_7.0.0'"}*

```diff
@@ -1,32 +1,38 @@
 {
+    "DL_5.0.0": "CANN_7.0.0",
     "DL_5.0.RC1": "CANN_6.3.RC1",
     "DL_5.0.RC2": "CANN_6.3.RC2",
     "DL_5.0.RC3": "CANN_7.0.RC1",
     "MindSpore_1.10.0": "CANN_6.0.1",
     "MindSpore_1.9.0": "CANN_6.0.RC1",
     "MindSpore_2.0.0rc1": "CANN_6.3.RC1",
     "MindSpore_2.1.0": "CANN_6.3.RC2",
     "MindSpore_2.2.0": "CANN_7.0.RC1",
+    "MindSpore_2.2.10": "CANN_7.0.0",
     "MindStudio_5.0.0": "CANN_6.0.1",
     "MindStudio_5.0.RC3": "CANN_6.0.RC1",
     "MindStudio_6.0.RC1": "CANN_6.3.RC1",
     "MindStudio_6.0.RC2": "CANN_6.3.RC2",
     "NoneMatched": [
         "MEF_5.0.RC1",
         "MEF_5.0.RC2",
         "TensorFlow_1.15.0",
         "TensorFlow_2.6.5",
         "NPU_6.0.0",
         "NPU_6.0.RC1",
         "NPU_23.0.RC1",
         "NPU_23.0.RC2",
-        "NPU_23.0.RC3"
+        "NPU_23.0.RC3",
+        "NPU_23.0.0"
     ],
     "Torch-npu_1.11.0": "CANN_6.3.RC1",
     "Torch-npu_1.11.0.post1": "CANN_6.3.RC2",
     "Torch-npu_1.11.0.post4": "CANN_7.0.RC1",
+    "Torch-npu_1.11.0.post8": "CANN_7.0.0",
     "Torch-npu_1.11.0rc2": "CANN_6.0.1",
     "Torch-npu_1.8.1": "CANN_6.0.1",
     "Torch-npu_1.8.1.post1": "CANN_6.3.RC1",
-    "Torch-npu_1.8.1.post2": "CANN_6.3.RC2"
+    "Torch-npu_1.8.1.post2": "CANN_6.3.RC2",
+    "Torch-npu_2.0.1.post1": "CANN_7.0.0",
+    "Torch-npu_2.1.0": "CANN_7.0.0"
 }
```

## ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {'insert': "[(9, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (23, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm'), "*

 * *           "('sha256', '3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816')])), "*

 * *           "(24, OrderedDict([('name', 'lapack-devel'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/a […]*

```diff
@@ -34,14 +34,18 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
@@ -97,14 +101,24 @@
         "name": "gmp-c++"
     },
     {
         "autodependency": "true",
         "name": "sshpass"
     },
     {
+        "name": "lapack",
+        "sha256": "3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "c102923e6d89af0ab808c256b12d042368d737c37ee5073f9dbab5331fee01a5",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-devel-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
         "name": "inotify-tools",
         "sha256": "0356b062c8d980935fe9120a7899899334cc77c7d46eb6f4e660b9407afba31c",
         "url": "https://mirrors.huaweicloud.com/epel/7/aarch64/Packages/i/inotify-tools-3.14-9.el7.aarch64.rpm"
     },
     {
         "autodependency": "true",
         "name": "fuse3"
```

## ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.3795620437956204%*

 * *Differences: {'10': "{'name': 'perl-HTTP-Tiny'}",*

 * * '11': "{'name': 'perl-PathTools'}",*

 * * '12': "{'name': 'perl-Pod-Escapes'}",*

 * * '13': "{'name': 'perl-Pod-Perldoc'}",*

 * * '14': "{'name': 'perl-Pod-Simple'}",*

 * * '15': "{'name': 'perl-Pod-Usage'}",*

 * * '16': "{'name': 'perl-Scalar-List-Utils'}",*

 * * '17': "{'name': 'perl-Socket'}",*

 * * '18': "{'name': 'perl-Storable'}",*

 * * '19': "{'name': 'perl-Text-ParseWords'}",*

 * * '2': "{'name': 'perl'}",*

 * * '20': "{'name': 'perl-Time-HiRes'}",*

 * * '21': "{'name': 'perl-Time-Local'}",*

 * * '22': "{'name': 'perl-co […]*

```diff
@@ -6,548 +6,411 @@
     },
     {
         "name": "kernel-devel",
         "sha256": "d0f711e1ea4006b4ebeb0c0b55b5db4561730c0d0243659e6597ae9f5cc4e1bc",
         "url": "https://mirrors.bfsu.edu.cn/centos-vault/altarch/7.6.1810/os/aarch64/Packages/kernel-devel-4.14.0-115.el7a.0.1.aarch64.rpm"
     },
     {
-        "name": "openssl",
-        "sha256": "cf10392c322c02c017b9f127102d45c91825af4c4edf21d2ae727fa1d8fc84c2",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/aarch64/os/Packages/openssl-1.1.1c-15.el8.aarch64.rpm"
-    },
-    {
-        "name": "openssl-libs",
-        "sha256": "e25209f9c272a5407ed0d8397e6f8ce8d6de1bb3a6186b06d23ec1533d19d18a",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/aarch64/os/Packages/openssl-libs-1.1.1c-15.el8.aarch64.rpm"
-    },
-    {
-        "name": "openssl-devel",
-        "sha256": "d44d32917756f320b9a2a441723901c61a941fc690e542499c371a8bec6f73f5",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/aarch64/os/Packages/openssl-devel-1.1.1c-15.el8.aarch64.rpm"
-    },
-    {
-        "name": "kernel-headers"
-    },
-    {
-        "name": "kernel-devel"
-    },
-    {
-        "name": "kernel-debug-devel"
-    },
-    {
-        "name": "openssl"
-    },
-    {
-        "name": "openssl-libs"
-    },
-    {
-        "name": "openssl-devel"
-    },
-    {
-        "name": "docker-ce-cli",
-        "release": "3.el7",
-        "version": "20.10.8"
-    },
-    {
-        "name": "containerd.io",
-        "release": "3.1.el7",
-        "version": "1.4.9"
-    },
-    {
-        "name": "docker-ce-rootless-extras",
-        "release": "3.el7",
-        "version": "20.10.8"
-    },
-    {
-        "name": "docker-ce",
-        "release": "3.el7",
-        "version": "20.10.8"
-    },
-    {
-        "name": "dkms",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "elfutils-libelf",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "elfutils-libelf-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "elfutils",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "elfutils-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "cpp",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "glibc-common",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "glibc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "glibc-headers",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "glibc-devel",
+        "name": "perl",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgcc",
+        "name": "perl-Carp",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgomp",
+        "name": "perl-Encode",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc",
+        "name": "perl-Exporter",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libstdc++",
+        "name": "perl-File-Path",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libstdc++-devel",
+        "name": "perl-File-Temp",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc-c++",
+        "name": "perl-Filter",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc-gfortran",
+        "name": "perl-Getopt-Long",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgfortran",
+        "name": "perl-HTTP-Tiny",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "make",
+        "name": "perl-PathTools",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libuv",
+        "name": "perl-Pod-Escapes",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "rhash",
+        "name": "perl-Pod-Perldoc",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-libs",
+        "name": "perl-Pod-Simple",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-pip",
+        "name": "perl-Pod-Usage",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-setuptools",
+        "name": "perl-Scalar-List-Utils",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3",
+        "name": "perl-Socket",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "unzip",
+        "name": "perl-Storable",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "bzip2",
+        "name": "perl-Text-ParseWords",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "zlib",
+        "name": "perl-Time-HiRes",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "zlib-devel",
+        "name": "perl-Time-Local",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libaec-devel",
+        "name": "perl-constant",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libaec",
+        "name": "perl-libs",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "hdf5-devel",
+        "name": "perl-macros",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "hdf5",
+        "name": "perl-parent",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libffi",
+        "name": "perl-podlators",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libffi-devel",
+        "name": "perl-threads",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "keyutils-libs",
+        "name": "perl-threads-shared",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "keyutils-libs-devel",
+        "name": "haveged",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libcom_err",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "gcc",
+        "sha256": "0a713c33643bf92a1986b45677f76c0fc0026991a0daa60820661cf61477cb17",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/gcc-7.3.0-1.el7.aarch64.rpm"
     },
     {
-        "name": "libcom_err-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "openssl11",
+        "sha256": "92c8ee0d5717ee724beef7560bf6290a47952a268c16bbe9a6c00741e0e362e7",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/openssl11-1.1.1w-1.el7.aarch64.rpm"
     },
     {
-        "name": "libselinux",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "openssl11-devel",
+        "sha256": "cf2ff754cea2753a29a188ebec685df65d7d54c53b80f7108bff9014ceaac700",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/openssl11-devel-1.1.1w-1.el7.aarch64.rpm"
     },
     {
-        "name": "libselinux-devel",
+        "name": "perl-WWW-Curl",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libkadm5",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "dkms",
+        "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
     },
     {
-        "name": "krb5-libs",
+        "name": "make",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "krb5-devel",
+        "name": "glibc-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "pcre-devel",
+        "name": "glibc-headers",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "sqlite",
+        "name": "glibc",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "sqlite-devel",
+        "name": "glibc-common",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "lapack",
+        "name": "unzip",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "blas",
+        "name": "bzip2",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "blas-devel",
+        "name": "hdf5",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-openmp",
+        "name": "libaec",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-openmp64",
+        "name": "libgfortran",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-openmp64_",
+        "name": "hdf5-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-serial",
+        "name": "libaec-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-serial64",
+        "name": "zlib-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-serial64_",
+        "name": "libffi",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-threads",
+        "name": "libffi-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-threads64",
+        "name": "sqlite",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-threads64_",
+        "name": "sqlite-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas",
+        "name": "blas",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "openblas-devel",
+        "name": "lapack",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
@@ -555,150 +418,30 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "pciutils-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "net-tools",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "lapack-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "pkgconfig",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libverto",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libverto-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libsepol",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libsepol-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "sshpass",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libmpc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "mpfr",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libarchive",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "emacs-filesystem",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "hwdata",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libtirpc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libselinux-python",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libselinux-utils",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "xz-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
@@ -707,303 +450,124 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "e2fsprogs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "e2fsprogs-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libss",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "iputils",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
-        "name": "inotify-tools",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
-        "name": "gzip",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
-        "name": "tcl",
-        "used_by": [
-            "expect"
-        ]
-    },
-    {
-        "name": "expect",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
-        "name": "iptables",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
-        "name": "ethtool",
-        "used_by": [
-            "edge",
-            "ha"
-        ]
-    },
-    {
         "name": "libseccomp",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "perl",
+        "name": "xz",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "perl-Carp",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "container-selinux",
+        "sha256": "5abc3b8b14690561ed0d8027eaafd12f680abf59fde3603a7732a7ce37b3fa21",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/container-selinux-2.107-3.el7.noarch.rpm"
     },
     {
-        "name": "perl-Encode",
+        "name": "audit-libs-python",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-Exporter",
+        "name": "checkpolicy",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-File-Path",
+        "name": "libcgroup",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-File-Temp",
+        "name": "libsemanage-python",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-Filter",
+        "name": "policycoreutils-python",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-Getopt-Long",
+        "name": "python-IPy",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-HTTP-Tiny",
+        "name": "setools-libs",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-PathTools",
+        "name": "audit",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Escapes",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Perldoc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Simple",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Usage",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Scalar-List-Utils",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Socket",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Storable",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Text-ParseWords",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-Time-HiRes",
+        "name": "audit-libs",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-Time-Local",
+        "name": "policycoreutils",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-constant",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "fuse-overlayfs",
+        "sha256": "b2e2cd07c7d4fe8b497537b963ca89e90d047b6142dafd7ba0fce5d3c0342b85",
+        "url": "https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/Packages/fuse-overlayfs-0.7.2-6.el7_8.aarch64.rpm"
     },
     {
-        "name": "perl-libs",
+        "name": "fuse3-libs",
         "used_by": [
-            "driver",
-            "cann",
-            "framework"
+            "docker"
         ]
     },
     {
-        "name": "perl-macros",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "slirp4netns",
+        "sha256": "c3d964fa9cb020cee2efdce3688ef075734b14bf1dd6fde036117d1914d23c3a",
+        "url": "https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/Packages/slirp4netns-0.4.3-4.el7_8.aarch64.rpm"
     },
     {
-        "name": "perl-parent",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "docker-ce-cli",
+        "release": "3.el7",
+        "version": "20.10.8"
     },
     {
-        "name": "perl-podlators",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "containerd.io",
+        "release": "3.1.el7",
+        "version": "1.4.9"
     },
     {
-        "name": "perl-threads",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "docker-ce-rootless-extras",
+        "release": "3.el7",
+        "version": "20.10.8"
     },
     {
-        "name": "perl-threads-shared",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "docker-ce",
+        "release": "3.el7",
+        "version": "20.10.8"
     }
 ]
```

## ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.4261744966442953%*

 * *Differences: {'10': "{'name': 'perl-HTTP-Tiny'}",*

 * * '11': "{'name': 'perl-PathTools'}",*

 * * '12': "{'name': 'perl-Pod-Escapes'}",*

 * * '13': "{'name': 'perl-Pod-Perldoc'}",*

 * * '14': "{'name': 'perl-Pod-Simple'}",*

 * * '15': "{'name': 'perl-Pod-Usage'}",*

 * * '16': "{'name': 'perl-Scalar-List-Utils'}",*

 * * '17': "{'name': 'perl-Socket'}",*

 * * '18': "{'name': 'perl-Storable'}",*

 * * '19': "{'name': 'perl-Text-ParseWords'}",*

 * * '2': "{'name': 'perl'}",*

 * * '20': "{'name': 'perl-Time-HiRes'}",*

 * * '21': "{'name': 'perl-Time-Local'}",*

 * * '22': "{'name': 'perl-co […]*

```diff
@@ -6,448 +6,403 @@
     },
     {
         "name": "kernel-devel",
         "sha256": "34e1ef62c789ba68fc7332eab68b812b7bbe625071a2020d5e04cb5441d3e548",
         "url": "https://mirrors.huaweicloud.com/centos-vault/7.6.1810/os/x86_64/Packages/kernel-devel-3.10.0-957.el7.x86_64.rpm"
     },
     {
-        "name": "openssl",
-        "sha256": "0ea161cbcbbf5db609bb4d7524750c0a6e57dc279282aa021aabf63a7cc63e79",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/x86_64/os/Packages/openssl-1.1.1c-15.el8.x86_64.rpm"
-    },
-    {
-        "name": "openssl-libs",
-        "sha256": "212def76c7dcc2cc8422b9ebcb9a485050c32f68cebabf66012bca3936cf79c3",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/x86_64/os/Packages/openssl-libs-1.1.1c-15.el8.x86_64.rpm"
-    },
-    {
-        "name": "openssl-devel",
-        "sha256": "7c1cdec5e46fb029dc086cc88d6467674acaf8f1b7fb70f11f109d7acb85d6ac",
-        "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/x86_64/os/Packages/openssl-devel-1.1.1c-15.el8.x86_64.rpm"
-    },
-    {
-        "name": "kernel-headers"
-    },
-    {
-        "name": "kernel-devel"
-    },
-    {
-        "name": "kernel-debug-devel"
-    },
-    {
-        "name": "openssl"
-    },
-    {
-        "name": "openssl-libs"
-    },
-    {
-        "name": "openssl-devel"
-    },
-    {
-        "name": "dkms",
+        "name": "perl",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "elfutils-libelf",
+        "name": "perl-Carp",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "elfutils-libelf-devel",
+        "name": "perl-Encode",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "elfutils",
+        "name": "perl-Exporter",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "elfutils-libs",
+        "name": "perl-File-Path",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "cpp",
+        "name": "perl-File-Temp",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "glibc-common",
+        "name": "perl-Filter",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "glibc",
+        "name": "perl-Getopt-Long",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "glibc-headers",
+        "name": "perl-HTTP-Tiny",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "glibc-devel",
+        "name": "perl-PathTools",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgcc",
+        "name": "perl-Pod-Escapes",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgomp",
+        "name": "perl-Pod-Perldoc",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc",
+        "name": "perl-Pod-Simple",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libquadmath",
+        "name": "perl-Pod-Usage",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libquadmath-devel",
+        "name": "perl-Scalar-List-Utils",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libstdc++",
+        "name": "perl-Socket",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libstdc++-devel",
+        "name": "perl-Storable",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc-c++",
+        "name": "perl-Text-ParseWords",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "gcc-gfortran",
+        "name": "perl-Time-HiRes",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libgfortran",
+        "name": "perl-Time-Local",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "make",
+        "name": "perl-constant",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libuv",
+        "name": "perl-libs",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "rhash",
+        "name": "perl-macros",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-libs",
+        "name": "perl-parent",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-pip",
+        "name": "perl-podlators",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3-setuptools",
+        "name": "perl-threads",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "python3",
+        "name": "perl-threads-shared",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libzstd",
+        "name": "haveged",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "unzip",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "gcc",
+        "sha256": "1878cce561d57714a0e1510378dc3af325790f29a5c9d1809a25f4bbc57ecab3",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/gcc-7.3.0-1.el7.x86_64.rpm"
     },
     {
-        "name": "bzip2",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "openssl11",
+        "sha256": "36d493058ecd41edae7c4ec252420d95d7eb3acc6f7a133c846f273d5c100454",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/openssl11-1.1.1w-1.el7.x86_64.rpm"
     },
     {
-        "name": "zlib",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "openssl11-devel",
+        "sha256": "1e852a4481f2665f9f82bf90b092a1624c91eed752ca46e43b5cd77af82cbcdb",
+        "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/packages/openssl11-devel-1.1.1w-1.el7.x86_64.rpm"
     },
     {
-        "name": "zlib-devel",
+        "name": "perl-WWW-Curl",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libaec-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "dkms",
+        "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
+        "url": "https://mirrors.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/dkms-2.6.1-5.oe1.noarch.rpm"
     },
     {
-        "name": "libaec",
+        "name": "make",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "hdf5-devel",
+        "name": "glibc-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "hdf5",
+        "name": "glibc-headers",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libffi",
+        "name": "glibc",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libffi-devel",
+        "name": "glibc-common",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "keyutils-libs",
+        "name": "unzip",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "keyutils-libs-devel",
+        "name": "bzip2",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libcom_err",
+        "name": "hdf5",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libcom_err-devel",
+        "name": "libaec",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libselinux",
+        "name": "libgfortran",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libselinux-devel",
+        "name": "libquadmath",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libkadm5",
+        "name": "hdf5-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "krb5-libs",
+        "name": "libaec-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "krb5-devel",
+        "name": "zlib-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "pcre-devel",
+        "name": "libffi",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "sqlite",
+        "name": "libffi-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "sqlite-devel",
+        "name": "sqlite",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "lapack",
+        "name": "sqlite-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
@@ -455,103 +410,15 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "blas-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-openmp",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-openmp64",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-openmp64_",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-serial",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-serial64",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-serial64_",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-threads",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-threads64",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-threads64_",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "openblas-devel",
+        "name": "lapack",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
@@ -559,142 +426,30 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "pciutils-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "net-tools",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "lapack-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "pkgconfig",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libverto",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libverto-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libsepol",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libsepol-devel",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "sshpass",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "libmpc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "mpfr",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libarchive",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "emacs-filesystem",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "hwdata",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libtirpc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libselinux-python",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "xz-devel",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
@@ -711,87 +466,40 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "e2fsprogs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "e2fsprogs-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libselinux-utils",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "libss",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
         "name": "xz",
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
-        "name": "xz-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
+        "name": "container-selinux",
+        "sha256": "5abc3b8b14690561ed0d8027eaafd12f680abf59fde3603a7732a7ce37b3fa21",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/container-selinux-2.107-3.el7.noarch.rpm"
     },
     {
         "name": "audit-libs-python",
         "used_by": [
             "docker"
         ]
     },
     {
         "name": "checkpolicy",
         "used_by": [
             "docker"
         ]
     },
     {
-        "name": "container-selinux",
-        "used_by": [
-            "docker"
-        ]
-    },
-    {
-        "name": "fuse-overlayfs",
-        "used_by": [
-            "docker"
-        ]
-    },
-    {
-        "name": "fuse3-libs",
+        "name": "libcgroup",
         "used_by": [
             "docker"
         ]
     },
     {
         "name": "libsemanage-python",
         "used_by": [
@@ -831,15 +539,20 @@
     {
         "name": "policycoreutils",
         "used_by": [
             "docker"
         ]
     },
     {
-        "name": "libcgroup",
+        "name": "fuse-overlayfs",
+        "sha256": "8e70be781ade8fcc4f4457275bba3babf7c88bf7bb8d3e37894ee0d4367bbf7b",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/fuse-overlayfs-0.7.2-6.el7_8.x86_64.rpm"
+    },
+    {
+        "name": "fuse3-libs",
         "used_by": [
             "docker"
         ]
     },
     {
         "name": "slirp4netns",
         "sha256": "b98eb2c09940f8fb40405c0fd310bfa2ebc8f2e5e2711df564b35db06d027286",
@@ -865,225 +578,9 @@
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "docker-scan-plugin",
         "release": "3.el7",
         "version": "0.23.0"
-    },
-    {
-        "name": "perl",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Carp",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Encode",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Exporter",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-File-Path",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-File-Temp",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Filter",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Getopt-Long",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-HTTP-Tiny",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-PathTools",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Escapes",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Perldoc",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Simple",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Pod-Usage",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Scalar-List-Utils",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Socket",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Storable",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Text-ParseWords",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Time-HiRes",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-Time-Local",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-constant",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-libs",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-macros",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-parent",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-podlators",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-threads",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
-    },
-    {
-        "name": "perl-threads-shared",
-        "used_by": [
-            "driver",
-            "cann",
-            "framework"
-        ]
     }
 ]
```

## ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo

```diff
@@ -1,14 +1,8 @@
-[extra]
-baseurl=https://mirrors.huaweicloud.com/centos/7/extras/x86_64/
-
 [base]
 baseurl=https://mirrors.huaweicloud.com/centos/7/os/x86_64/
 
 [epel]
 baseurl=https://mirrors.huaweicloud.com/epel/7/x86_64/
 
-[update]
-baseurl=https://mirrors.huaweicloud.com/centos/7/updates/x86_64/
-
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/x86_64/stable/
```

## ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9298245614035088%*

 * *Differences: {'insert': "[(13, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (14, "*

 * *           "OrderedDict([('name', 'libtool-ltdl'), ('autodependency', 'true')])), (31, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm'), "*

 * *           "('sha256', '3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816')])), "*

 * *           "(32, OrderedDict([('name', 'lapack-devel […]*

```diff
@@ -62,14 +62,22 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
+        "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "libtool-ltdl"
+    },
+    {
         "info": "need upgrade to match the new openssl form repo",
         "name": "gnutls",
         "release": "6.h7.eulerosv2r10",
         "version": "3.6.14"
     },
     {
         "name": "openblas",
@@ -144,14 +152,24 @@
     },
     {
         "autodependency": "true",
         "info": "used for driver maybe",
         "name": "elfutils-devel"
     },
     {
+        "name": "lapack",
+        "sha256": "3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "c102923e6d89af0ab808c256b12d042368d737c37ee5073f9dbab5331fee01a5",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-devel-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
         "name": "dkms",
         "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
```

## ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {'insert': "[(12, OrderedDict([('name', 'libtool-ltdl'), ('autodependency', 'true')])), (20, "*

 * *           "OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (38, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-3.8.0-16.oe1.x86_64.rpm'), "*

 * *           "('sha256', '3a0823530c69342be29666e9b199795e1461cdceaa1db1f082ec4f59112664ed')])), "*

 * *           "(39, OrderedDict([('name', 'lapack-devel') […]*

```diff
@@ -56,14 +56,18 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
+        "autodependency": "true",
+        "name": "libtool-ltdl"
+    },
+    {
         "info": "need upgrade to match the new openssl form repo",
         "name": "gnutls",
         "release": "6.h7.eulerosv2r10",
         "version": "3.6.14"
     },
     {
         "name": "openblas",
@@ -94,14 +98,18 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
         "name": "libgomp"
     },
     {
         "autodependency": "true",
         "name": "gcc-gfortran"
     },
     {
@@ -183,14 +191,24 @@
     },
     {
         "autodependency": "true",
         "info": "used for driver maybe",
         "name": "elfutils-devel"
     },
     {
+        "name": "lapack",
+        "sha256": "3a0823530c69342be29666e9b199795e1461cdceaa1db1f082ec4f59112664ed",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-3.8.0-16.oe1.x86_64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "ab8af42c808ab7ba076ca5c4a6421b81486834ac524d83856e32c3090254ba1f",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-devel-3.8.0-16.oe1.x86_64.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
     },
     {
         "name": "dkms",
         "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
```

## ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9550561797752809%*

 * *Differences: {'insert': "[(33, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (34, "*

 * *           "OrderedDict([('name', 'libtool-ltdl'), ('autodependency', 'true')])), (52, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm'), "*

 * *           "('sha256', '3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816')])), "*

 * *           "(53, OrderedDict([('name', 'lapack-devel […]*

```diff
@@ -184,14 +184,22 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
+        "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "libtool-ltdl"
+    },
+    {
         "info": "need upgrade to match the new openssl form repo",
         "name": "gnutls",
         "release": "1.h11.eulerosv2r8",
         "version": "3.6.7"
     },
     {
         "name": "openblas",
@@ -272,14 +280,24 @@
     },
     {
         "autodependency": "true",
         "info": "python and gnureadline",
         "name": "ncurses-devel"
     },
     {
+        "name": "lapack",
+        "sha256": "3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "c102923e6d89af0ab808c256b12d042368d737c37ee5073f9dbab5331fee01a5",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-devel-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
         "name": "dkms",
         "sha256": "c8d63b95ec9d4379bdaeef0067ff6f880a7f6d0f18d96dc3deda48e791a8c780",
```

## ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9487179487179487%*

 * *Differences: {'insert': "[(29, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (30, "*

 * *           "OrderedDict([('name', 'libtool-ltdl'), ('autodependency', 'true')])), (59, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm'), "*

 * *           "('sha256', '3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816')])), "*

 * *           "(60, OrderedDict([('name', 'lapack-devel […]*

```diff
@@ -160,14 +160,22 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
+        "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "libtool-ltdl"
+    },
+    {
         "info": "need upgrade to match the new openssl form repo",
         "name": "gnutls",
         "release": "6.h12.eulerosv2r9",
         "version": "3.6.9"
     },
     {
         "name": "openblas",
@@ -316,14 +324,24 @@
     },
     {
         "autodependency": "true",
         "info": "python gnureadline",
         "name": "ncurses-devel"
     },
     {
+        "name": "lapack",
+        "sha256": "3987d07d3c93259344f06ce690d4fd4456539dc41895ceb6af5fb652475d6816",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "c102923e6d89af0ab808c256b12d042368d737c37ee5073f9dbab5331fee01a5",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/Packages/lapack-devel-3.8.0-16.oe1.aarch64.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
     },
     {
         "name": "dkms",
         "sha256": "c8d63b95ec9d4379bdaeef0067ff6f880a7f6d0f18d96dc3deda48e791a8c780",
```

## ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9452054794520548%*

 * *Differences: {'insert': "[(31, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (32, "*

 * *           "OrderedDict([('name', 'libtool-ltdl'), ('autodependency', 'true')])), (63, "*

 * *           "OrderedDict([('name', 'lapack'), ('url', "*

 * *           "'https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-3.8.0-16.oe1.x86_64.rpm'), "*

 * *           "('sha256', '3a0823530c69342be29666e9b199795e1461cdceaa1db1f082ec4f59112664ed')])), "*

 * *           "(64, OrderedDict([('name', 'lapack-devel') […]*

```diff
@@ -172,14 +172,22 @@
         "name": "cmake"
     },
     {
         "autodependency": "true",
         "name": "unzip"
     },
     {
+        "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "libtool-ltdl"
+    },
+    {
         "info": "need upgrade to match the new openssl form repo",
         "name": "gnutls",
         "release": "6.h12.eulerosv2r9",
         "version": "3.6.9"
     },
     {
         "name": "openblas",
@@ -338,14 +346,24 @@
     },
     {
         "autodependency": "true",
         "info": "used for driver maybe",
         "name": "elfutils-devel"
     },
     {
+        "name": "lapack",
+        "sha256": "3a0823530c69342be29666e9b199795e1461cdceaa1db1f082ec4f59112664ed",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-3.8.0-16.oe1.x86_64.rpm"
+    },
+    {
+        "name": "lapack-devel",
+        "sha256": "ab8af42c808ab7ba076ca5c4a6421b81486834ac524d83856e32c3090254ba1f",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/Packages/lapack-devel-3.8.0-16.oe1.x86_64.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
     },
     {
         "name": "dkms",
         "sha256": "4b31e97ff478c39228785acbbd702ca69fa2e498c2ad710b130049463fd21928",
```

## ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9210526315789473%*

 * *Differences: {'insert': "[(12, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (13, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (14, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -47,14 +47,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8897058823529411%*

 * *Differences: {'23': "{'autodependency': 'true', delete: ['url', 'sha256']}",*

 * * 'insert': "[(9, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (10, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -35,14 +35,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
@@ -89,17 +101,16 @@
     },
     {
         "autodependency": "true",
         "info": "used for mindspore",
         "name": "gmp-c++"
     },
     {
-        "name": "sshpass",
-        "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
-        "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
+        "autodependency": "true",
+        "name": "sshpass"
     },
     {
         "name": "inotify-tools",
         "sha256": "eb4df7f1af81cde3f559800543a052e98f61fec87500742612c689c0329355c6",
         "url": "https://mirrors.huaweicloud.com/epel/8/Everything/aarch64/Packages/i/inotify-tools-3.14-19.el8.aarch64.rpm"
     },
     {
```

## ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo

```diff
@@ -1,8 +1,8 @@
 [base]
-baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/
+baseurl = https://update.cs2c.com.cn/NS/V10/V10SP1/os/adv/lic/base/aarch64/
 
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/aarch64/stable/
 
 [extra]
 baseurl=https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/
```

## ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8863636363636364%*

 * *Differences: {'23': "{'autodependency': 'true', delete: ['url', 'sha256']}",*

 * * 'insert': "[(9, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (10, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -35,14 +35,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
@@ -89,17 +101,16 @@
     },
     {
         "autodependency": "true",
         "info": "docker need",
         "name": "libcgroup"
     },
     {
-        "name": "sshpass",
-        "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
-        "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
+        "autodependency": "true",
+        "name": "sshpass"
     },
     {
         "info": "docker need",
         "name": "slirp4netns",
         "release": "4.el7_8",
         "version": "0.4.3"
     },
```

## ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo

```diff
@@ -1,8 +1,8 @@
 [base]
-baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/
+baseurl = https://update.cs2c.com.cn/NS/V10/V10SP1/os/adv/lic/base/x86_64/
 
 [extra]
 baseurl=https://mirrors.huaweicloud.com/centos/7/extras/x86_64/
 
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/x86_64/stable/
```

## ascend_deployer/downloader/config/Kylin_V10_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9117647058823529%*

 * *Differences: {'insert': "[(9, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (10, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -35,14 +35,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9142857142857143%*

 * *Differences: {'insert': "[(10, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (12, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -39,14 +39,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.926829268292683%*

 * *Differences: {'insert': "[(10, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (12, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -39,14 +39,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.921875%*

 * *Differences: {'insert': "[(1, OrderedDict([('name', 'readline-devel'), ('autodependency', 'true')])), (2, "*

 * *           "OrderedDict([('name', 'ncurses-devel'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (12, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (13, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -1,14 +1,22 @@
 [
     {
         "autodependency": "true",
         "name": "tar"
     },
     {
         "autodependency": "true",
+        "name": "readline-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "ncurses-devel"
+    },
+    {
+        "autodependency": "true",
         "name": "python3-libselinux"
     },
     {
         "autodependency": "true",
         "name": "gcc"
     },
     {
@@ -35,14 +43,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.90625%*

 * *Differences: {'insert': "[(9, OrderedDict([('name', 'haveged'), ('autodependency', 'true')])), (10, "*

 * *           "OrderedDict([('name', 'lapack'), ('autodependency', 'true')])), (11, "*

 * *           "OrderedDict([('name', 'lapack-devel'), ('autodependency', 'true')]))]"}*

```diff
@@ -35,14 +35,26 @@
     },
     {
         "autodependency": "true",
         "name": "net-tools"
     },
     {
         "autodependency": "true",
+        "name": "haveged"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack"
+    },
+    {
+        "autodependency": "true",
+        "name": "lapack-devel"
+    },
+    {
+        "autodependency": "true",
         "info": "python cffi",
         "name": "libffi-devel"
     },
     {
         "autodependency": "true",
         "info": "python zlib",
         "name": "zlib-devel"
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt

```diff
@@ -1,3561 +0,0 @@
-00000000: 4d6f 6465 6d4d 616e 6167 6572 2d67 6c69  ModemManager-gli
-00000010: 622e 6161 7263 6836 3420 2020 2020 2020  b.aarch64       
-00000020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000030: 2020 2020 2020 312e 3134 2e30 2d32 2e75        1.14.0-2.u
-00000040: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00000050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000060: 2040 616e 6163 6f6e 6461 0a4e 6574 776f   @anaconda.Netwo
-00000070: 726b 4d61 6e61 6765 722e 6161 7263 6836  rkManager.aarch6
-00000080: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00000090: 2020 2020 2020 2020 2020 2020 2020 313a                1:
-000000a0: 312e 3236 2e32 2d35 2e75 7032 2e75 656c  1.26.2-5.up2.uel
-000000b0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-000000c0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-000000d0: 616e 6163 6f6e 6461 0a4e 6574 776f 726b  anaconda.Network
-000000e0: 4d61 6e61 6765 722d 636f 6e66 6967 2d73  Manager-config-s
-000000f0: 6572 7665 722e 6e6f 6172 6368 2020 2020  erver.noarch    
-00000100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000110: 2020 2020 2020 2020 2031 3a31 2e32 362e           1:1.26.
-00000120: 322d 352e 7570 322e 7565 6c32 3020 2020  2-5.up2.uel20   
-00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000140: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00000150: 6e64 610a 4e65 7477 6f72 6b4d 616e 6167  nda.NetworkManag
-00000160: 6572 2d68 656c 702e 6e6f 6172 6368 2020  er-help.noarch  
-00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000180: 2020 2020 2020 2020 2020 2031 3a31 2e32             1:1.2
-00000190: 362e 322d 352e 7570 322e 7565 6c32 3020  6.2-5.up2.uel20 
-000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001b0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-000001c0: 636f 6e64 610a 4e65 7477 6f72 6b4d 616e  conda.NetworkMan
-000001d0: 6167 6572 2d6c 6962 6e6d 2e61 6172 6368  ager-libnm.aarch
-000001e0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000001f0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00000200: 3a31 2e32 362e 322d 352e 7570 322e 7565  :1.26.2-5.up2.ue
-00000210: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000230: 4061 6e61 636f 6e64 610a 556e 696f 6e54  @anaconda.UnionT
-00000240: 6563 682d 6770 672d 6b65 7973 2e61 6172  ech-gpg-keys.aar
-00000250: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000270: 2031 2e30 2d33 2e34 2e75 656c 3230 2020   1.0-3.4.uel20  
-00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000290: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000002a0: 6f6e 6461 0a55 6e69 6f6e 5465 6368 2d6c  onda.UnionTech-l
-000002b0: 6174 6573 742d 7265 6c65 6173 652e 6161  atest-release.aa
-000002c0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002e0: 2020 312e 302d 3136 3236 3831 3031 3639    1.0-1626810169
-000002f0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2040 616e 6163 6f6e 6461 0a55 6e69     @anaconda.Uni
-00000320: 6f6e 5465 6368 2d6c 6f67 6f73 2e6e 6f61  onTech-logos.noa
-00000330: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000350: 312e 302d 392e 7570 342e 7565 6c32 3020  1.0-9.up4.uel20 
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00000380: 636f 6e64 610a 556e 696f 6e54 6563 682d  conda.UnionTech-
-00000390: 6c73 622e 6161 7263 6836 3420 2020 2020  lsb.aarch64     
-000003a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003b0: 2020 2020 2020 2020 352e 302d 312e 7570          5.0-1.up
-000003c0: 332e 7565 6c32 3020 2020 2020 2020 2020  3.uel20         
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 4061 6e61 636f 6e64 610a 556e      @anaconda.Un
-000003f0: 696f 6e54 6563 682d 7065 7266 6f72 6d61  ionTech-performa
-00000400: 6e63 652e 6161 7263 6836 3420 2020 2020  nce.aarch64     
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 2020 2020 2020 2020 3130 3230 2d32 2e31          1020-2.1
-00000430: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2040 616e 6163 6f6e 6461 0a55 6e69     @anaconda.Uni
-00000460: 6f6e 5465 6368 2d72 656c 6561 7365 2e61  onTech-release.a
-00000470: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000490: 2020 2031 3032 302d 322e 312e 7565 6c32     1020-2.1.uel2
-000004a0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000004b0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000004c0: 6e61 636f 6e64 610a 556e 696f 6e54 6563  naconda.UnionTec
-000004d0: 682d 7265 706f 696e 666f 2e61 6172 6368  h-repoinfo.aarch
-000004e0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000004f0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00000500: 2e30 2d31 2e75 656c 3230 2020 2020 2020  .0-1.uel20      
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00000530: 0a55 6e69 6f6e 5465 6368 2d72 6570 6f73  .UnionTech-repos
-00000540: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2020 2031 2e30 2d33 2e34 2e75 656c       1.0-3.4.uel
-00000570: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00000580: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00000590: 616e 6163 6f6e 6461 0a55 6e69 6f6e 5465  anaconda.UnionTe
-000005a0: 6368 2d72 706d 2d63 6f6e 6669 672e 6161  ch-rpm-config.aa
-000005b0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 3330 2d31 332e 7570 352e 7565 6c32    30-13.up5.uel2
-000005e0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000005f0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00000600: 6e61 636f 6e64 610a 6162 6174 7469 732d  naconda.abattis-
-00000610: 6361 6e74 6172 656c 6c2d 666f 6e74 732e  cantarell-fonts.
-00000620: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2030 2e32 3031 2d31 2e75 656c 3230     0.201-1.uel20
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00000670: 6163 6f6e 6461 0a61 636c 2e61 6172 6368  aconda.acl.aarch
-00000680: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00000690: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-000006a0: 2e32 2e35 332d 382e 7565 6c32 3020 2020  .2.53-8.uel20   
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006c0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000006d0: 6e64 610a 6164 7761 6974 612d 6963 6f6e  nda.adwaita-icon
-000006e0: 2d74 6865 6d65 2e6e 6f61 7263 6820 2020  -theme.noarch   
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2020 2020 332e 3337 2e32            3.37.2
-00000710: 2d32 2e75 656c 3230 2020 2020 2020 2020  -2.uel20        
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2020 2040 616e 6163 6f6e 6461 0a61       @anaconda.a
-00000740: 742d 7370 6932 2d61 746b 2e61 6172 6368  t-spi2-atk.aarch
-00000750: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00000760: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00000770: 2e33 342e 322d 312e 7565 6c32 3020 2020  .34.2-1.uel20   
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000007a0: 6e64 610a 6174 2d73 7069 322d 636f 7265  nda.at-spi2-core
-000007b0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2020 2032 2e33 362e 302d 312e 7565       2.36.0-1.ue
-000007e0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000800: 4061 6e61 636f 6e64 610a 6174 6b2e 6161  @anaconda.atk.aa
-00000810: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 2020 322e 3336 2e30 2d31 2e75 656c 3230    2.36.0-1.uel20
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00000860: 6163 6f6e 6461 0a61 7474 722e 6161 7263  aconda.attr.aarc
-00000870: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 322e 342e 3438 2d31 332e 7570 312e 7565  2.4.48-13.up1.ue
-000008a0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 4061 6e61 636f 6e64 610a 6175 6469 742e  @anaconda.audit.
-000008d0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 313a 332e 302d 332e 7565 6c32      1:3.0-3.uel2
-00000900: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00000910: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00000920: 6e61 636f 6e64 610a 6175 6469 742d 6c69  naconda.audit-li
-00000930: 6273 2e61 6172 6368 3634 2020 2020 2020  bs.aarch64      
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 2020 2020 2031 3a33 2e30 2d33 2e75         1:3.0-3.u
-00000960: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2040 616e 6163 6f6e 6461 0a61 7574 6873   @anaconda.auths
-00000990: 656c 6563 742e 6161 7263 6836 3420 2020  elect.aarch64   
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 2020 312e 322e 312d            1.2.1-
-000009c0: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 4061 6e61 636f 6e64 610a 6175      @anaconda.au
-000009f0: 746f 6765 6e2e 6161 7263 6836 3420 2020  togen.aarch64   
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2020 2020 2020 352e 3138 2e31            5.18.1
-00000a20: 362d 312e 7565 6c32 3020 2020 2020 2020  6-1.uel20       
-00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a40: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00000a50: 6176 6168 692d 6c69 6273 2e61 6172 6368  avahi-libs.aarch
-00000a60: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00000a70: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00000a80: 2e38 2d34 2e75 656c 3230 2020 2020 2020  .8-4.uel20      
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000aa0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00000ab0: 0a62 6173 6573 7973 7465 6d2e 6e6f 6172  .basesystem.noar
-00000ac0: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00000ae0: 322d 322e 7565 6c32 3020 2020 2020 2020  2-2.uel20       
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00000b10: 6261 7368 2e61 6172 6368 3634 2020 2020  bash.aarch64    
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 2020 2020 2035 2e30 2d31 372e           5.0-17.
-00000b40: 7570 312e 7565 6c32 3020 2020 2020 2020  up1.uel20       
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00000b70: 6269 6e75 7469 6c73 2e61 6172 6368 3634  binutils.aarch64
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 2020 2020 2020 2020 2020 2032 2e33               2.3
-00000ba0: 342d 3131 2e75 656c 3230 2020 2020 2020  4-11.uel20      
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00000bd0: 0a62 6c75 657a 2e61 6172 6368 3634 2020  .bluez.aarch64  
-00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2020 2020 2020 2020 2035 2e35 342d             5.54-
-00000c00: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 2020 2020 4061 6e61 636f 6e64 610a 626c      @anaconda.bl
-00000c30: 7565 7a2d 6c69 6273 2e61 6172 6368 3634  uez-libs.aarch64
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 2020 2020 2020 2020 2035 2e35               5.5
-00000c60: 342d 312e 7565 6c32 3020 2020 2020 2020  4-1.uel20       
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00000c90: 626f 6f73 742d 696f 7374 7265 616d 732e  boost-iostreams.
-00000ca0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 312e 3733 2e30 2d33 2e75 656c      1.73.0-3.uel
-00000cd0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00000cf0: 616e 6163 6f6e 6461 0a62 726f 746c 692e  anaconda.brotli.
-00000d00: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2020 312e 302e 372d 342e 7565 6c32      1.0.7-4.uel2
-00000d30: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00000d40: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00000d50: 6e61 636f 6e64 610a 6274 7266 732d 7072  naconda.btrfs-pr
-00000d60: 6f67 732e 6161 7263 6836 3420 2020 2020  ogs.aarch64     
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 2020 352e 372d 312e 7565          5.7-1.ue
-00000d90: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 4061 6e61 636f 6e64 610a 627a 6970 322e  @anaconda.bzip2.
-00000dc0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 2020 2020 312e 302e 382d 332e 7565 6c32      1.0.8-3.uel2
-00000df0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00000e00: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00000e10: 6e61 636f 6e64 610a 6361 2d63 6572 7469  naconda.ca-certi
-00000e20: 6669 6361 7465 732e 6e6f 6172 6368 2020  ficates.noarch  
-00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e40: 2020 2020 2020 2020 2020 2032 3032 302e             2020.
-00000e50: 322e 3436 2d31 2e75 656c 3230 2020 2020  2.46-1.uel20    
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00000e80: 6461 0a63 6169 726f 2e61 6172 6368 3634  da.cairo.aarch64
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ea0: 2020 2020 2020 2020 2020 2020 2031 2e31               1.1
-00000eb0: 362e 302d 342e 7565 6c32 3020 2020 2020  6.0-4.uel20     
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00000ee0: 610a 6368 6b63 6f6e 6669 672e 6161 7263  a.chkconfig.aarc
-00000ef0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 312e 3134 2d31 2e75 656c 3230 2020 2020  1.14-1.uel20    
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00000f40: 6461 0a63 6872 6f6e 792e 6161 7263 6836  da.chrony.aarch6
-00000f50: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00000f60: 2020 2020 2020 2020 2020 2020 2020 332e                3.
-00000f70: 352d 332e 7565 6c32 3020 2020 2020 2020  5-3.uel20       
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00000fa0: 6368 726f 6e79 2d68 656c 702e 6e6f 6172  chrony-help.noar
-00000fb0: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-00000fd0: 2e35 2d33 2e75 656c 3230 2020 2020 2020  .5-3.uel20      
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00001000: 0a63 6f6c 6f72 642d 6c69 6273 2e61 6172  .colord-libs.aar
-00001010: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001030: 2031 2e34 2e34 2d31 2e75 656c 3230 2020   1.4.4-1.uel20  
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00001060: 6f6e 6461 0a63 6f72 6575 7469 6c73 2e61  onda.coreutils.a
-00001070: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2020 2038 2e33 322d 322e 7570 312e 7565     8.32-2.up1.ue
-000010a0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 4061 6e61 636f 6e64 610a 6370 696f 2e61  @anaconda.cpio.a
-000010d0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2032 2e31 332d 332e 7565 6c32 3020     2.13-3.uel20 
-00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00001120: 636f 6e64 610a 6370 702e 6161 7263 6836  conda.cpp.aarch6
-00001130: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00001140: 2020 2020 2020 2020 2020 2020 2020 372e                7.
-00001150: 332e 302d 3230 3231 3036 3035 2e33 392e  3.0-20210605.39.
-00001160: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 4061 6e61 636f 6e64 610a 6372 6163    @anaconda.crac
-00001190: 6b6c 6962 2e61 6172 6368 3634 2020 2020  klib.aarch64    
-000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011b0: 2020 2020 2020 2020 2032 2e39 2e37 2d34           2.9.7-4
-000011c0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 2040 616e 6163 6f6e 6461 0a63 726f     @anaconda.cro
-000011f0: 6e69 652e 6161 7263 6836 3420 2020 2020  nie.aarch64     
-00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001210: 2020 2020 2020 2020 312e 352e 352d 332e          1.5.5-3.
-00001220: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 2020 4061 6e61 636f 6e64 610a 6372 6f6e    @anaconda.cron
-00001250: 7461 6273 2e6e 6f61 7263 6820 2020 2020  tabs.noarch     
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 312e 3131 2d32 312e          1.11-21.
-00001280: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 4061 6e61 636f 6e64 610a 6372 7970    @anaconda.cryp
-000012b0: 746f 2d70 6f6c 6963 6965 732e 6e6f 6172  to-policies.noar
-000012c0: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-000012e0: 3032 3030 3631 392d 312e 6769 7437 3831  0200619-1.git781
-000012f0: 6262 6434 2e75 656c 3230 2020 2020 2020  bbd4.uel20      
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00001320: 0a63 7279 7074 7365 7475 702e 6161 7263  .cryptsetup.aarc
-00001330: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001350: 322e 332e 332d 312e 7565 6c32 3020 2020  2.3.3-1.uel20   
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00001380: 6e64 610a 6375 7073 2d6c 6962 732e 6161  nda.cups-libs.aa
-00001390: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2020 313a 322e 322e 3133 2d36 2e75 7031    1:2.2.13-6.up1
-000013c0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 2020 2040 616e 6163 6f6e 6461 0a63 7572     @anaconda.cur
-000013f0: 6c2e 6161 7263 6836 3420 2020 2020 2020  l.aarch64       
-00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001410: 2020 2020 2020 372e 3731 2e31 2d37 2e75        7.71.1-7.u
-00001420: 7031 2e75 656c 3230 2020 2020 2020 2020  p1.uel20        
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2020 2040 616e 6163 6f6e 6461 0a63       @anaconda.c
-00001450: 7972 7573 2d73 6173 6c2d 6c69 622e 6161  yrus-sasl-lib.aa
-00001460: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001480: 2020 322e 312e 3237 2d31 322e 7565 6c32    2.1.27-12.uel2
-00001490: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000014a0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000014b0: 6e61 636f 6e64 610a 6461 7863 746c 2d6c  naconda.daxctl-l
-000014c0: 6962 732e 6161 7263 6836 3420 2020 2020  ibs.aarch64     
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014e0: 2020 2020 2020 2020 3638 2d31 2e75 656c          68-1.uel
-000014f0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00001500: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00001510: 616e 6163 6f6e 6461 0a64 6275 732e 6161  anaconda.dbus.aa
-00001520: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 313a 312e 3132 2e31 362d 3137 2e75    1:1.12.16-17.u
-00001550: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2040 616e 6163 6f6e 6461 0a64 6275 732d   @anaconda.dbus-
-00001580: 636f 6d6d 6f6e 2e6e 6f61 7263 6820 2020  common.noarch   
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 2020 313a 312e 3132            1:1.12
-000015b0: 2e31 362d 3137 2e75 656c 3230 2020 2020  .16-17.uel20    
-000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015d0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000015e0: 6461 0a64 6275 732d 6461 656d 6f6e 2e61  da.dbus-daemon.a
-000015f0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001610: 2020 2031 3a31 2e31 322e 3136 2d31 372e     1:1.12.16-17.
-00001620: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 2020 4061 6e61 636f 6e64 610a 6462 7573    @anaconda.dbus
-00001650: 2d6c 6962 732e 6161 7263 6836 3420 2020  -libs.aarch64   
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 2020 313a 312e 3132            1:1.12
-00001680: 2e31 362d 3137 2e75 656c 3230 2020 2020  .16-17.uel20    
-00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016a0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000016b0: 6461 0a64 6275 732d 746f 6f6c 732e 6161  da.dbus-tools.aa
-000016c0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 313a 312e 3132 2e31 362d 3137 2e75    1:1.12.16-17.u
-000016f0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2040 616e 6163 6f6e 6461 0a64 6275 732d   @anaconda.dbus-
-00001720: 7831 312e 6161 7263 6836 3420 2020 2020  x11.aarch64     
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 2020 2020 313a 312e 3132 2e31          1:1.12.1
-00001750: 362d 3137 2e75 656c 3230 2020 2020 2020  6-17.uel20      
-00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001770: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00001780: 0a64 6278 746f 6f6c 2e61 6172 6368 3634  .dbxtool.aarch64
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 2020 2020 2020 2038 2d31               8-1
-000017b0: 302e 7565 6c32 3020 2020 2020 2020 2020  0.uel20         
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 2020 4061 6e61 636f 6e64 610a 6463      @anaconda.dc
-000017e0: 6f6e 662e 6161 7263 6836 3420 2020 2020  onf.aarch64     
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2020 2020 2020 2020 302e 3334 2e30 2d34          0.34.0-4
-00001810: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 2040 616e 6163 6f6e 6461 0a64 6576     @anaconda.dev
-00001840: 6963 652d 6d61 7070 6572 2e61 6172 6368  ice-mapper.aarch
-00001850: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00001860: 2020 2020 2020 2020 2020 2020 2020 2038                 8
-00001870: 3a31 2e30 322e 3137 312d 352e 7570 312e  :1.02.171-5.up1.
-00001880: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 4061 6e61 636f 6e64 610a 6465 7669    @anaconda.devi
-000018b0: 6365 2d6d 6170 7065 722d 6576 656e 742e  ce-mapper-event.
-000018c0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018e0: 2020 2020 383a 312e 3032 2e31 3731 2d35      8:1.02.171-5
-000018f0: 2e75 7031 2e75 656c 3230 2020 2020 2020  .up1.uel20      
-00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001910: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00001920: 0a64 6863 702e 6161 7263 6836 3420 2020  .dhcp.aarch64   
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2020 2020 2020 3132 3a34 2e34            12:4.4
-00001950: 2e32 2d35 2e75 7031 2e75 656c 3230 2020  .2-5.up1.uel20  
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00001980: 6f6e 6461 0a64 6863 702d 6865 6c70 2e6e  onda.dhcp-help.n
-00001990: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 3132 3a34 2e34 2e32 2d35 2e75 7031    12:4.4.2-5.up1
-000019c0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 2020 2040 616e 6163 6f6e 6461 0a64 6966     @anaconda.dif
-000019f0: 6675 7469 6c73 2e61 6172 6368 3634 2020  futils.aarch64  
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 2020 2020 2020 2033 2e37 2d33             3.7-3
-00001a20: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 2020 2040 616e 6163 6f6e 6461 0a64 6b6d     @anaconda.dkm
-00001a50: 732e 6e6f 6172 6368 2020 2020 2020 2020  s.noarch        
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2020 2032 2e36 2e31 2d36 2e75 656c       2.6.1-6.uel
-00001a80: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00001aa0: 616e 6163 6f6e 6461 0a64 6d69 6465 636f  anaconda.dmideco
-00001ab0: 6465 2e61 6172 6368 3634 2020 2020 2020  de.aarch64      
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 2020 2020 2020 2031 3a33 2e32 2d33 2e75         1:3.2-3.u
-00001ae0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b00: 2040 616e 6163 6f6e 6461 0a64 6e66 2e6e   @anaconda.dnf.n
-00001b10: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2020 342e 322e 3233 2d34 2e75 656c 3230    4.2.23-4.uel20
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00001b60: 6163 6f6e 6461 0a64 6e66 2d68 656c 702e  aconda.dnf-help.
-00001b70: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2034 2e32 2e32 332d 342e 7565 6c32     4.2.23-4.uel2
-00001ba0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00001bc0: 6e61 636f 6e64 610a 646e 662d 706c 7567  naconda.dnf-plug
-00001bd0: 696e 732d 636f 7265 2e6e 6f61 7263 6820  ins-core.noarch 
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2020 2020 2020 2020 2020 2020 342e 302e              4.0.
-00001c00: 3137 2d32 2e75 7031 2e75 656c 3230 2020  17-2.up1.uel20  
-00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c20: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00001c30: 6f6e 6461 0a64 6f73 6673 746f 6f6c 732e  onda.dosfstools.
-00001c40: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 342e 312d 392e 7565 6c32 3020      4.1-9.uel20 
-00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00001c90: 636f 6e64 610a 6472 6163 7574 2e61 6172  conda.dracut.aar
-00001ca0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cc0: 2030 3530 2d35 2e75 656c 3230 2020 2020   050-5.uel20    
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ce0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00001cf0: 6461 0a64 7261 6375 742d 636f 6e66 6967  da.dracut-config
-00001d00: 2d72 6573 6375 652e 6161 7263 6836 3420  -rescue.aarch64 
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d20: 2020 2020 2020 2020 2020 2020 3035 302d              050-
-00001d30: 352e 7565 6c32 3020 2020 2020 2020 2020  5.uel20         
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 2020 4061 6e61 636f 6e64 610a 6472      @anaconda.dr
-00001d60: 6163 7574 2d6e 6574 776f 726b 2e61 6172  acut-network.aar
-00001d70: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2030 3530 2d35 2e75 656c 3230 2020 2020   050-5.uel20    
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001db0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00001dc0: 6461 0a64 7261 6375 742d 7371 7561 7368  da.dracut-squash
-00001dd0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2020 2020 2030 3530 2d35 2e75 656c 3230       050-5.uel20
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00001e20: 6163 6f6e 6461 0a65 3266 7370 726f 6773  aconda.e2fsprogs
-00001e30: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 2020 2020 2031 2e34 352e 362d 322e 7565       1.45.6-2.ue
-00001e60: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 4061 6e61 636f 6e64 610a 6532 6673 7072  @anaconda.e2fspr
-00001e90: 6f67 732d 6865 6c70 2e6e 6f61 7263 6820  ogs-help.noarch 
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 2020 2020 2020 2020 2020 2020 312e 3435              1.45
-00001ec0: 2e36 2d32 2e75 656c 3230 2020 2020 2020  .6-2.uel20      
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00001ef0: 0a65 6274 6162 6c65 732e 6161 7263 6836  .ebtables.aarch6
-00001f00: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00001f10: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-00001f20: 302e 3131 2d32 2e75 656c 3230 2020 2020  0.11-2.uel20    
-00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f40: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00001f50: 6461 0a65 6669 2d66 696c 6573 7973 7465  da.efi-filesyste
-00001f60: 6d2e 6e6f 6172 6368 2020 2020 2020 2020  m.noarch        
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2020 2034 2d34 2e75 7031 2e75 656c       4-4.up1.uel
-00001f90: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00001fb0: 616e 6163 6f6e 6461 0a65 6669 2d73 7270  anaconda.efi-srp
-00001fc0: 6d2d 6d61 6372 6f73 2e6e 6f61 7263 6820  m-macros.noarch 
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 2020 2020 2020 2020 342d 342e              4-4.
-00001ff0: 7570 312e 7565 6c32 3020 2020 2020 2020  up1.uel20       
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00002020: 6566 6962 6f6f 746d 6772 2e61 6172 6368  efibootmgr.aarch
-00002030: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00002040: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00002050: 372d 322e 7565 6c32 3020 2020 2020 2020  7-2.uel20       
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00002080: 6566 6976 6172 2e61 6172 6368 3634 2020  efivar.aarch64  
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 2020 2020 2020 2020 2020 2033 372d 332e             37-3.
-000020b0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 4061 6e61 636f 6e64 610a 6566 6976    @anaconda.efiv
-000020e0: 6172 2d6c 6962 732e 6161 7263 6836 3420  ar-libs.aarch64 
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 2020 2020 2020 2020 2020 3337 2d33              37-3
-00002110: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2040 616e 6163 6f6e 6461 0a65 6c66     @anaconda.elf
-00002140: 7574 696c 732e 6161 7263 6836 3420 2020  utils.aarch64   
-00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002160: 2020 2020 2020 2020 2020 302e 3138 302d            0.180-
-00002170: 332e 7565 6c32 3020 2020 2020 2020 2020  3.uel20         
-00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002190: 2020 2020 4061 6e61 636f 6e64 610a 6574      @anaconda.et
-000021a0: 6874 6f6f 6c2e 6161 7263 6836 3420 2020  htool.aarch64   
-000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021c0: 2020 2020 2020 2020 2020 323a 352e 342d            2:5.4-
-000021d0: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2020 2020 4061 6e61 636f 6e64 610a 6578      @anaconda.ex
-00002200: 7061 742e 6161 7263 6836 3420 2020 2020  pat.aarch64     
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 2020 322e 322e 392d 322e          2.2.9-2.
-00002230: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 4061 6e61 636f 6e64 610a 6669 6c65    @anaconda.file
-00002260: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2035 2e33 392d 312e 7565 6c32       5.39-1.uel2
-00002290: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000022a0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000022b0: 6e61 636f 6e64 610a 6669 6c65 2d6c 6962  naconda.file-lib
-000022c0: 732e 6161 7263 6836 3420 2020 2020 2020  s.aarch64       
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2020 2020 2020 352e 3339 2d31 2e75 656c        5.39-1.uel
-000022f0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00002300: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00002310: 616e 6163 6f6e 6461 0a66 696c 6573 7973  anaconda.filesys
-00002320: 7465 6d2e 6161 7263 6836 3420 2020 2020  tem.aarch64     
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 332e 3134 2d32 2e75          3.14-2.u
-00002350: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2040 616e 6163 6f6e 6461 0a66 696e 6475   @anaconda.findu
-00002380: 7469 6c73 2e61 6172 6368 3634 2020 2020  tils.aarch64    
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 2020 2032 3a34 2e37 2e30           2:4.7.0
-000023b0: 2d35 2e75 656c 3230 2020 2020 2020 2020  -5.uel20        
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 2020 2040 616e 6163 6f6e 6461 0a66       @anaconda.f
-000023e0: 6970 7363 6865 636b 2e61 6172 6368 3634  ipscheck.aarch64
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 2020 2020 2020 2020 2020 2031 2e35               1.5
-00002410: 2e30 2d38 2e75 656c 3230 2020 2020 2020  .0-8.uel20      
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00002440: 0a66 6972 6577 616c 6c64 2e6e 6f61 7263  .firewalld.noarc
-00002450: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-00002460: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-00002470: 362e 362d 342e 7565 6c32 3020 2020 2020  6.6-4.uel20     
-00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002490: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-000024a0: 610a 6669 7265 7761 6c6c 642d 646f 632e  a.firewalld-doc.
-000024b0: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2030 2e36 2e36 2d34 2e75 656c 3230     0.6.6-4.uel20
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00002500: 6163 6f6e 6461 0a66 6f6e 7463 6f6e 6669  aconda.fontconfi
-00002510: 672e 6161 7263 6836 3420 2020 2020 2020  g.aarch64       
-00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002530: 2020 2020 2020 322e 3133 2e39 322d 312e        2.13.92-1.
-00002540: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 4061 6e61 636f 6e64 610a 666f 6e74    @anaconda.font
-00002570: 732d 6669 6c65 7379 7374 656d 2e6e 6f61  s-filesystem.noa
-00002580: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-00002590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025a0: 322e 302e 322d 342e 7565 6c32 3020 2020  2.0.2-4.uel20   
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000025d0: 6e64 610a 6672 6565 7479 7065 2e61 6172  nda.freetype.aar
-000025e0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 2032 2e31 302e 322d 332e 7565 6c32 3020   2.10.2-3.uel20 
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00002630: 636f 6e64 610a 6672 6962 6964 692e 6161  conda.fribidi.aa
-00002640: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 312e 302e 3130 2d31 2e75 656c 3230    1.0.10-1.uel20
-00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002680: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00002690: 6163 6f6e 6461 0a66 7573 652e 6161 7263  aconda.fuse.aarc
-000026a0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 322e 392e 392d 342e 7565 6c32 3020 2020  2.9.9-4.uel20   
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000026f0: 6e64 610a 6675 7365 2d63 6f6d 6d6f 6e2e  nda.fuse-common.
-00002700: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 332e 392e 322d 342e 7565 6c32      3.9.2-4.uel2
-00002730: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00002740: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00002750: 6e61 636f 6e64 610a 6675 7365 2d68 656c  naconda.fuse-hel
-00002760: 702e 6161 7263 6836 3420 2020 2020 2020  p.aarch64       
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 322e 392e 392d 342e 7565        2.9.9-4.ue
-00002790: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 4061 6e61 636f 6e64 610a 6761 6d69 6e2e  @anaconda.gamin.
-000027c0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 302e 312e 3130 2d33 392e 7565      0.1.10-39.ue
-000027f0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 4061 6e61 636f 6e64 610a 6761 776b 2e61  @anaconda.gawk.a
-00002820: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2035 2e30 2e31 2d33 2e75 656c 3230     5.0.1-3.uel20
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00002870: 6163 6f6e 6461 0a67 632e 6161 7263 6836  aconda.gc.aarch6
-00002880: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00002890: 2020 2020 2020 2020 2020 2020 2020 382e                8.
-000028a0: 302e 342d 332e 7565 6c32 3020 2020 2020  0.4-3.uel20     
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-000028d0: 610a 6763 632e 6161 7263 6836 3420 2020  a.gcc.aarch64   
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 2020 2020 2020 2020 372e 332e 302d            7.3.0-
-00002900: 3230 3231 3036 3035 2e33 392e 7565 6c32  20210605.39.uel2
-00002910: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00002920: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00002930: 6e61 636f 6e64 610a 6763 722e 6161 7263  naconda.gcr.aarc
-00002940: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002960: 332e 3334 2e30 2d31 2e75 656c 3230 2020  3.34.0-1.uel20  
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00002990: 6f6e 6461 0a67 6462 6d2e 6161 7263 6836  onda.gdbm.aarch6
-000029a0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-000029b0: 2020 2020 2020 2020 2020 2020 2020 313a                1:
-000029c0: 312e 3138 2e31 2d31 2e75 656c 3230 2020  1.18.1-1.uel20  
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000029f0: 6f6e 6461 0a67 6469 736b 2e61 6172 6368  onda.gdisk.aarch
-00002a00: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00002a20: 2e30 2e35 2d31 2e75 656c 3230 2020 2020  .0.5-1.uel20    
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00002a50: 6461 0a67 646b 2d70 6978 6275 6632 2e61  da.gdk-pixbuf2.a
-00002a60: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2032 2e33 382e 302d 392e 7565 6c32     2.38.0-9.uel2
-00002a90: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00002ab0: 6e61 636f 6e64 610a 6765 7474 6578 742e  naconda.gettext.
-00002ac0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 302e 3231 2d34 2e75 656c 3230      0.21-4.uel20
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00002b10: 6163 6f6e 6461 0a67 6c69 622d 6e65 7477  aconda.glib-netw
-00002b20: 6f72 6b69 6e67 2e61 6172 6368 3634 2020  orking.aarch64  
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2020 2020 2032 2e36 322e             2.62.
-00002b50: 342d 312e 7565 6c32 3020 2020 2020 2020  4-1.uel20       
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00002b80: 676c 6962 322e 6161 7263 6836 3420 2020  glib2.aarch64   
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2020 2020 2020 322e 3636 2e38            2.66.8
-00002bb0: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2040 616e 6163 6f6e 6461 0a67       @anaconda.g
-00002be0: 6c69 6232 2d68 656c 702e 6e6f 6172 6368  lib2-help.noarch
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2032 2e36               2.6
-00002c10: 362e 382d 312e 7565 6c32 3020 2020 2020  6.8-1.uel20     
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00002c40: 610a 676c 6962 632e 6161 7263 6836 3420  a.glibc.aarch64 
-00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c60: 2020 2020 2020 2020 2020 2020 322e 3238              2.28
-00002c70: 2d36 392e 7570 312e 7565 6c32 3020 2020  -69.up1.uel20   
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00002ca0: 6e64 610a 676c 6962 632d 636f 6d6d 6f6e  nda.glibc-common
-00002cb0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2032 2e32 382d 3639 2e75 7031       2.28-69.up1
-00002ce0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2040 616e 6163 6f6e 6461 0a67 6c69     @anaconda.gli
-00002d10: 6263 2d64 6576 656c 2e61 6172 6368 3634  bc-devel.aarch64
-00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d30: 2020 2020 2020 2020 2020 2020 2032 2e32               2.2
-00002d40: 382d 3639 2e75 7031 2e75 656c 3230 2020  8-69.up1.uel20  
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00002d70: 6f6e 6461 0a67 6d70 2e61 6172 6368 3634  onda.gmp.aarch64
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2020 2020 2020 2020 2020 2020 2031 3a36               1:6
-00002da0: 2e32 2e30 2d31 2e75 656c 3230 2020 2020  .2.0-1.uel20    
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00002dd0: 6461 0a67 6e75 7067 322e 6161 7263 6836  da.gnupg2.aarch6
-00002de0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00002df0: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-00002e00: 322e 3231 2d33 2e75 656c 3230 2020 2020  2.21-3.uel20    
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00002e30: 6461 0a67 6e75 746c 732e 6161 7263 6836  da.gnutls.aarch6
-00002e40: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00002e50: 2020 2020 2020 2020 2020 2020 2020 332e                3.
-00002e60: 362e 3134 2d37 2e75 656c 3230 2020 2020  6.14-7.uel20    
-00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e80: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00002e90: 6461 0a67 6f62 6a65 6374 2d69 6e74 726f  da.gobject-intro
-00002ea0: 7370 6563 7469 6f6e 2e61 6172 6368 3634  spection.aarch64
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ec0: 2020 2020 2020 2020 2020 2020 2031 2e35               1.5
-00002ed0: 382e 332d 312e 7565 6c32 3020 2020 2020  8.3-1.uel20     
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ef0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00002f00: 610a 6770 676d 652e 6161 7263 6836 3420  a.gpgme.aarch64 
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 2020 2020 2020 2020 312e 3134              1.14
-00002f30: 2e30 2d31 2e75 656c 3230 2020 2020 2020  .0-1.uel20      
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00002f60: 0a67 7261 7068 6974 6532 2e61 6172 6368  .graphite2.aarch
-00002f70: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00002f80: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00002f90: 2e33 2e31 342d 322e 7565 6c32 3020 2020  .3.14-2.uel20   
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00002fc0: 6e64 610a 6772 6570 2e61 6172 6368 3634  nda.grep.aarch64
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fe0: 2020 2020 2020 2020 2020 2020 2033 2e34               3.4
-00002ff0: 2d30 2e75 656c 3230 2020 2020 2020 2020  -0.uel20        
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 2020 2020 2040 616e 6163 6f6e 6461 0a67       @anaconda.g
-00003020: 726f 6666 2e61 6172 6368 3634 2020 2020  roff.aarch64    
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2020 2020 2031 2e32 322e 342d           1.22.4-
-00003050: 362e 7565 6c32 3020 2020 2020 2020 2020  6.uel20         
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2020 2020 4061 6e61 636f 6e64 610a 6772      @anaconda.gr
-00003080: 7562 2d74 6865 6d65 732d 6465 6570 696e  ub-themes-deepin
-00003090: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 2020 2020 2031 2e30 2e31 2d31 302e 7565       1.0.1-10.ue
-000030c0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030e0: 4061 6e61 636f 6e64 610a 6772 7562 322d  @anaconda.grub2-
-000030f0: 636f 6d6d 6f6e 2e6e 6f61 7263 6820 2020  common.noarch   
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 2020 2020 2020 2020 2020 313a 322e 3034            1:2.04
-00003120: 2d31 382e 7570 382e 7565 6c32 3020 2020  -18.up8.uel20   
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003150: 6e64 610a 6772 7562 322d 6566 692d 6161  nda.grub2-efi-aa
-00003160: 3634 2e61 6172 6368 3634 2020 2020 2020  64.aarch64      
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2031 3a32 2e30 342d 3138         1:2.04-18
-00003190: 2e75 7038 2e75 656c 3230 2020 2020 2020  .up8.uel20      
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031b0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000031c0: 0a67 7275 6232 2d65 6669 2d61 6136 342d  .grub2-efi-aa64-
-000031d0: 6364 626f 6f74 2e61 6172 6368 3634 2020  cdboot.aarch64  
-000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 2020 2020 2020 2020 2031 3a32 2e30             1:2.0
-00003200: 342d 3138 2e75 7038 2e75 656c 3230 2020  4-18.up8.uel20  
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00003230: 6f6e 6461 0a67 7275 6232 2d65 6669 2d61  onda.grub2-efi-a
-00003240: 6136 342d 6d6f 6475 6c65 732e 6e6f 6172  a64-modules.noar
-00003250: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-00003260: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00003270: 3a32 2e30 342d 3138 2e75 7038 2e75 656c  :2.04-18.up8.uel
-00003280: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00003290: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-000032a0: 616e 6163 6f6e 6461 0a67 7275 6232 2d74  anaconda.grub2-t
-000032b0: 6f6f 6c73 2e61 6172 6368 3634 2020 2020  ools.aarch64    
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2020 2020 2031 3a32 2e30 342d           1:2.04-
-000032e0: 3138 2e75 7038 2e75 656c 3230 2020 2020  18.up8.uel20    
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00003310: 6461 0a67 7275 6232 2d74 6f6f 6c73 2d65  da.grub2-tools-e
-00003320: 7874 7261 2e61 6172 6368 3634 2020 2020  xtra.aarch64    
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2020 2031 3a32 2e30 342d           1:2.04-
-00003350: 3138 2e75 7038 2e75 656c 3230 2020 2020  18.up8.uel20    
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00003380: 6461 0a67 7275 6232 2d74 6f6f 6c73 2d6d  da.grub2-tools-m
-00003390: 696e 696d 616c 2e61 6172 6368 3634 2020  inimal.aarch64  
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 2020 2020 2020 2020 2020 2031 3a32 2e30             1:2.0
-000033c0: 342d 3138 2e75 7038 2e75 656c 3230 2020  4-18.up8.uel20  
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000033f0: 6f6e 6461 0a67 7275 6262 792e 6161 7263  onda.grubby.aarc
-00003400: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 382e 3430 2d32 362e 7565 6c32 3020 2020  8.40-26.uel20   
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003450: 6e64 610a 6773 6574 7469 6e67 732d 6465  nda.gsettings-de
-00003460: 736b 746f 702d 7363 6865 6d61 732e 6161  sktop-schemas.aa
-00003470: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 332e 3337 2e31 2d31 2e75 656c 3230    3.37.1-1.uel20
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034b0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-000034c0: 6163 6f6e 6461 0a67 746b 322e 6161 7263  aconda.gtk2.aarc
-000034d0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 322e 3234 2e33 322d 382e 7565 6c32 3020  2.24.32-8.uel20 
-00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003510: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00003520: 636f 6e64 610a 6774 6b33 2e61 6172 6368  conda.gtk3.aarch
-00003530: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00003540: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-00003550: 2e32 342e 3231 2d32 2e75 656c 3230 2020  .24.21-2.uel20  
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00003580: 6f6e 6461 0a67 7569 6c65 2e61 6172 6368  onda.guile.aarch
-00003590: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2035                 5
-000035b0: 3a32 2e30 2e31 342d 3137 2e75 656c 3230  :2.0.14-17.uel20
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035d0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-000035e0: 6163 6f6e 6461 0a67 7a69 702e 6161 7263  aconda.gzip.aarc
-000035f0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 312e 3130 2d31 2e75 656c 3230 2020 2020  1.10-1.uel20    
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00003640: 6461 0a68 6172 6662 757a 7a2e 6161 7263  da.harfbuzz.aarc
-00003650: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 322e 362e 382d 312e 7565 6c32 3020 2020  2.6.8-1.uel20   
-00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000036a0: 6e64 610a 6864 7061 726d 2e61 6172 6368  nda.hdparm.aarch
-000036b0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2039                 9
-000036d0: 2e35 382d 312e 7565 6c32 3020 2020 2020  .58-1.uel20     
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00003700: 610a 6869 636f 6c6f 722d 6963 6f6e 2d74  a.hicolor-icon-t
-00003710: 6865 6d65 2e6e 6f61 7263 6820 2020 2020  heme.noarch     
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 2020 302e 3137 2d36 2e75          0.17-6.u
-00003740: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003760: 2040 616e 6163 6f6e 6461 0a68 6f73 746e   @anaconda.hostn
-00003770: 616d 652e 6161 7263 6836 3420 2020 2020  ame.aarch64     
-00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003790: 2020 2020 2020 2020 332e 3231 2d31 2e75          3.21-1.u
-000037a0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2040 616e 6163 6f6e 6461 0a68 7764 6174   @anaconda.hwdat
-000037d0: 612e 6e6f 6172 6368 2020 2020 2020 2020  a.noarch        
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 2020 2020 2030 2e33 3337 2d31 2e75 656c       0.337-1.uel
-00003800: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00003810: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00003820: 616e 6163 6f6e 6461 0a69 6d61 2d65 766d  anaconda.ima-evm
-00003830: 2d75 7469 6c73 2d6c 6962 732e 6161 7263  -utils-libs.aarc
-00003840: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 312e 332e 312d 362e 7565 6c32 3020 2020  1.3.1-6.uel20   
-00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003890: 6e64 610a 696e 666f 2e61 6172 6368 3634  nda.info.aarch64
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2020 2020 2020 2020 2020 2020 2036 2e37               6.7
-000038c0: 2d32 2e75 656c 3230 2020 2020 2020 2020  -2.uel20        
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2040 616e 6163 6f6e 6461 0a69       @anaconda.i
-000038f0: 6e69 7473 6372 6970 7473 2e61 6172 6368  nitscripts.aarch
-00003900: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00003910: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00003920: 302e 3034 2d32 2e75 7031 2e75 656c 3230  0.04-2.up1.uel20
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00003950: 6163 6f6e 6461 0a69 7063 616c 632e 6161  aconda.ipcalc.aa
-00003960: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 2020 302e 342e 312d 312e 7565 6c32 3020    0.4.1-1.uel20 
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-000039b0: 636f 6e64 610a 6970 726f 7574 652e 6161  conda.iproute.aa
-000039c0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 2020 352e 352e 302d 352e 7565 6c32 3020    5.5.0-5.uel20 
-000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00003a10: 636f 6e64 610a 6970 726f 7574 652d 6865  conda.iproute-he
-00003a20: 6c70 2e6e 6f61 7263 6820 2020 2020 2020  lp.noarch       
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2020 2020 352e 352e 302d 352e 7565        5.5.0-5.ue
-00003a50: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 4061 6e61 636f 6e64 610a 6970 7275 7469  @anaconda.ipruti
-00003a80: 6c73 2e61 6172 6368 3634 2020 2020 2020  ls.aarch64      
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2032 2e34 2e31 382e 312d         2.4.18.1-
-00003ab0: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2020 2020 4061 6e61 636f 6e64 610a 6970      @anaconda.ip
-00003ae0: 7365 742e 6161 7263 6836 3420 2020 2020  set.aarch64     
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 2020 2020 372e 362d 302e 7565          7.6-0.ue
-00003b10: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b30: 4061 6e61 636f 6e64 610a 6970 7365 742d  @anaconda.ipset-
-00003b40: 6c69 6273 2e61 6172 6368 3634 2020 2020  libs.aarch64    
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2020 2020 2020 2020 2037 2e36 2d30 2e75           7.6-0.u
-00003b70: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 2040 616e 6163 6f6e 6461 0a69 7074 6162   @anaconda.iptab
-00003ba0: 6c65 732e 6161 7263 6836 3420 2020 2020  les.aarch64     
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 2020 2020 2020 2020 312e 382e 352d 322e          1.8.5-2.
-00003bd0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 4061 6e61 636f 6e64 610a 6970 7461    @anaconda.ipta
-00003c00: 626c 6573 2d68 656c 702e 6e6f 6172 6368  bles-help.noarch
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 2020 2020 2020 2020 2020 2031 2e38               1.8
-00003c30: 2e35 2d32 2e75 656c 3230 2020 2020 2020  .5-2.uel20      
-00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00003c60: 0a69 7074 6162 6c65 732d 6c69 6273 2e61  .iptables-libs.a
-00003c70: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 2031 2e38 2e35 2d32 2e75 656c 3230     1.8.5-2.uel20
-00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cb0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00003cc0: 6163 6f6e 6461 0a69 7075 7469 6c73 2e61  aconda.iputils.a
-00003cd0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2032 3031 3930 3730 392d 372e 7565     20190709-7.ue
-00003d00: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 4061 6e61 636f 6e64 610a 6972 7162 616c  @anaconda.irqbal
-00003d30: 616e 6365 2e61 6172 6368 3634 2020 2020  ance.aarch64    
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 2020 2020 2020 2020 2033 3a31 2e37 2e30           3:1.7.0
-00003d60: 2d33 2e75 656c 3230 2020 2020 2020 2020  -3.uel20        
-00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2020 2020 2040 616e 6163 6f6e 6461 0a6a       @anaconda.j
-00003d90: 616e 7373 6f6e 2e61 6172 6368 3634 2020  ansson.aarch64  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 2020 2020 2020 2032 2e31 332e             2.13.
-00003dc0: 312d 312e 7565 6c32 3020 2020 2020 2020  1-1.uel20       
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00003df0: 6a62 6967 6b69 742d 6c69 6273 2e61 6172  jbigkit-libs.aar
-00003e00: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e20: 2032 2e31 2d31 392e 7565 6c32 3020 2020   2.1-19.uel20   
-00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e40: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003e50: 6e64 610a 6a73 6f6e 2d63 2e61 6172 6368  nda.json-c.aarch
-00003e60: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00003e70: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00003e80: 2e31 352d 312e 7565 6c32 3020 2020 2020  .15-1.uel20     
-00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ea0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00003eb0: 610a 6a73 6f6e 2d67 6c69 622e 6161 7263  a.json-glib.aarc
-00003ec0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 312e 342e 342d 322e 7565 6c32 3020 2020  1.4.4-2.uel20   
-00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f00: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003f10: 6e64 610a 6b62 642e 6161 7263 6836 3420  nda.kbd.aarch64 
-00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f30: 2020 2020 2020 2020 2020 2020 322e 322e              2.2.
-00003f40: 302d 312e 7570 312e 7565 6c32 3020 2020  0-1.up1.uel20   
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00003f70: 6e64 610a 6b62 642d 6c65 6761 6379 2e6e  nda.kbd-legacy.n
-00003f80: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fa0: 2020 322e 322e 302d 312e 7570 312e 7565    2.2.0-1.up1.ue
-00003fb0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fd0: 4061 6e61 636f 6e64 610a 6b62 642d 6d69  @anaconda.kbd-mi
-00003fe0: 7363 2e6e 6f61 7263 6820 2020 2020 2020  sc.noarch       
-00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004000: 2020 2020 2020 322e 322e 302d 312e 7570        2.2.0-1.up
-00004010: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004030: 2020 2020 4061 6e61 636f 6e64 610a 6b65      @anaconda.ke
-00004040: 726e 656c 2e61 6172 6368 3634 2020 2020  rnel.aarch64    
-00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004060: 2020 2020 2020 2020 2034 2e31 392e 3930           4.19.90
-00004070: 2d32 3130 362e 332e 302e 3030 3935 2e75  -2106.3.0.0095.u
-00004080: 7032 2e75 656c 3230 2020 2020 2020 2020  p2.uel20        
-00004090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040a0: 2020 2020 2040 616e 6163 6f6e 6461 0a6b       @anaconda.k
-000040b0: 6572 6e65 6c2d 6465 7665 6c2e 6161 7263  ernel-devel.aarc
-000040c0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040e0: 342e 3139 2e39 302d 3231 3036 2e33 2e30  4.19.90-2106.3.0
-000040f0: 2e30 3039 352e 7570 322e 7565 6c32 3020  .0095.up2.uel20 
-00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004110: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00004120: 636f 6e64 610a 6b65 726e 656c 2d74 6f6f  conda.kernel-too
-00004130: 6c73 2e61 6172 6368 3634 2020 2020 2020  ls.aarch64      
-00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004150: 2020 2020 2020 2034 2e31 392e 3930 2d32         4.19.90-2
-00004160: 3130 362e 332e 302e 3030 3935 2e75 7032  106.3.0.0095.up2
-00004170: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 2020 2040 616e 6163 6f6e 6461 0a6b 6578     @anaconda.kex
-000041a0: 6563 2d74 6f6f 6c73 2e61 6172 6368 3634  ec-tools.aarch64
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 2020 2020 2020 2020 2020 2020 2032 2e30               2.0
-000041d0: 2e32 302d 3136 2e75 656c 3230 2020 2020  .20-16.uel20    
-000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041f0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00004200: 6461 0a6b 6579 7574 696c 732d 6c69 6273  da.keyutils-libs
-00004210: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2020 2020 2031 2e36 2e33 2d31 2e75 656c       1.6.3-1.uel
-00004240: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00004250: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00004260: 616e 6163 6f6e 6461 0a6b 6d6f 642e 6161  anaconda.kmod.aa
-00004270: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004290: 2020 3237 2d38 2e75 656c 3230 2020 2020    27-8.uel20    
-000042a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042b0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000042c0: 6461 0a6b 6d6f 642d 6865 6c70 2e61 6172  da.kmod-help.aar
-000042d0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2032 372d 382e 7565 6c32 3020 2020 2020   27-8.uel20     
-00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004310: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00004320: 610a 6b6d 6f64 2d6b 7664 6f2e 6161 7263  a.kmod-kvdo.aarc
-00004330: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004350: 362e 322e 322e 3234 2d37 2e75 656c 3230  6.2.2.24-7.uel20
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00004380: 6163 6f6e 6461 0a6b 6d6f 642d 6c69 6273  aconda.kmod-libs
-00004390: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2020 2020 2032 372d 382e 7565 6c32 3020       27-8.uel20 
-000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043d0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-000043e0: 636f 6e64 610a 6b70 6172 7478 2e61 6172  conda.kpartx.aar
-000043f0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2030 2e38 2e34 2d36 2e75 7031 2e75 656c   0.8.4-6.up1.uel
-00004420: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00004430: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00004440: 616e 6163 6f6e 6461 0a6b 7262 352d 6c69  anaconda.krb5-li
-00004450: 6273 2e61 6172 6368 3634 2020 2020 2020  bs.aarch64      
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 2031 2e31 382e 322d 332e         1.18.2-3.
-00004480: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044a0: 2020 4061 6e61 636f 6e64 610a 6c63 6d73    @anaconda.lcms
-000044b0: 322e 6161 7263 6836 3420 2020 2020 2020  2.aarch64       
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2020 2020 2020 322e 3131 2d31 2e75 656c        2.11-1.uel
-000044e0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00004500: 616e 6163 6f6e 6461 0a6c 6573 732e 6161  anaconda.less.aa
-00004510: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004530: 2020 3535 312d 362e 7565 6c32 3020 2020    551-6.uel20   
-00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004550: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00004560: 6e64 610a 6c69 6249 4345 2e61 6172 6368  nda.libICE.aarch
-00004570: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00004580: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00004590: 2e30 2e31 302d 342e 7565 6c32 3020 2020  .0.10-4.uel20   
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000045c0: 6e64 610a 6c69 6253 4d2e 6161 7263 6836  nda.libSM.aarch6
-000045d0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-000045e0: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-000045f0: 322e 332d 342e 7565 6c32 3020 2020 2020  2.3-4.uel20     
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00004620: 610a 6c69 6258 3131 2e61 6172 6368 3634  a.libX11.aarch64
-00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004640: 2020 2020 2020 2020 2020 2020 2031 2e36               1.6
-00004650: 2e39 2d35 2e75 656c 3230 2020 2020 2020  .9-5.uel20      
-00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00004680: 0a6c 6962 5861 752e 6161 7263 6836 3420  .libXau.aarch64 
-00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 2020 2020 2020 2020 2020 312e 302e              1.0.
-000046b0: 392d 322e 7565 6c32 3020 2020 2020 2020  9-2.uel20       
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046d0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000046e0: 6c69 6258 6177 2e61 6172 6368 3634 2020  libXaw.aarch64  
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 2020 2020 2020 2031 2e30 2e31             1.0.1
-00004710: 332d 3133 2e75 656c 3230 2020 2020 2020  3-13.uel20      
-00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00004740: 0a6c 6962 5863 6f6d 706f 7369 7465 2e61  .libXcomposite.a
-00004750: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2030 2e34 2e35 2d31 2e75 656c 3230     0.4.5-1.uel20
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-000047a0: 6163 6f6e 6461 0a6c 6962 5863 7572 736f  aconda.libXcurso
-000047b0: 722e 6161 7263 6836 3420 2020 2020 2020  r.aarch64       
-000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047d0: 2020 2020 2020 312e 322e 302d 312e 7565        1.2.0-1.ue
-000047e0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 4061 6e61 636f 6e64 610a 6c69 6258 6461  @anaconda.libXda
-00004810: 6d61 6765 2e61 6172 6368 3634 2020 2020  mage.aarch64    
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 2020 2020 2020 2020 2031 2e31 2e35 2d31           1.1.5-1
-00004840: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004860: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-00004870: 5865 7874 2e61 6172 6368 3634 2020 2020  Xext.aarch64    
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 2020 2020 2031 2e33 2e34 2d34           1.3.4-4
-000048a0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-000048d0: 5866 6978 6573 2e61 6172 6368 3634 2020  Xfixes.aarch64  
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 2020 2020 2020 2020 2035 2e30 2e33             5.0.3
-00004900: 2d31 312e 7565 6c32 3020 2020 2020 2020  -11.uel20       
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00004930: 6c69 6258 6674 2e61 6172 6368 3634 2020  libXft.aarch64  
-00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004950: 2020 2020 2020 2020 2020 2032 2e33 2e33             2.3.3
-00004960: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00004990: 6962 5869 2e61 6172 6368 3634 2020 2020  ibXi.aarch64    
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2020 2020 2020 2020 2031 2e37 2e31 302d           1.7.10-
-000049c0: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-000049f0: 6258 696e 6572 616d 612e 6161 7263 6836  bXinerama.aarch6
-00004a00: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00004a10: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-00004a20: 312e 342d 352e 7565 6c32 3020 2020 2020  1.4-5.uel20     
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00004a50: 610a 6c69 6258 6d75 2e61 6172 6368 3634  a.libXmu.aarch64
-00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a70: 2020 2020 2020 2020 2020 2020 2031 2e31               1.1
-00004a80: 2e33 2d31 2e75 656c 3230 2020 2020 2020  .3-1.uel20      
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00004ab0: 0a6c 6962 5870 6d2e 6161 7263 6836 3420  .libXpm.aarch64 
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 2020 2020 2020 2020 332e 352e              3.5.
-00004ae0: 3133 2d31 2e75 656c 3230 2020 2020 2020  13-1.uel20      
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00004b10: 0a6c 6962 5872 616e 6472 2e61 6172 6368  .libXrandr.aarch
-00004b20: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00004b40: 2e35 2e32 2d31 2e75 656c 3230 2020 2020  .5.2-1.uel20    
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b60: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00004b70: 6461 0a6c 6962 5872 656e 6465 722e 6161  da.libXrender.aa
-00004b80: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2020 302e 392e 3130 2d31 302e 7565 6c32    0.9.10-10.uel2
-00004bb0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00004bd0: 6e61 636f 6e64 610a 6c69 6258 742e 6161  naconda.libXt.aa
-00004be0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2020 312e 322e 302d 312e 7565 6c32 3020    1.2.0-1.uel20 
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00004c30: 636f 6e64 610a 6c69 6258 7473 742e 6161  conda.libXtst.aa
-00004c40: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c60: 2020 312e 322e 332d 3130 2e75 656c 3230    1.2.3-10.uel20
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00004c90: 6163 6f6e 6461 0a6c 6962 6163 6c2e 6161  aconda.libacl.aa
-00004ca0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 322e 322e 3533 2d38 2e75 656c 3230    2.2.53-8.uel20
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00004cf0: 6163 6f6e 6461 0a6c 6962 6169 6f2e 6161  aconda.libaio.aa
-00004d00: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 2020 302e 332e 3131 322d 312e 7565 6c32    0.3.112-1.uel2
-00004d30: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00004d40: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00004d50: 6e61 636f 6e64 610a 6c69 6261 7263 6869  naconda.libarchi
-00004d60: 7665 2e61 6172 6368 3634 2020 2020 2020  ve.aarch64      
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2020 2020 2033 2e34 2e33 2d32 2e75         3.4.3-2.u
-00004d90: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004db0: 2040 616e 6163 6f6e 6461 0a6c 6962 6172   @anaconda.libar
-00004dc0: 676f 6e32 2e61 6172 6368 3634 2020 2020  gon2.aarch64    
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 2020 2020 2032 3031 3930 3730           2019070
-00004df0: 322d 312e 7565 6c32 3020 2020 2020 2020  2-1.uel20       
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00004e20: 6c69 6261 7373 7561 6e2e 6161 7263 6836  libassuan.aarch6
-00004e30: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00004e40: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-00004e50: 352e 332d 312e 7565 6c32 3020 2020 2020  5.3-1.uel20     
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00004e80: 610a 6c69 6261 7461 736d 6172 742e 6161  a.libatasmart.aa
-00004e90: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004eb0: 2020 302e 3139 2d31 372e 7565 6c32 3020    0.19-17.uel20 
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00004ee0: 636f 6e64 610a 6c69 6262 6c6b 6964 2e61  conda.libblkid.a
-00004ef0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2032 2e33 352e 322d 362e 7570 312e     2.35.2-6.up1.
-00004f20: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 4061 6e61 636f 6e64 610a 6c69 6262    @anaconda.libb
-00004f50: 6c6f 636b 6465 762e 6161 7263 6836 3420  lockdev.aarch64 
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 2020 2020 322e 3234              2.24
-00004f80: 2d32 2e75 656c 3230 2020 2020 2020 2020  -2.uel20        
-00004f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fa0: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00004fb0: 6962 6279 7465 7369 7a65 2e61 6172 6368  ibbytesize.aarch
-00004fc0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00004fe0: 2e34 2d31 2e75 656c 3230 2020 2020 2020  .4-1.uel20      
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00005010: 0a6c 6962 6361 702e 6161 7263 6836 3420  .libcap.aarch64 
-00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 2020 2020 2020 2020 2020 322e 3332              2.32
-00005040: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005070: 6962 6361 702d 6e67 2e61 6172 6368 3634  ibcap-ng.aarch64
-00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005090: 2020 2020 2020 2020 2020 2020 2030 2e37               0.7
-000050a0: 2e31 302d 312e 7565 6c32 3020 2020 2020  .10-1.uel20     
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-000050d0: 610a 6c69 6263 6f6d 7073 2e61 6172 6368  a.libcomps.aarch
-000050e0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00005100: 2e31 2e31 302d 322e 7565 6c32 3020 2020  .1.10-2.uel20   
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00005130: 6e64 610a 6c69 6263 7572 6c2e 6161 7263  nda.libcurl.aarc
-00005140: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 372e 3731 2e31 2d37 2e75 7031 2e75 656c  7.71.1-7.up1.uel
-00005170: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00005180: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00005190: 616e 6163 6f6e 6461 0a6c 6962 6461 656d  anaconda.libdaem
-000051a0: 6f6e 2e61 6172 6368 3634 2020 2020 2020  on.aarch64      
-000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2020 2020 2020 2030 2e31 342d 3230 2e75         0.14-20.u
-000051d0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2040 616e 6163 6f6e 6461 0a6c 6962 6461   @anaconda.libda
-00005200: 7472 6965 2e61 6172 6368 3634 2020 2020  trie.aarch64    
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2020 2020 2020 2030 2e32 2e31 322d           0.2.12-
-00005230: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005250: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00005260: 6264 622e 6161 7263 6836 3420 2020 2020  bdb.aarch64     
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2020 2020 2020 352e 332e 3238 2d33          5.3.28-3
-00005290: 362e 7565 6c32 3020 2020 2020 2020 2020  6.uel20         
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-000052c0: 6264 6e66 2e61 6172 6368 3634 2020 2020  bdnf.aarch64    
-000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 2020 2020 2020 2020 2030 2e34 382e 302d           0.48.0-
-000052f0: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005310: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00005320: 6264 726d 2e61 6172 6368 3634 2020 2020  bdrm.aarch64    
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2020 2032 2e34 2e31 3032           2.4.102
-00005350: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005380: 6962 6564 6974 2e61 6172 6368 3634 2020  ibedit.aarch64  
-00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 2020 2020 2020 2020 2033 2e31 2d32             3.1-2
-000053b0: 372e 7565 6c32 3020 2020 2020 2020 2020  7.uel20         
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-000053e0: 6265 706f 7879 2e61 6172 6368 3634 2020  bepoxy.aarch64  
-000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005400: 2020 2020 2020 2020 2020 2031 2e35 2e34             1.5.4
-00005410: 2d32 2e75 656c 3230 2020 2020 2020 2020  -2.uel20        
-00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005430: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005440: 6962 6573 7472 2e61 6172 6368 3634 2020  ibestr.aarch64  
-00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 2020 2020 2020 2020 2020 2030 2e31 2e31             0.1.1
-00005470: 312d 312e 7565 6c32 3020 2020 2020 2020  1-1.uel20       
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000054a0: 6c69 6265 762e 6161 7263 6836 3420 2020  libev.aarch64   
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2020 2020 2020 342e 3333 2d32            4.33-2
-000054d0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054f0: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-00005500: 6576 2d68 656c 702e 6161 7263 6836 3420  ev-help.aarch64 
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 2020 342e 3333              4.33
-00005530: 2d32 2e75 656c 3230 2020 2020 2020 2020  -2.uel20        
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005560: 6962 6576 656e 742e 6161 7263 6836 3420  ibevent.aarch64 
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2020 2020 2020 2020 2020 2020 322e 312e              2.1.
-00005590: 3132 2d33 2e75 656c 3230 2020 2020 2020  12-3.uel20      
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000055c0: 0a6c 6962 6661 7374 6a73 6f6e 2e61 6172  .libfastjson.aar
-000055d0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2030 2e39 392e 382d 332e 7565 6c32 3020   0.99.8-3.uel20 
-00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005610: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00005620: 636f 6e64 610a 6c69 6266 6469 736b 2e61  conda.libfdisk.a
-00005630: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2032 2e33 352e 322d 362e 7570 312e     2.35.2-6.up1.
-00005660: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 4061 6e61 636f 6e64 610a 6c69 6266    @anaconda.libf
-00005690: 6669 2e61 6172 6368 3634 2020 2020 2020  fi.aarch64      
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2020 2020 2033 2e33 2d37 2e75 656c         3.3-7.uel
-000056c0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-000056e0: 616e 6163 6f6e 6461 0a6c 6962 6763 632e  anaconda.libgcc.
-000056f0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 372e 332e 302d 3230 3231 3036      7.3.0-202106
-00005720: 3035 2e33 392e 7565 6c32 3020 2020 2020  05.39.uel20     
-00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005740: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00005750: 610a 6c69 6267 6372 7970 742e 6161 7263  a.libgcrypt.aarc
-00005760: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 312e 382e 362d 332e 7565 6c32 3020 2020  1.8.6-3.uel20   
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-000057b0: 6e64 610a 6c69 6267 6f6d 702e 6161 7263  nda.libgomp.aarc
-000057c0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 372e 332e 302d 3230 3231 3036 3035 2e33  7.3.0-20210605.3
-000057f0: 392e 7565 6c32 3020 2020 2020 2020 2020  9.uel20         
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005810: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00005820: 6267 7067 2d65 7272 6f72 2e61 6172 6368  bgpg-error.aarch
-00005830: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00005840: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00005850: 2e33 382d 312e 7565 6c32 3020 2020 2020  .38-1.uel20     
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00005880: 610a 6c69 6267 7564 6576 2e61 6172 6368  a.libgudev.aarch
-00005890: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-000058b0: 3333 2d31 2e75 656c 3230 2020 2020 2020  33-1.uel20      
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000058e0: 0a6c 6962 6775 7362 2e61 6172 6368 3634  .libgusb.aarch64
-000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005900: 2020 2020 2020 2020 2020 2020 2030 2e33               0.3
-00005910: 2e34 2d31 2e75 656c 3230 2020 2020 2020  .4-1.uel20      
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005930: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00005940: 0a6c 6962 6963 616c 2e61 6172 6368 3634  .libical.aarch64
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 2020 2020 2020 2020 2020 2033 2e30               3.0
-00005970: 2e38 2d31 2e75 656c 3230 2020 2020 2020  .8-1.uel20      
-00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005990: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000059a0: 0a6c 6962 6963 752e 6161 7263 6836 3420  .libicu.aarch64 
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2020 2020 2020 2020 3632 2e31              62.1
-000059d0: 2d35 2e75 656c 3230 2020 2020 2020 2020  -5.uel20        
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005a00: 6962 6964 6e32 2e61 6172 6368 3634 2020  ibidn2.aarch64  
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 2020 2020 2020 2020 2020 2032 2e33 2e30             2.3.0
-00005a30: 2d33 2e75 656c 3230 2020 2020 2020 2020  -3.uel20        
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00005a60: 6962 6a70 6567 2d74 7572 626f 2e61 6172  ibjpeg-turbo.aar
-00005a70: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2032 2e30 2e35 2d31 2e75 7031 2e75 656c   2.0.5-1.up1.uel
-00005aa0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00005ac0: 616e 6163 6f6e 6461 0a6c 6962 6b63 6170  anaconda.libkcap
-00005ad0: 692e 6161 7263 6836 3420 2020 2020 2020  i.aarch64       
-00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005af0: 2020 2020 2020 312e 322e 302d 342e 7565        1.2.0-4.ue
-00005b00: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 4061 6e61 636f 6e64 610a 6c69 626b 7362  @anaconda.libksb
-00005b30: 612e 6161 7263 6836 3420 2020 2020 2020  a.aarch64       
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2020 312e 342e 302d 322e 7565        1.4.0-2.ue
-00005b60: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b80: 4061 6e61 636f 6e64 610a 6c69 626d 6574  @anaconda.libmet
-00005b90: 616c 696e 6b2e 6161 7263 6836 3420 2020  alink.aarch64   
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 2020 2020 2020 2020 302e 312e 332d            0.1.3-
-00005bc0: 382e 7565 6c32 3020 2020 2020 2020 2020  8.uel20         
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00005bf0: 626d 6e6c 2e61 6172 6368 3634 2020 2020  bmnl.aarch64    
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c10: 2020 2020 2020 2020 2031 2e30 2e34 2d31           1.0.4-1
-00005c20: 302e 7565 6c32 3020 2020 2020 2020 2020  0.uel20         
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00005c50: 626d 6f64 756c 656d 642e 6161 7263 6836  bmodulemd.aarch6
-00005c60: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00005c70: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-00005c80: 392e 342d 312e 7565 6c32 3020 2020 2020  9.4-1.uel20     
-00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ca0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00005cb0: 610a 6c69 626d 6f75 6e74 2e61 6172 6368  a.libmount.aarch
-00005cc0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
-00005ce0: 2e33 352e 322d 362e 7570 312e 7565 6c32  .35.2-6.up1.uel2
-00005cf0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00005d00: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00005d10: 6e61 636f 6e64 610a 6c69 626d 7063 2e61  naconda.libmpc.a
-00005d20: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d40: 2020 2031 2e32 2e30 2d31 2e75 656c 3230     1.2.0-1.uel20
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d60: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00005d70: 6163 6f6e 6461 0a6c 6962 6e64 702e 6161  aconda.libndp.aa
-00005d80: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2020 312e 372d 332e 7565 6c32 3020 2020    1.7-3.uel20   
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00005dd0: 6e64 610a 6c69 626e 6574 2e61 6172 6368  nda.libnet.aarch
-00005de0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00005e00: 2e32 2d31 2e75 656c 3230 2020 2020 2020  .2-1.uel20      
-00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e20: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00005e30: 0a6c 6962 6e65 7466 696c 7465 725f 636f  .libnetfilter_co
-00005e40: 6e6e 7472 6163 6b2e 6161 7263 6836 3420  nntrack.aarch64 
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 2020 2020 2020 2020 2020 312e 302e              1.0.
-00005e70: 382d 312e 7565 6c32 3020 2020 2020 2020  8-1.uel20       
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00005ea0: 6c69 626e 666e 6574 6c69 6e6b 2e61 6172  libnfnetlink.aar
-00005eb0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2031 2e30 2e31 2d31 352e 7565 6c32 3020   1.0.1-15.uel20 
-00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ef0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00005f00: 636f 6e64 610a 6c69 626e 6674 6e6c 2e61  conda.libnftnl.a
-00005f10: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2031 2e31 2e37 2d31 2e75 656c 3230     1.1.7-1.uel20
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f50: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00005f60: 6163 6f6e 6461 0a6c 6962 6e67 6874 7470  aconda.libnghttp
-00005f70: 322e 6161 7263 6836 3420 2020 2020 2020  2.aarch64       
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 312e 3431 2e30 2d32 2e75        1.41.0-2.u
-00005fa0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 2040 616e 6163 6f6e 6461 0a6c 6962 6e6c   @anaconda.libnl
-00005fd0: 332e 6161 7263 6836 3420 2020 2020 2020  3.aarch64       
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 332e 352e 302d 342e 7565        3.5.0-4.ue
-00006000: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006020: 4061 6e61 636f 6e64 610a 6c69 626e 6c33  @anaconda.libnl3
-00006030: 2d68 656c 702e 6161 7263 6836 3420 2020  -help.aarch64   
-00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006050: 2020 2020 2020 2020 2020 332e 352e 302d            3.5.0-
-00006060: 342e 7565 6c32 3020 2020 2020 2020 2020  4.uel20         
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00006090: 626e 736c 322e 6161 7263 6836 3420 2020  bnsl2.aarch64   
-000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2020 2020 2020 2020 2020 312e 332e 302d            1.3.0-
-000060c0: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-000060f0: 6270 6361 702e 6161 7263 6836 3420 2020  bpcap.aarch64   
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2020 2020 2020 2020 2020 3134 3a31 2e39            14:1.9
-00006120: 2e31 2d36 2e75 656c 3230 2020 2020 2020  .1-6.uel20      
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00006150: 0a6c 6962 7069 7065 6c69 6e65 2e61 6172  .libpipeline.aar
-00006160: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2031 2e35 2e32 2d31 2e75 656c 3230 2020   1.5.2-1.uel20  
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000061b0: 6f6e 6461 0a6c 6962 706e 672e 6161 7263  onda.libpng.aarc
-000061c0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 323a 312e 362e 3337 2d31 2e75 656c 3230  2:1.6.37-1.uel20
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00006210: 6163 6f6e 6461 0a6c 6962 7072 6f78 792e  aconda.libproxy.
-00006220: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00006230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006240: 2020 2020 302e 342e 3135 2d31 372e 7565      0.4.15-17.ue
-00006250: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 4061 6e61 636f 6e64 610a 6c69 6270 736c  @anaconda.libpsl
-00006280: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2030 2e32 312e 312d 312e 7565       0.21.1-1.ue
-000062b0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 4061 6e61 636f 6e64 610a 6c69 6270 7771  @anaconda.libpwq
-000062e0: 7561 6c69 7479 2e61 6172 6368 3634 2020  uality.aarch64  
-000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006300: 2020 2020 2020 2020 2020 2031 2e34 2e32             1.4.2
-00006310: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00006340: 6962 7265 706f 2e61 6172 6368 3634 2020  ibrepo.aarch64  
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 2020 2020 2020 2031 2e31 322e             1.12.
-00006370: 302d 332e 7565 6c32 3020 2020 2020 2020  0-3.uel20       
-00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000063a0: 6c69 6272 6570 6f72 742d 6669 6c65 7379  libreport-filesy
-000063b0: 7374 656d 2e6e 6f61 7263 6820 2020 2020  stem.noarch     
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063d0: 2020 2020 2020 2020 322e 3130 2e31 2d31          2.10.1-1
-000063e0: 302e 7565 6c32 3020 2020 2020 2020 2020  0.uel20         
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00006410: 6273 6563 636f 6d70 2e61 6172 6368 3634  bseccomp.aarch64
-00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2020 2020 2020 2020 2020 2020 2032 2e35               2.5
-00006440: 2e30 2d33 2e75 656c 3230 2020 2020 2020  .0-3.uel20      
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00006470: 0a6c 6962 7365 6363 6f6d 702d 6865 6c70  .libseccomp-help
-00006480: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-00006490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064a0: 2020 2020 322e 352e 302d 332e 7565 6c32      2.5.0-3.uel2
-000064b0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000064c0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000064d0: 6e61 636f 6e64 610a 6c69 6273 6563 7265  naconda.libsecre
-000064e0: 742e 6161 7263 6836 3420 2020 2020 2020  t.aarch64       
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2020 2020 2020 302e 3230 2e33 2d31 2e75        0.20.3-1.u
-00006510: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2040 616e 6163 6f6e 6461 0a6c 6962 7365   @anaconda.libse
-00006540: 6c69 6e75 782e 6161 7263 6836 3420 2020  linux.aarch64   
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2020 2020 2020 2020 2020 332e 312d 332e            3.1-3.
-00006570: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 4061 6e61 636f 6e64 610a 6c69 6273    @anaconda.libs
-000065a0: 656d 616e 6167 652e 6161 7263 6836 3420  emanage.aarch64 
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2020 2020 2020 2020 2020 2020 332e 312d              3.1-
-000065d0: 332e 7565 6c32 3020 2020 2020 2020 2020  3.uel20         
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00006600: 6273 6570 6f6c 2e61 6172 6368 3634 2020  bsepol.aarch64  
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 2020 2020 2020 2020 2033 2e31 2d34             3.1-4
-00006630: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-00006660: 7369 6773 6567 762e 6161 7263 6836 3420  sigsegv.aarch64 
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 2020 2020 2020 2020 2020 322e 3132              2.12
-00006690: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066b0: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-000066c0: 6962 736d 6172 7463 6f6c 732e 6161 7263  ibsmartcols.aarc
-000066d0: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 322e 3335 2e32 2d36 2e75 7031 2e75 656c  2.35.2-6.up1.uel
-00006700: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00006710: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00006720: 616e 6163 6f6e 6461 0a6c 6962 736f 6c76  anaconda.libsolv
-00006730: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 2020 2030 2e37 2e31 342d 332e 7565       0.7.14-3.ue
-00006760: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 4061 6e61 636f 6e64 610a 6c69 6273 6f6c  @anaconda.libsol
-00006790: 762d 6865 6c70 2e6e 6f61 7263 6820 2020  v-help.noarch   
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 2020 2020 2020 302e 372e 3134            0.7.14
-000067c0: 2d33 2e75 656c 3230 2020 2020 2020 2020  -3.uel20        
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-000067f0: 6962 736f 7570 2e61 6172 6368 3634 2020  ibsoup.aarch64  
-00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 2020 2020 2020 2020 2020 2032 2e37 312e             2.71.
-00006820: 302d 322e 7565 6c32 3020 2020 2020 2020  0-2.uel20       
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00006850: 6c69 6273 7368 2e61 6172 6368 3634 2020  libssh.aarch64  
-00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 2020 2020 2020 2020 2030 2e39 2e34             0.9.4
-00006880: 2d33 2e75 656c 3230 2020 2020 2020 2020  -3.uel20        
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-000068b0: 6962 7373 682d 6865 6c70 2e6e 6f61 7263  ibssh-help.noarc
-000068c0: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-000068d0: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-000068e0: 392e 342d 332e 7565 6c32 3020 2020 2020  9.4-3.uel20     
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00006910: 610a 6c69 6273 7464 632b 2b2e 6161 7263  a.libstdc++.aarc
-00006920: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 372e 332e 302d 3230 3231 3036 3035 2e33  7.3.0-20210605.3
-00006950: 392e 7565 6c32 3020 2020 2020 2020 2020  9.uel20         
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00006980: 6274 6173 6e31 2e61 6172 6368 3634 2020  btasn1.aarch64  
-00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2020 2034 2e31 362e             4.16.
-000069b0: 302d 312e 7565 6c32 3020 2020 2020 2020  0-1.uel20       
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000069e0: 6c69 6274 6561 6d2e 6161 7263 6836 3420  libteam.aarch64 
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2020 2020 2020 2020 2020 2020 312e 3330              1.30
-00006a10: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00006a40: 6962 7468 6169 2e61 6172 6368 3634 2020  ibthai.aarch64  
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 2020 2020 2020 2020 2020 2030 2e31 2e32             0.1.2
-00006a70: 382d 342e 7565 6c32 3020 2020 2020 2020  8-4.uel20       
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00006aa0: 6c69 6274 6966 662e 6161 7263 6836 3420  libtiff.aarch64 
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 2020 2020 2020 2020 2020 2020 342e 312e              4.1.
-00006ad0: 302d 332e 7565 6c32 3020 2020 2020 2020  0-3.uel20       
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00006b00: 6c69 6274 6972 7063 2e61 6172 6368 3634  libtirpc.aarch64
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 2020 2020 2031 2e32               1.2
-00006b30: 2e36 2d31 2e75 656c 3230 2020 2020 2020  .6-1.uel20      
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00006b60: 0a6c 6962 746f 6f6c 2d6c 7464 6c2e 6161  .libtool-ltdl.aa
-00006b70: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 322e 342e 362d 3333 2e75 656c 3230    2.4.6-33.uel20
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00006bc0: 6163 6f6e 6461 0a6c 6962 7564 6973 6b73  aconda.libudisks
-00006bd0: 322e 6161 7263 6836 3420 2020 2020 2020  2.aarch64       
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 2020 322e 392e 302d 322e 7570        2.9.0-2.up
-00006c00: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c20: 2020 2020 4061 6e61 636f 6e64 610a 6c69      @anaconda.li
-00006c30: 6275 6e69 7374 7269 6e67 2e61 6172 6368  bunistring.aarch
-00006c40: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00006c60: 2e39 2e31 302d 382e 7565 6c32 3020 2020  .9.10-8.uel20   
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00006c90: 6e64 610a 6c69 6275 6f73 6465 7669 6365  nda.libuosdevice
-00006ca0: 632d 6c69 6273 2e61 6172 6368 3634 2020  c-libs.aarch64  
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 2020 2020 2020 2020 2031 2e30 2e30             1.0.0
-00006cd0: 2e38 2d32 2e75 656c 3230 2020 2020 2020  .8-2.uel20      
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cf0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00006d00: 0a6c 6962 7573 6278 2e61 6172 6368 3634  .libusbx.aarch64
-00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 2020 2020 2020 2031 2e30               1.0
-00006d30: 2e32 332d 312e 7565 6c32 3020 2020 2020  .23-1.uel20     
-00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d50: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00006d60: 610a 6c69 6275 7365 722e 6161 7263 6836  a.libuser.aarch6
-00006d70: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00006d80: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-00006d90: 3632 2d32 312e 7565 6c32 3020 2020 2020  62-21.uel20     
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006db0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00006dc0: 610a 6c69 6275 7465 6d70 7465 722e 6161  a.libutempter.aa
-00006dd0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 2020 312e 322e 312d 322e 7565 6c32 3020    1.2.1-2.uel20 
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00006e20: 636f 6e64 610a 6c69 6275 7569 642e 6161  conda.libuuid.aa
-00006e30: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 322e 3335 2e32 2d36 2e75 7031 2e75    2.35.2-6.up1.u
-00006e60: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 2040 616e 6163 6f6e 6461 0a6c 6962 7665   @anaconda.libve
-00006e90: 7274 6f2e 6161 7263 6836 3420 2020 2020  rto.aarch64     
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 2020 2020 302e 332e 312d 322e          0.3.1-2.
-00006ec0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ee0: 2020 4061 6e61 636f 6e64 610a 6c69 6278    @anaconda.libx
-00006ef0: 6362 2e61 6172 6368 3634 2020 2020 2020  cb.aarch64      
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 2020 2031 2e31 342d 312e 7565         1.14-1.ue
-00006f20: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 4061 6e61 636f 6e64 610a 6c69 6278 6372  @anaconda.libxcr
-00006f50: 7970 742e 6161 7263 6836 3420 2020 2020  ypt.aarch64     
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 342e 342e 3136 2d31          4.4.16-1
-00006f80: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-00006fb0: 7863 7279 7074 2d64 6576 656c 2e61 6172  xcrypt-devel.aar
-00006fc0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2034 2e34 2e31 362d 312e 7565 6c32 3020   4.4.16-1.uel20 
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00007010: 636f 6e64 610a 6c69 6278 6b62 636f 6d6d  conda.libxkbcomm
-00007020: 6f6e 2e61 6172 6368 3634 2020 2020 2020  on.aarch64      
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 2020 2030 2e38 2e34 2d36 2e75         0.8.4-6.u
-00007050: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 2040 616e 6163 6f6e 6461 0a6c 6962 786d   @anaconda.libxm
-00007080: 6c32 2e61 6172 6368 3634 2020 2020 2020  l2.aarch64      
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2032 2e39 2e31 302d 3136         2.9.10-16
-000070b0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2040 616e 6163 6f6e 6461 0a6c 6962     @anaconda.lib
-000070e0: 786d 6c32 2d68 656c 702e 6e6f 6172 6368  xml2-help.noarch
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007100: 2020 2020 2020 2020 2020 2020 2032 2e39               2.9
-00007110: 2e31 302d 3136 2e75 656c 3230 2020 2020  .10-16.uel20    
-00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00007140: 6461 0a6c 6962 7961 6d6c 2e61 6172 6368  da.libyaml.aarch
-00007150: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00007160: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00007170: 2e32 2e35 2d31 2e75 656c 3230 2020 2020  .2.5-1.uel20    
-00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000071a0: 6461 0a6c 6963 656e 7365 2d63 6f6e 6669  da.license-confi
-000071b0: 672e 6161 7263 6836 3420 2020 2020 2020  g.aarch64       
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2020 2020 3230 3231 2e30 352e 3234        2021.05.24
-000071e0: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007200: 2020 2020 2040 616e 6163 6f6e 6461 0a6c       @anaconda.l
-00007210: 696e 7578 2d66 6972 6d77 6172 652e 6e6f  inux-firmware.no
-00007220: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007240: 2032 3032 3030 3831 372d 322e 7565 6c32   20200817-2.uel2
-00007250: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00007260: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00007270: 6e61 636f 6e64 610a 6c6f 6772 6f74 6174  naconda.logrotat
-00007280: 652e 6161 7263 6836 3420 2020 2020 2020  e.aarch64       
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2020 2020 332e 3136 2e30 2d31 2e75        3.16.0-1.u
-000072b0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2040 616e 6163 6f6e 6461 0a6c 7368 772e   @anaconda.lshw.
-000072e0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 422e 3032 2e31 382d 3231 2e75      B.02.18-21.u
-00007310: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2040 616e 6163 6f6e 6461 0a6c 7373 6373   @anaconda.lsscs
-00007340: 692e 6161 7263 6836 3420 2020 2020 2020  i.aarch64       
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 2020 302e 3330 2d32 2e75 656c        0.30-2.uel
-00007370: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00007380: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00007390: 616e 6163 6f6e 6461 0a6c 7561 2e61 6172  anaconda.lua.aar
-000073a0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2035 2e33 2e35 2d34 2e75 656c 3230 2020   5.3.5-4.uel20  
-000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073e0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000073f0: 6f6e 6461 0a6c 766d 322e 6161 7263 6836  onda.lvm2.aarch6
-00007400: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00007410: 2020 2020 2020 2020 2020 2020 2020 383a                8:
-00007420: 322e 3033 2e30 392d 352e 7570 312e 7565  2.03.09-5.up1.ue
-00007430: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007450: 4061 6e61 636f 6e64 610a 6c76 6d32 2d64  @anaconda.lvm2-d
-00007460: 6275 7364 2e61 6172 6368 3634 2020 2020  busd.aarch64    
-00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007480: 2020 2020 2020 2020 2038 3a32 2e30 332e           8:2.03.
-00007490: 3039 2d35 2e75 7031 2e75 656c 3230 2020  09-5.up1.uel20  
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000074c0: 6f6e 6461 0a6c 766d 322d 6865 6c70 2e6e  onda.lvm2-help.n
-000074d0: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 383a 322e 3033 2e30 392d 352e 7570    8:2.03.09-5.up
-00007500: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 4061 6e61 636f 6e64 610a 6c7a      @anaconda.lz
-00007530: 342e 6161 7263 6836 3420 2020 2020 2020  4.aarch64       
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 312e 392e 322d 332e 7565        1.9.2-3.ue
-00007560: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007580: 4061 6e61 636f 6e64 610a 6c7a 6f2e 6161  @anaconda.lzo.aa
-00007590: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075b0: 2020 322e 3130 2d31 2e75 656c 3230 2020    2.10-1.uel20  
-000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075d0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000075e0: 6f6e 6461 0a6d 616b 652e 6161 7263 6836  onda.make.aarch6
-000075f0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00007600: 2020 2020 2020 2020 2020 2020 2020 313a                1:
-00007610: 342e 332d 312e 7565 6c32 3020 2020 2020  4.3-1.uel20     
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00007640: 610a 6d61 6e2d 6462 2e61 6172 6368 3634  a.man-db.aarch64
-00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2020 2020 2020 2020 2020 2032 2e38               2.8
-00007670: 2e37 2d36 2e75 656c 3230 2020 2020 2020  .7-6.uel20      
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000076a0: 0a6d 6172 6961 6462 2d63 6f6e 6e65 6374  .mariadb-connect
-000076b0: 6f72 2d63 2e61 6172 6368 3634 2020 2020  or-c.aarch64    
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2020 2020 2033 2e30 2e36 2d37           3.0.6-7
-000076e0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2040 616e 6163 6f6e 6461 0a6d 6461     @anaconda.mda
-00007710: 646d 2e61 6172 6368 3634 2020 2020 2020  dm.aarch64      
-00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 2020 2020 2034 2e31 2d72 6332 2e30         4.1-rc2.0
-00007740: 2e39 2e75 656c 3230 2020 2020 2020 2020  .9.uel20        
-00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007760: 2020 2020 2040 616e 6163 6f6e 6461 0a6d       @anaconda.m
-00007770: 6f6b 7574 696c 2e61 6172 6368 3634 2020  okutil.aarch64  
-00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007790: 2020 2020 2020 2020 2020 2031 3a30 2e34             1:0.4
-000077a0: 2e30 2d31 2e75 656c 3230 2020 2020 2020  .0-1.uel20      
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000077d0: 0a6d 6f7a 6a73 3738 2e61 6172 6368 3634  .mozjs78.aarch64
-000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077f0: 2020 2020 2020 2020 2020 2020 2037 382e               78.
-00007800: 342e 302d 322e 7565 6c32 3020 2020 2020  4.0-2.uel20     
-00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00007830: 610a 6d70 6672 2e61 6172 6368 3634 2020  a.mpfr.aarch64  
-00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2020 2020 2034 2e31 2e30             4.1.0
-00007860: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 2020 2020 2040 616e 6163 6f6e 6461 0a6d       @anaconda.m
-00007890: 756c 7469 7061 7468 2d74 6f6f 6c73 2e61  ultipath-tools.a
-000078a0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2030 2e38 2e34 2d36 2e75 7031 2e75     0.8.4-6.up1.u
-000078d0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2040 616e 6163 6f6e 6461 0a6d 756c 7469   @anaconda.multi
-00007900: 7061 7468 2d74 6f6f 6c73 2d68 656c 702e  path-tools-help.
-00007910: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 2020 302e 382e 342d 362e 7570 312e      0.8.4-6.up1.
-00007940: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 4061 6e61 636f 6e64 610a 6e63 7572    @anaconda.ncur
-00007970: 7365 732e 6161 7263 6836 3420 2020 2020  ses.aarch64     
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 2020 362e 322d 312e 7565          6.2-1.ue
-000079a0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 4061 6e61 636f 6e64 610a 6e63 7572 7365  @anaconda.ncurse
-000079d0: 732d 6261 7365 2e6e 6f61 7263 6820 2020  s-base.noarch   
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2020 2020 362e 322d 312e            6.2-1.
-00007a00: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 4061 6e61 636f 6e64 610a 6e63 7572    @anaconda.ncur
-00007a30: 7365 732d 6c69 6273 2e61 6172 6368 3634  ses-libs.aarch64
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 2020 2020 2020 2020 2020 2020 2036 2e32               6.2
-00007a60: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 2020 2040 616e 6163 6f6e 6461 0a6e       @anaconda.n
-00007a90: 6463 746c 2e61 6172 6368 3634 2020 2020  dctl.aarch64    
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 2020 2020 2036 382d 312e 7565           68-1.ue
-00007ac0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 4061 6e61 636f 6e64 610a 6e64 6374 6c2d  @anaconda.ndctl-
-00007af0: 6c69 6273 2e61 6172 6368 3634 2020 2020  libs.aarch64    
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2020 2020 2020 2036 382d 312e 7565           68-1.ue
-00007b20: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 4061 6e61 636f 6e64 610a 6e65 742d 736e  @anaconda.net-sn
-00007b50: 6d70 2d6c 6962 732e 6161 7263 6836 3420  mp-libs.aarch64 
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2020 2020 313a 352e              1:5.
-00007b80: 392d 332e 7570 312e 7565 6c32 3020 2020  9-3.up1.uel20   
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00007bb0: 6e64 610a 6e65 7474 6c65 2e61 6172 6368  nda.nettle.aarch
-00007bc0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-00007be0: 2e36 2d32 2e75 656c 3230 2020 2020 2020  .6-2.uel20      
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00007c10: 0a6e 6577 742e 6161 7263 6836 3420 2020  .newt.aarch64   
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 2020 302e 3532 2e32            0.52.2
-00007c40: 312d 352e 7565 6c32 3020 2020 2020 2020  1-5.uel20       
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00007c70: 6e66 7461 626c 6573 2e61 6172 6368 3634  nftables.aarch64
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 2020 2020 2031 3a30               1:0
-00007ca0: 2e39 2e36 2d32 2e75 656c 3230 2020 2020  .9.6-2.uel20    
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00007cd0: 6461 0a6e 6674 6162 6c65 732d 6865 6c70  da.nftables-help
-00007ce0: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 313a 302e 392e 362d 322e 7565      1:0.9.6-2.ue
-00007d10: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 4061 6e61 636f 6e64 610a 6e70 7468 2e61  @anaconda.npth.a
-00007d40: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 2020 2031 2e36 2d31 2e75 656c 3230 2020     1.6-1.uel20  
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00007d90: 6f6e 6461 0a6e 7370 722e 6161 7263 6836  onda.nspr.aarch6
-00007da0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00007db0: 2020 2020 2020 2020 2020 2020 2020 342e                4.
-00007dc0: 3236 2e30 2d32 2e75 656c 3230 2020 2020  26.0-2.uel20    
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00007df0: 6461 0a6e 7373 2e61 6172 6368 3634 2020  da.nss.aarch64  
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 2020 2020 2020 2020 2033 2e35 342e             3.54.
-00007e20: 302d 372e 7565 6c32 3020 2020 2020 2020  0-7.uel20       
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00007e50: 6e73 732d 6865 6c70 2e61 6172 6368 3634  nss-help.aarch64
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 2020 2020 2020 2020 2033 2e35               3.5
-00007e80: 342e 302d 372e 7565 6c32 3020 2020 2020  4.0-7.uel20     
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00007eb0: 610a 6e73 732d 736f 6674 6f6b 6e2e 6161  a.nss-softokn.aa
-00007ec0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 332e 3534 2e30 2d37 2e75 656c 3230    3.54.0-7.uel20
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00007f10: 6163 6f6e 6461 0a6e 7373 2d75 7469 6c2e  aconda.nss-util.
-00007f20: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 332e 3534 2e30 2d37 2e75 656c      3.54.0-7.uel
-00007f50: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00007f60: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00007f70: 616e 6163 6f6e 6461 0a6e 756d 6163 746c  anaconda.numactl
-00007f80: 2d6c 6962 732e 6161 7263 6836 3420 2020  -libs.aarch64   
-00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2020 2020 2020 2020 322e 302e 3133            2.0.13
-00007fb0: 2d34 2e75 656c 3230 2020 2020 2020 2020  -4.uel20        
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2020 2040 616e 6163 6f6e 6461 0a6f       @anaconda.o
-00007fe0: 7065 6e6c 6461 702e 6161 7263 6836 3420  penldap.aarch64 
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008000: 2020 2020 2020 2020 2020 2020 322e 342e              2.4.
-00008010: 3530 2d37 2e75 656c 3230 2020 2020 2020  50-7.uel20      
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00008040: 0a6f 7065 6e73 7368 2e61 6172 6368 3634  .openssh.aarch64
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 2020 2020 2038 2e32               8.2
-00008070: 7031 2d31 302e 7570 342e 7565 6c32 3020  p1-10.up4.uel20 
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008090: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-000080a0: 636f 6e64 610a 6f70 656e 7373 682d 636c  conda.openssh-cl
-000080b0: 6965 6e74 732e 6161 7263 6836 3420 2020  ients.aarch64   
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 2020 382e 3270 312d            8.2p1-
-000080e0: 3130 2e75 7034 2e75 656c 3230 2020 2020  10.up4.uel20    
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008110: 6461 0a6f 7065 6e73 7368 2d68 656c 702e  da.openssh-help.
-00008120: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2038 2e32 7031 2d31 302e 7570 342e     8.2p1-10.up4.
-00008150: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 4061 6e61 636f 6e64 610a 6f70 656e    @anaconda.open
-00008180: 7373 682d 7365 7276 6572 2e61 6172 6368  ssh-server.aarch
-00008190: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2038                 8
-000081b0: 2e32 7031 2d31 302e 7570 342e 7565 6c32  .2p1-10.up4.uel2
-000081c0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-000081d0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000081e0: 6e61 636f 6e64 610a 6f73 2d70 726f 6265  naconda.os-probe
-000081f0: 722e 6161 7263 6836 3420 2020 2020 2020  r.aarch64       
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2020 2020 2020 312e 3737 2d32 2e75 656c        1.77-2.uel
-00008220: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00008230: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00008240: 616e 6163 6f6e 6461 0a70 3131 2d6b 6974  anaconda.p11-kit
-00008250: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008270: 2020 2020 2030 2e32 332e 3230 2d32 2e75       0.23.20-2.u
-00008280: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082a0: 2040 616e 6163 6f6e 6461 0a70 3131 2d6b   @anaconda.p11-k
-000082b0: 6974 2d74 7275 7374 2e61 6172 6368 3634  it-trust.aarch64
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 2020 2020 2020 2030 2e32               0.2
-000082e0: 332e 3230 2d32 2e75 656c 3230 2020 2020  3.20-2.uel20    
-000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008300: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008310: 6461 0a70 616d 2e61 6172 6368 3634 2020  da.pam.aarch64  
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 2020 2031 2e34 2e30             1.4.0
-00008340: 2d35 2e75 7032 2e75 656c 3230 2020 2020  -5.up2.uel20    
-00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008360: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008370: 6461 0a70 616e 676f 2e61 6172 6368 3634  da.pango.aarch64
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 2020 2020 2020 2020 2020 2031 2e34               1.4
-000083a0: 342e 372d 332e 7565 6c32 3020 2020 2020  4.7-3.uel20     
-000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083c0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-000083d0: 610a 7061 7274 6564 2e61 6172 6368 3634  a.parted.aarch64
-000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2020 2020 2020 2020 2020 2033 2e33               3.3
-00008400: 2d36 2e75 656c 3230 2020 2020 2020 2020  -6.uel20        
-00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008420: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00008430: 6173 7377 642e 6161 7263 6836 3420 2020  asswd.aarch64   
-00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 2020 2020 2020 2020 302e 3830 2d37            0.80-7
-00008460: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2040 616e 6163 6f6e 6461 0a70 6369     @anaconda.pci
-00008490: 7574 696c 732e 6161 7263 6836 3420 2020  utils.aarch64   
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2020 2020 2020 332e 362e 342d            3.6.4-
-000084c0: 342e 7565 6c32 3020 2020 2020 2020 2020  4.uel20         
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2020 2020 4061 6e61 636f 6e64 610a 7063      @anaconda.pc
-000084f0: 7265 2e61 6172 6368 3634 2020 2020 2020  re.aarch64      
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2020 2020 2038 2e34 342d 322e 7565         8.44-2.ue
-00008520: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 4061 6e61 636f 6e64 610a 7063 7265 322e  @anaconda.pcre2.
-00008550: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 3130 2e33 352d 312e 7565 6c32      10.35-1.uel2
-00008580: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00008590: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-000085a0: 6e61 636f 6e64 610a 7065 726c 2e61 6172  naconda.perl.aar
-000085b0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2034 3a35 2e32 382e 332d 362e 7570 312e   4:5.28.3-6.up1.
-000085e0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-00008610: 2d41 6c67 6f72 6974 686d 2d44 6966 662e  -Algorithm-Diff.
-00008620: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008640: 2020 2031 2e31 3930 332d 3134 2e75 656c     1.1903-14.uel
-00008650: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00008660: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00008670: 616e 6163 6f6e 6461 0a70 6572 6c2d 4172  anaconda.perl-Ar
-00008680: 6368 6976 652d 5461 722e 6e6f 6172 6368  chive-Tar.noarch
-00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086a0: 2020 2020 2020 2020 2020 2020 2032 2e33               2.3
-000086b0: 382d 312e 7565 6c32 3020 2020 2020 2020  8-1.uel20       
-000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086d0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000086e0: 7065 726c 2d42 2d44 6562 7567 2e6e 6f61  perl-B-Debug.noa
-000086f0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 312e 3236 2d34 2e75 656c 3230 2020 2020  1.26-4.uel20    
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008740: 6461 0a70 6572 6c2d 4350 414e 2d4d 6574  da.perl-CPAN-Met
-00008750: 612e 6e6f 6172 6368 2020 2020 2020 2020  a.noarch        
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2032 2e31 3530 3031 302d 3431       2.150010-41
-00008780: 392e 7565 6c32 3020 2020 2020 2020 2020  9.uel20         
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 4061 6e61 636f 6e64 610a 7065      @anaconda.pe
-000087b0: 726c 2d43 5041 4e2d 4d65 7461 2d52 6571  rl-CPAN-Meta-Req
-000087c0: 7569 7265 6d65 6e74 732e 6e6f 6172 6368  uirements.noarch
-000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087e0: 2020 2020 2020 2020 2020 2020 2032 2e31               2.1
-000087f0: 3430 2d34 3139 2e75 656c 3230 2020 2020  40-419.uel20    
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008820: 6461 0a70 6572 6c2d 4350 414e 2d4d 6574  da.perl-CPAN-Met
-00008830: 612d 5941 4d4c 2e6e 6f61 7263 6820 2020  a-YAML.noarch   
-00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008850: 2020 2020 2020 2020 2020 302e 3031 382d            0.018-
-00008860: 3432 302e 7565 6c32 3020 2020 2020 2020  420.uel20       
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00008890: 7065 726c 2d43 6172 702e 6e6f 6172 6368  perl-Carp.noarch
-000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088b0: 2020 2020 2020 2020 2020 2020 2031 2e35               1.5
-000088c0: 302d 3431 382e 7565 6c32 3020 2020 2020  0-418.uel20     
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-000088f0: 610a 7065 726c 2d43 6f6d 7072 6573 732d  a.perl-Compress-
-00008900: 5261 772d 427a 6970 322e 6161 7263 6836  Raw-Bzip2.aarch6
-00008910: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00008920: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-00008930: 3039 352d 312e 7565 6c32 3020 2020 2020  095-1.uel20     
-00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008950: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00008960: 610a 7065 726c 2d43 6f6d 7072 6573 732d  a.perl-Compress-
-00008970: 5261 772d 5a6c 6962 2e61 6172 6368 3634  Raw-Zlib.aarch64
-00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008990: 2020 2020 2020 2020 2020 2020 2031 3a32               1:2
-000089a0: 2e30 3935 2d31 2e75 656c 3230 2020 2020  .095-1.uel20    
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000089d0: 6461 0a70 6572 6c2d 436f 6e66 6967 2d50  da.perl-Config-P
-000089e0: 6572 6c2d 562e 6e6f 6172 6368 2020 2020  erl-V.noarch    
-000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a00: 2020 2020 2020 2020 2030 2e33 312d 312e           0.31-1.
-00008a10: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-00008a40: 2d44 6174 612d 4475 6d70 6572 2e61 6172  -Data-Dumper.aar
-00008a50: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2032 2e31 3733 2d31 2e75 656c 3230 2020   2.173-1.uel20  
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00008aa0: 6f6e 6461 0a70 6572 6c2d 4465 7665 6c2d  onda.perl-Devel-
-00008ab0: 5050 506f 7274 2e61 6172 6368 3634 2020  PPPort.aarch64  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2033 2e35 382d             3.58-
-00008ae0: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 4061 6e61 636f 6e64 610a 7065      @anaconda.pe
-00008b10: 726c 2d44 6967 6573 742e 6e6f 6172 6368  rl-Digest.noarch
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 2020 2020 2020 2020 2020 2031 2e31               1.1
-00008b40: 372d 3431 392e 7565 6c32 3020 2020 2020  7-419.uel20     
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b60: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00008b70: 610a 7065 726c 2d44 6967 6573 742d 4d44  a.perl-Digest-MD
-00008b80: 352e 6161 7263 6836 3420 2020 2020 2020  5.aarch64       
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ba0: 2020 2020 2020 322e 3535 2d34 3139 2e75        2.55-419.u
-00008bb0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bd0: 2040 616e 6163 6f6e 6461 0a70 6572 6c2d   @anaconda.perl-
-00008be0: 4469 6765 7374 2d53 4841 2e61 6172 6368  Digest-SHA.aarch
-00008bf0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00008c10: 3a36 2e30 322d 372e 7565 6c32 3020 2020  :6.02-7.uel20   
-00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c30: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00008c40: 6e64 610a 7065 726c 2d45 6e63 6f64 652e  nda.perl-Encode.
-00008c50: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 343a 332e 3036 2d31 2e75 656c      4:3.06-1.uel
-00008c80: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00008c90: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00008ca0: 616e 6163 6f6e 6461 0a70 6572 6c2d 456e  anaconda.perl-En
-00008cb0: 636f 6465 2d4c 6f63 616c 652e 6e6f 6172  code-Locale.noar
-00008cc0: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00008ce0: 2e30 352d 3132 2e75 656c 3230 2020 2020  .05-12.uel20    
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008d10: 6461 0a70 6572 6c2d 456e 636f 6465 2d64  da.perl-Encode-d
-00008d20: 6576 656c 2e61 6172 6368 3634 2020 2020  evel.aarch64    
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 2020 2020 2034 3a33 2e30 362d           4:3.06-
-00008d50: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2020 4061 6e61 636f 6e64 610a 7065      @anaconda.pe
-00008d80: 726c 2d45 6e76 2e6e 6f61 7263 6820 2020  rl-Env.noarch   
-00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008da0: 2020 2020 2020 2020 2020 312e 3034 2d33            1.04-3
-00008db0: 3937 2e75 656c 3230 2020 2020 2020 2020  97.uel20        
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00008de0: 6572 6c2d 4578 706f 7274 6572 2e6e 6f61  erl-Exporter.noa
-00008df0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e10: 352e 3734 2d31 2e75 656c 3230 2020 2020  5.74-1.uel20    
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00008e40: 6461 0a70 6572 6c2d 4578 7455 7469 6c73  da.perl-ExtUtils
-00008e50: 2d43 6f6d 6d61 6e64 2e6e 6f61 7263 6820  -Command.noarch 
-00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e70: 2020 2020 2020 2020 2020 2020 313a 372e              1:7.
-00008e80: 3436 2d31 2e75 656c 3230 2020 2020 2020  46-1.uel20      
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ea0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00008eb0: 0a70 6572 6c2d 4578 7455 7469 6c73 2d49  .perl-ExtUtils-I
-00008ec0: 6e73 7461 6c6c 2e6e 6f61 7263 6820 2020  nstall.noarch   
-00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ee0: 2020 2020 2020 2020 2020 322e 3136 2d31            2.16-1
-00008ef0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-00008f20: 6c2d 4578 7455 7469 6c73 2d4d 616b 654d  l-ExtUtils-MakeM
-00008f30: 616b 6572 2e6e 6f61 7263 6820 2020 2020  aker.noarch     
-00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f50: 2020 2020 2020 2020 313a 372e 3436 2d31          1:7.46-1
-00008f60: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-00008f90: 6c2d 4578 7455 7469 6c73 2d4d 616e 6966  l-ExtUtils-Manif
-00008fa0: 6573 742e 6e6f 6172 6368 2020 2020 2020  est.noarch      
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 2020 2020 2020 2031 3a31 2e37 322d 312e         1:1.72-1.
-00008fd0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ff0: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-00009000: 2d45 7874 5574 696c 732d 5061 7273 6558  -ExtUtils-ParseX
-00009010: 532e 6e6f 6172 6368 2020 2020 2020 2020  S.noarch        
-00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009030: 2020 2020 2032 3a33 2e33 352d 312e 7565       2:3.35-1.ue
-00009040: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 4061 6e61 636f 6e64 610a 7065 726c 2d46  @anaconda.perl-F
-00009070: 696c 652d 4665 7463 682e 6e6f 6172 6368  ile-Fetch.noarch
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2020 2020 2020 2020 2020 2030 2e35               0.5
-000090a0: 362d 342e 7565 6c32 3020 2020 2020 2020  6-4.uel20       
-000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090c0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000090d0: 7065 726c 2d46 696c 652d 486f 6d65 4469  perl-File-HomeDi
-000090e0: 722e 6e6f 6172 6368 2020 2020 2020 2020  r.noarch        
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2020 2020 2031 2e30 3034 2d34 2e75 656c       1.004-4.uel
-00009110: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00009120: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-00009130: 616e 6163 6f6e 6461 0a70 6572 6c2d 4669  anaconda.perl-Fi
-00009140: 6c65 2d50 6174 682e 6e6f 6172 6368 2020  le-Path.noarch  
-00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009160: 2020 2020 2020 2020 2020 2032 2e31 372d             2.17-
-00009170: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009190: 2020 2020 4061 6e61 636f 6e64 610a 7065      @anaconda.pe
-000091a0: 726c 2d46 696c 652d 5465 6d70 2e6e 6f61  rl-File-Temp.noa
-000091b0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 313a 302e 3233 302e 3930 302d 312e 7565  1:0.230.900-1.ue
-000091e0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009200: 4061 6e61 636f 6e64 610a 7065 726c 2d46  @anaconda.perl-F
-00009210: 696c 652d 5768 6963 682e 6e6f 6172 6368  ile-Which.noarch
-00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009230: 2020 2020 2020 2020 2020 2020 2031 2e32               1.2
-00009240: 332d 312e 7565 6c32 3020 2020 2020 2020  3-1.uel20       
-00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009260: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00009270: 7065 726c 2d46 696c 7465 722e 6161 7263  perl-Filter.aarc
-00009280: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 323a 312e 3630 2d31 2e75 656c 3230 2020  2:1.60-1.uel20  
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-000092d0: 6f6e 6461 0a70 6572 6c2d 4669 6c74 6572  onda.perl-Filter
-000092e0: 2d53 696d 706c 652e 6e6f 6172 6368 2020  -Simple.noarch  
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2020 2020 2020 2020 2020 2031 3a30 2e39             1:0.9
-00009310: 342d 312e 7565 6c32 3020 2020 2020 2020  4-1.uel20       
-00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009330: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00009340: 7065 726c 2d47 6574 6f70 742d 4c6f 6e67  perl-Getopt-Long
-00009350: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 2020 313a 322e 3531 2d31 2e75 656c      1:2.51-1.uel
-00009380: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-00009390: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-000093a0: 616e 6163 6f6e 6461 0a70 6572 6c2d 4854  anaconda.perl-HT
-000093b0: 5450 2d54 696e 792e 6e6f 6172 6368 2020  TP-Tiny.noarch  
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 2020 2020 2020 2030 2e30 3736             0.076
-000093e0: 2d33 2e75 656c 3230 2020 2020 2020 2020  -3.uel20        
-000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009400: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00009410: 6572 6c2d 494f 2d43 6f6d 7072 6573 732e  erl-IO-Compress.
-00009420: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009440: 2020 2032 2e30 3935 2d31 2e75 656c 3230     2.095-1.uel20
-00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009460: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00009470: 6163 6f6e 6461 0a70 6572 6c2d 494f 2d53  aconda.perl-IO-S
-00009480: 6f63 6b65 742d 4950 2e6e 6f61 7263 6820  ocket-IP.noarch 
-00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094a0: 2020 2020 2020 2020 2020 2020 302e 3339              0.39
-000094b0: 2d34 3230 2e75 656c 3230 2020 2020 2020  -420.uel20      
-000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-000094e0: 0a70 6572 6c2d 494f 2d53 6f63 6b65 742d  .perl-IO-Socket-
-000094f0: 5353 4c2e 6e6f 6172 6368 2020 2020 2020  SSL.noarch      
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2032 2e30 3638 2d31 2e75         2.068-1.u
-00009520: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009540: 2040 616e 6163 6f6e 6461 0a70 6572 6c2d   @anaconda.perl-
-00009550: 4950 432d 436d 642e 6e6f 6172 6368 2020  IPC-Cmd.noarch  
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 2020 2020 2020 2032 3a31 2e30             2:1.0
-00009580: 342d 342e 7565 6c32 3020 2020 2020 2020  4-4.uel20       
-00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095a0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-000095b0: 7065 726c 2d49 5043 2d53 7973 562e 6161  perl-IPC-SysV.aa
-000095c0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 322e 3038 2d31 2e75 656c 3230 2020    2.08-1.uel20  
-000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-00009610: 6f6e 6461 0a70 6572 6c2d 4950 432d 5379  onda.perl-IPC-Sy
-00009620: 7374 656d 2d53 696d 706c 652e 6e6f 6172  stem-Simple.noar
-00009630: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-00009640: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-00009650: 2e33 302d 312e 7565 6c32 3020 2020 2020  .30-1.uel20     
-00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009670: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-00009680: 610a 7065 726c 2d4a 534f 4e2d 5050 2e6e  a.perl-JSON-PP.n
-00009690: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 313a 342e 3035 2d31 2e75 656c 3230    1:4.05-1.uel20
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-000096e0: 6163 6f6e 6461 0a70 6572 6c2d 4c6f 6361  aconda.perl-Loca
-000096f0: 6c65 2d43 6f64 6573 2e6e 6f61 7263 6820  le-Codes.noarch 
-00009700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009710: 2020 2020 2020 2020 2020 2020 332e 3630              3.60
-00009720: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00009750: 6572 6c2d 4c6f 6361 6c65 2d4d 616b 6574  erl-Locale-Maket
-00009760: 6578 742e 6e6f 6172 6368 2020 2020 2020  ext.noarch      
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009780: 2020 2020 2020 2031 3a31 2e32 392d 312e         1:1.29-1.
-00009790: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-000097c0: 2d4d 494d 452d 4261 7365 3634 2e61 6172  -MIME-Base64.aar
-000097d0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 2033 2e31 352d 3431 392e 7565 6c32 3020   3.15-419.uel20 
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-00009820: 636f 6e64 610a 7065 726c 2d4d 6174 682d  conda.perl-Math-
-00009830: 4269 6749 6e74 2e6e 6f61 7263 6820 2020  BigInt.noarch   
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 2020 313a 312e 3939            1:1.99
-00009860: 3938 2e31 382d 312e 7565 6c32 3020 2020  98.18-1.uel20   
-00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-00009890: 6e64 610a 7065 726c 2d4d 6174 682d 4269  nda.perl-Math-Bi
-000098a0: 6749 6e74 2d46 6173 7443 616c 632e 6161  gInt-FastCalc.aa
-000098b0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098d0: 2020 302e 3530 3039 2d32 2e75 656c 3230    0.5009-2.uel20
-000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098f0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00009900: 6163 6f6e 6461 0a70 6572 6c2d 4d61 7468  aconda.perl-Math
-00009910: 2d42 6967 5261 742e 6e6f 6172 6368 2020  -BigRat.noarch  
-00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009930: 2020 2020 2020 2020 2020 2030 2e32 3631             0.261
-00009940: 342d 322e 7565 6c32 3020 2020 2020 2020  4-2.uel20       
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00009970: 7065 726c 2d4d 6f64 756c 652d 436f 7265  perl-Module-Core
-00009980: 4c69 7374 2e6e 6f61 7263 6820 2020 2020  List.noarch     
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2020 2020 2020 313a 352e 3230 3230          1:5.2020
-000099b0: 3037 3137 2d31 2e75 656c 3230 2020 2020  0717-1.uel20    
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-000099e0: 6461 0a70 6572 6c2d 4d6f 6475 6c65 2d4c  da.perl-Module-L
-000099f0: 6f61 642e 6e6f 6172 6368 2020 2020 2020  oad.noarch      
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 2020 2020 2031 3a30 2e33 342d 312e         1:0.34-1.
-00009a20: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-00009a50: 2d4d 6f64 756c 652d 4c6f 6164 2d43 6f6e  -Module-Load-Con
-00009a60: 6469 7469 6f6e 616c 2e6e 6f61 7263 6820  ditional.noarch 
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 2020 2020 2020 302e 3732              0.72
-00009a90: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00009ac0: 6572 6c2d 4d6f 6475 6c65 2d4d 6574 6164  erl-Module-Metad
-00009ad0: 6174 612e 6e6f 6172 6368 2020 2020 2020  ata.noarch      
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 2020 2031 2e30 3030 3033 372d         1.000037-
-00009b00: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b20: 2020 2020 4061 6e61 636f 6e64 610a 7065      @anaconda.pe
-00009b30: 726c 2d4d 6f7a 696c 6c61 2d43 412e 6e6f  rl-Mozilla-CA.no
-00009b40: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b60: 2031 3a32 3032 3030 3532 302d 312e 7565   1:20200520-1.ue
-00009b70: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 4061 6e61 636f 6e64 610a 7065 726c 2d4e  @anaconda.perl-N
-00009ba0: 6574 2d53 534c 6561 792e 6161 7263 6836  et-SSLeay.aarch6
-00009bb0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-00009bd0: 3838 2d35 2e75 656c 3230 2020 2020 2020  88-5.uel20      
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00009c00: 0a70 6572 6c2d 5061 7261 6d73 2d43 6865  .perl-Params-Che
-00009c10: 636b 2e6e 6f61 7263 6820 2020 2020 2020  ck.noarch       
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 2020 2020 313a 302e 3338 2d34 3138        1:0.38-418
-00009c40: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-00009c70: 6c2d 5061 7468 546f 6f6c 732e 6161 7263  l-PathTools.aarc
-00009c80: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ca0: 332e 3735 2d35 2e75 656c 3230 2020 2020  3.75-5.uel20    
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-00009cd0: 6461 0a70 6572 6c2d 5065 726c 2d4f 5354  da.perl-Perl-OST
-00009ce0: 7970 652e 6e6f 6172 6368 2020 2020 2020  ype.noarch      
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2020 2020 2031 2e30 3130 2d34 3231         1.010-421
-00009d10: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d30: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-00009d40: 6c2d 5065 726c 494f 2d76 6961 2d51 756f  l-PerlIO-via-Quo
-00009d50: 7465 6450 7269 6e74 2e6e 6f61 7263 6820  tedPrint.noarch 
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 2020 2020 2020 2020 2020 2020 302e 3038              0.08
-00009d80: 2d33 3937 2e75 656c 3230 2020 2020 2020  -397.uel20      
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-00009db0: 0a70 6572 6c2d 506f 642d 4368 6563 6b65  .perl-Pod-Checke
-00009dc0: 722e 6e6f 6172 6368 2020 2020 2020 2020  r.noarch        
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2020 2020 2034 3a31 2e37 332d 3339 382e       4:1.73-398.
-00009df0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-00009e20: 2d50 6f64 2d45 7363 6170 6573 2e6e 6f61  -Pod-Escapes.noa
-00009e30: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 313a 312e 3037 2d34 3139 2e75 656c 3230  1:1.07-419.uel20
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-00009e80: 6163 6f6e 6461 0a70 6572 6c2d 506f 642d  aconda.perl-Pod-
-00009e90: 5061 7273 6572 2e6e 6f61 7263 6820 2020  Parser.noarch   
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009eb0: 2020 2020 2020 2020 2020 312e 3633 2d33            1.63-3
-00009ec0: 3937 2e75 656c 3230 2020 2020 2020 2020  97.uel20        
-00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-00009ef0: 6572 6c2d 506f 642d 5065 726c 646f 632e  erl-Pod-Perldoc.
-00009f00: 6e6f 6172 6368 2020 2020 2020 2020 2020  noarch          
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 2020 2031 3a33 2e32 382d 332e 7565 6c32     1:3.28-3.uel2
-00009f30: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-00009f40: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-00009f50: 6e61 636f 6e64 610a 7065 726c 2d50 6f64  naconda.perl-Pod
-00009f60: 2d53 696d 706c 652e 6e6f 6172 6368 2020  -Simple.noarch  
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 2020 2020 2020 2020 2031 3a33 2e34             1:3.4
-00009f90: 302d 312e 7565 6c32 3020 2020 2020 2020  0-1.uel20       
-00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fb0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-00009fc0: 7065 726c 2d50 6f64 2d55 7361 6765 2e6e  perl-Pod-Usage.n
-00009fd0: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ff0: 2020 343a 312e 3730 2d31 2e75 656c 3230    4:1.70-1.uel20
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000a020: 6163 6f6e 6461 0a70 6572 6c2d 5363 616c  aconda.perl-Scal
-0000a030: 6172 2d4c 6973 742d 5574 696c 732e 6161  ar-List-Utils.aa
-0000a040: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 343a 312e 3535 2d31 2e75 656c 3230    4:1.55-1.uel20
-0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a080: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000a090: 6163 6f6e 6461 0a70 6572 6c2d 536f 636b  aconda.perl-Sock
-0000a0a0: 6574 2e61 6172 6368 3634 2020 2020 2020  et.aarch64      
-0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0c0: 2020 2020 2020 2034 3a32 2e30 3330 2d31         4:2.030-1
-0000a0d0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-0000a100: 6c2d 5374 6f72 6162 6c65 2e61 6172 6368  l-Storable.aarch
-0000a110: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-0000a130: 3a33 2e31 352d 322e 7565 6c32 3020 2020  :3.15-2.uel20   
-0000a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a150: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000a160: 6e64 610a 7065 726c 2d53 7973 2d53 7973  nda.perl-Sys-Sys
-0000a170: 6c6f 672e 6161 7263 6836 3420 2020 2020  log.aarch64     
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a190: 2020 2020 2020 2020 302e 3336 2d31 2e75          0.36-1.u
-0000a1a0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2040 616e 6163 6f6e 6461 0a70 6572 6c2d   @anaconda.perl-
-0000a1d0: 5465 726d 2d41 4e53 4943 6f6c 6f72 2e6e  Term-ANSIColor.n
-0000a1e0: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 352e 3031 2d31 2e75 656c 3230 2020    5.01-1.uel20  
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000a230: 6f6e 6461 0a70 6572 6c2d 5465 726d 2d43  onda.perl-Term-C
-0000a240: 6170 2e6e 6f61 7263 6820 2020 2020 2020  ap.noarch       
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 2020 2020 312e 3137 2d35 3130 2e75        1.17-510.u
-0000a270: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2040 616e 6163 6f6e 6461 0a70 6572 6c2d   @anaconda.perl-
-0000a2a0: 5465 7374 2d48 6172 6e65 7373 2e6e 6f61  Test-Harness.noa
-0000a2b0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2d0: 313a 332e 3432 2d31 2e75 656c 3230 2020  1:3.42-1.uel20  
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000a300: 6f6e 6461 0a70 6572 6c2d 5465 7374 2d53  onda.perl-Test-S
-0000a310: 696d 706c 652e 6e6f 6172 6368 2020 2020  imple.noarch    
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2020 2020 2020 2032 3a31 2e33 3032           2:1.302
-0000a340: 3135 362d 312e 7565 6c32 3020 2020 2020  156-1.uel20     
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000a370: 610a 7065 726c 2d54 6578 742d 4261 6c61  a.perl-Text-Bala
-0000a380: 6e63 6564 2e6e 6f61 7263 6820 2020 2020  nced.noarch     
-0000a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3a0: 2020 2020 2020 2020 322e 3033 2d34 3230          2.03-420
-0000a3b0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3d0: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-0000a3e0: 6c2d 5465 7874 2d44 6966 662e 6e6f 6172  l-Text-Diff.noar
-0000a3f0: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-0000a400: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-0000a410: 2e34 352d 372e 7565 6c32 3020 2020 2020  .45-7.uel20     
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000a440: 610a 7065 726c 2d54 6578 742d 5061 7273  a.perl-Text-Pars
-0000a450: 6557 6f72 6473 2e6e 6f61 7263 6820 2020  eWords.noarch   
-0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a470: 2020 2020 2020 2020 2020 332e 3330 2d34            3.30-4
-0000a480: 3139 2e75 656c 3230 2020 2020 2020 2020  19.uel20        
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000a4b0: 6572 6c2d 5465 7874 2d54 6162 732b 5772  erl-Text-Tabs+Wr
-0000a4c0: 6170 2e6e 6f61 7263 6820 2020 2020 2020  ap.noarch       
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4e0: 2020 2020 2020 3230 3133 2e30 3532 332d        2013.0523-
-0000a4f0: 3431 392e 7565 6c32 3020 2020 2020 2020  419.uel20       
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000a520: 7065 726c 2d54 6872 6561 642d 5175 6575  perl-Thread-Queu
-0000a530: 652e 6e6f 6172 6368 2020 2020 2020 2020  e.noarch        
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2033 2e31 332d 332e 7565 6c32       3.13-3.uel2
-0000a560: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000a570: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000a580: 6e61 636f 6e64 610a 7065 726c 2d54 696d  naconda.perl-Tim
-0000a590: 652d 4869 5265 732e 6161 7263 6836 3420  e-HiRes.aarch64 
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2020 2020 2020 2020 2020 2020 313a 312e              1:1.
-0000a5c0: 3937 3634 2d31 2e75 656c 3230 2020 2020  9764-1.uel20    
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-0000a5f0: 6461 0a70 6572 6c2d 5469 6d65 2d4c 6f63  da.perl-Time-Loc
-0000a600: 616c 2e6e 6f61 7263 6820 2020 2020 2020  al.noarch       
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 2020 2020 323a 312e 3330 302d 312e        2:1.300-1.
-0000a630: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-0000a660: 2d55 5249 2e6e 6f61 7263 6820 2020 2020  -URI.noarch     
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 312e 3736 2d33 2e75          1.76-3.u
-0000a690: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2040 616e 6163 6f6e 6461 0a70 6572 6c2d   @anaconda.perl-
-0000a6c0: 556e 6963 6f64 652d 436f 6c6c 6174 652e  Unicode-Collate.
-0000a6d0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6f0: 2020 2020 312e 3237 2d32 2e75 656c 3230      1.27-2.uel20
-0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a710: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000a720: 6163 6f6e 6461 0a70 6572 6c2d 556e 6963  aconda.perl-Unic
-0000a730: 6f64 652d 4e6f 726d 616c 697a 652e 6161  ode-Normalize.aa
-0000a740: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 2020 312e 3236 2d34 3139 2e75 656c 3230    1.26-419.uel20
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a780: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000a790: 6163 6f6e 6461 0a70 6572 6c2d 6175 746f  aconda.perl-auto
-0000a7a0: 6469 652e 6e6f 6172 6368 2020 2020 2020  die.noarch      
-0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7c0: 2020 2020 2020 2032 2e33 322d 312e 7565         2.32-1.ue
-0000a7d0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 4061 6e61 636f 6e64 610a 7065 726c 2d62  @anaconda.perl-b
-0000a800: 6967 6e75 6d2e 6e6f 6172 6368 2020 2020  ignum.noarch    
-0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a820: 2020 2020 2020 2020 2030 2e35 312d 312e           0.51-1.
-0000a830: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a850: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-0000a860: 2d63 6f6e 7374 616e 742e 6e6f 6172 6368  -constant.noarch
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 2020 2020 2020 2020 2020 2020 2031 2e33               1.3
-0000a890: 332d 3432 312e 7565 6c32 3020 2020 2020  3-421.uel20     
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000a8c0: 610a 7065 726c 2d64 6576 656c 2e61 6172  a.perl-devel.aar
-0000a8d0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8f0: 2034 3a35 2e32 382e 332d 362e 7570 312e   4:5.28.3-6.up1.
-0000a900: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 4061 6e61 636f 6e64 610a 7065 726c    @anaconda.perl
-0000a930: 2d65 7870 6572 696d 656e 7461 6c2e 6e6f  -experimental.no
-0000a940: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a960: 2030 2e30 3232 2d31 2e75 656c 3230 2020   0.022-1.uel20  
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000a990: 6f6e 6461 0a70 6572 6c2d 6c69 626e 6574  onda.perl-libnet
-0000a9a0: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 2020 332e 3131 2d34 3230 2e75 656c      3.11-420.uel
-0000a9d0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000a9f0: 616e 6163 6f6e 6461 0a70 6572 6c2d 6c69  anaconda.perl-li
-0000aa00: 6273 2e61 6172 6368 3634 2020 2020 2020  bs.aarch64      
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2020 2020 2020 2034 3a35 2e32 382e 332d         4:5.28.3-
-0000aa30: 362e 7570 312e 7565 6c32 3020 2020 2020  6.up1.uel20     
-0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa50: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000aa60: 610a 7065 726c 2d70 6172 656e 742e 6e6f  a.perl-parent.no
-0000aa70: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 2031 3a30 2e32 3338 2d31 2e75 656c 3230   1:0.238-1.uel20
-0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aab0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000aac0: 6163 6f6e 6461 0a70 6572 6c2d 7065 726c  aconda.perl-perl
-0000aad0: 6661 712e 6e6f 6172 6368 2020 2020 2020  faq.noarch      
-0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaf0: 2020 2020 2020 2035 2e32 3032 3030 3532         5.2020052
-0000ab00: 332d 312e 7565 6c32 3020 2020 2020 2020  3-1.uel20       
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab20: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000ab30: 7065 726c 2d70 6f64 6c61 746f 7273 2e6e  perl-podlators.n
-0000ab40: 6f61 7263 6820 2020 2020 2020 2020 2020  oarch           
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab60: 2020 313a 342e 3134 2d31 2e75 656c 3230    1:4.14-1.uel20
-0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab80: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000ab90: 6163 6f6e 6461 0a70 6572 6c2d 7468 7265  aconda.perl-thre
-0000aba0: 6164 732e 6161 7263 6836 3420 2020 2020  ads.aarch64     
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 2020 2020 323a 322e 3231 2d31          2:2.21-1
-0000abd0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abf0: 2020 2040 616e 6163 6f6e 6461 0a70 6572     @anaconda.per
-0000ac00: 6c2d 7468 7265 6164 732d 7368 6172 6564  l-threads-shared
-0000ac10: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 2020 2031 2e35 392d 332e 7565 6c32       1.59-3.uel2
-0000ac40: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000ac60: 6e61 636f 6e64 610a 7065 726c 2d76 6572  naconda.perl-ver
-0000ac70: 7369 6f6e 2e61 6172 6368 3634 2020 2020  sion.aarch64    
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 2020 2020 2020 2038 3a30 2e39 392e           8:0.99.
-0000aca0: 3237 2d31 2e75 656c 3230 2020 2020 2020  27-1.uel20      
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acc0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000acd0: 0a70 6967 7a2e 6161 7263 6836 3420 2020  .pigz.aarch64   
-0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acf0: 2020 2020 2020 2020 2020 322e 342d 372e            2.4-7.
-0000ad00: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad20: 2020 4061 6e61 636f 6e64 610a 7069 6e65    @anaconda.pine
-0000ad30: 6e74 7279 2e61 6172 6368 3634 2020 2020  ntry.aarch64    
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad50: 2020 2020 2020 2020 2031 2e31 2e30 2d35           1.1.0-5
-0000ad60: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad80: 2020 2040 616e 6163 6f6e 6461 0a70 6978     @anaconda.pix
-0000ad90: 6d61 6e2e 6161 7263 6836 3420 2020 2020  man.aarch64     
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 2020 2020 2020 2020 302e 3430 2e30 2d31          0.40.0-1
-0000adc0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 2020 2040 616e 6163 6f6e 6461 0a70 6b67     @anaconda.pkg
-0000adf0: 636f 6e66 2e61 6172 6368 3634 2020 2020  conf.aarch64    
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 2020 2031 2e37 2e33 2d31           1.7.3-1
-0000ae20: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae40: 2020 2040 616e 6163 6f6e 6461 0a70 6c79     @anaconda.ply
-0000ae50: 6d6f 7574 682e 6161 7263 6836 3420 2020  mouth.aarch64   
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 2020 2020 2020 2020 302e 392e 352d            0.9.5-
-0000ae80: 322e 7570 312e 7565 6c32 3020 2020 2020  2.up1.uel20     
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aea0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000aeb0: 610a 706c 796d 6f75 7468 2d74 6865 6d65  a.plymouth-theme
-0000aec0: 2d63 6861 7267 652e 6161 7263 6836 3420  -charge.aarch64 
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aee0: 2020 2020 2020 2020 2020 2020 302e 392e              0.9.
-0000aef0: 352d 322e 7570 312e 7565 6c32 3020 2020  5-2.up1.uel20   
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000af20: 6e64 610a 706f 6c69 6379 636f 7265 7574  nda.policycoreut
-0000af30: 696c 732e 6161 7263 6836 3420 2020 2020  ils.aarch64     
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 2020 2020 332e 312d 372e 7565          3.1-7.ue
-0000af60: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 4061 6e61 636f 6e64 610a 706f 6c6b 6974  @anaconda.polkit
-0000af90: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2030 2e31 3136 2d38 2e75 7031       0.116-8.up1
-0000afc0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 2040 616e 6163 6f6e 6461 0a70 6f6c     @anaconda.pol
-0000aff0: 6b69 742d 6c69 6273 2e61 6172 6368 3634  kit-libs.aarch64
-0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b010: 2020 2020 2020 2020 2020 2020 2030 2e31               0.1
-0000b020: 3136 2d38 2e75 7031 2e75 656c 3230 2020  16-8.up1.uel20  
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000b050: 6f6e 6461 0a70 6f6c 6b69 742d 706b 6c61  onda.polkit-pkla
-0000b060: 2d63 6f6d 7061 742e 6161 7263 6836 3420  -compat.aarch64 
-0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b080: 2020 2020 2020 2020 2020 2020 302e 312d              0.1-
-0000b090: 3230 2e75 656c 3230 2020 2020 2020 2020  20.uel20        
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000b0c0: 6f70 742e 6161 7263 6836 3420 2020 2020  opt.aarch64     
-0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0e0: 2020 2020 2020 2020 312e 3138 2d31 2e75          1.18-1.u
-0000b0f0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b110: 2040 616e 6163 6f6e 6461 0a70 6f77 6572   @anaconda.power
-0000b120: 746f 702e 6161 7263 6836 3420 2020 2020  top.aarch64     
-0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b140: 2020 2020 2020 2020 322e 392d 3132 2e75          2.9-12.u
-0000b150: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2040 616e 6163 6f6e 6461 0a70 726f 6370   @anaconda.procp
-0000b180: 732d 6e67 2e61 6172 6368 3634 2020 2020  s-ng.aarch64    
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 2020 2020 2020 2020 2033 2e33 2e31 362d           3.3.16-
-0000b1b0: 3137 2e75 656c 3230 2020 2020 2020 2020  17.uel20        
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000b1e0: 726f 6370 732d 6e67 2d68 656c 702e 6e6f  rocps-ng-help.no
-0000b1f0: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b210: 2033 2e33 2e31 362d 3137 2e75 656c 3230   3.3.16-17.uel20
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000b240: 6163 6f6e 6461 0a70 7562 6c69 6373 7566  aconda.publicsuf
-0000b250: 6669 782d 6c69 7374 2e6e 6f61 7263 6820  fix-list.noarch 
-0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 2020 2020 2020 2020 2020 2020 3230 3230              2020
-0000b280: 3037 3138 2d31 2e75 656c 3230 2020 2020  0718-1.uel20    
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-0000b2b0: 6461 0a70 7974 686f 6e2d 7069 702d 7768  da.python-pip-wh
-0000b2c0: 6565 6c2e 6e6f 6172 6368 2020 2020 2020  eel.noarch      
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 2020 2020 2032 302e 322e 322d 312e         20.2.2-1.
-0000b2f0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 4061 6e61 636f 6e64 610a 7079 7468    @anaconda.pyth
-0000b320: 6f6e 2d73 6574 7570 746f 6f6c 732e 6e6f  on-setuptools.no
-0000b330: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b350: 2034 342e 312e 312d 312e 7565 6c32 3020   44.1.1-1.uel20 
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b370: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000b380: 636f 6e64 610a 7079 7468 6f6e 322e 6161  conda.python2.aa
-0000b390: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 322e 372e 3138 2d31 2e75 656c 3230    2.7.18-1.uel20
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000b3e0: 6163 6f6e 6461 0a70 7974 686f 6e32 2d64  aconda.python2-d
-0000b3f0: 6562 7567 2e61 6172 6368 3634 2020 2020  ebug.aarch64    
-0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b410: 2020 2020 2020 2020 2032 2e37 2e31 382d           2.7.18-
-0000b420: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 4061 6e61 636f 6e64 610a 7079      @anaconda.py
-0000b450: 7468 6f6e 322d 6465 7665 6c2e 6161 7263  thon2-devel.aarc
-0000b460: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 322e 372e 3138 2d31 2e75 656c 3230 2020  2.7.18-1.uel20  
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000b4b0: 6f6e 6461 0a70 7974 686f 6e32 2d68 656c  onda.python2-hel
-0000b4c0: 702e 6e6f 6172 6368 2020 2020 2020 2020  p.noarch        
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4e0: 2020 2020 2032 2e37 2e31 382d 312e 7565       2.7.18-1.ue
-0000b4f0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 4061 6e61 636f 6e64 610a 7079 7468 6f6e  @anaconda.python
-0000b520: 322d 7069 702e 6e6f 6172 6368 2020 2020  2-pip.noarch    
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b540: 2020 2020 2020 2020 2032 302e 322e 322d           20.2.2-
-0000b550: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b570: 2020 2020 4061 6e61 636f 6e64 610a 7079      @anaconda.py
-0000b580: 7468 6f6e 322d 7365 7475 7074 6f6f 6c73  thon2-setuptools
-0000b590: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5b0: 2020 2020 3434 2e31 2e31 2d31 2e75 656c      44.1.1-1.uel
-0000b5c0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000b5e0: 616e 6163 6f6e 6461 0a70 7974 686f 6e32  anaconda.python2
-0000b5f0: 2d74 6b69 6e74 6572 2e61 6172 6368 3634  -tkinter.aarch64
-0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b610: 2020 2020 2020 2020 2020 2020 2032 2e37               2.7
-0000b620: 2e31 382d 312e 7565 6c32 3020 2020 2020  .18-1.uel20     
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000b650: 610a 7079 7468 6f6e 322d 746f 6f6c 732e  a.python2-tools.
-0000b660: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 2020 322e 372e 3138 2d31 2e75 656c      2.7.18-1.uel
-0000b690: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000b6b0: 616e 6163 6f6e 6461 0a70 7974 686f 6e33  anaconda.python3
-0000b6c0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 2020 2020 2033 2e37 2e39 2d31 332e 7565       3.7.9-13.ue
-0000b6f0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 4061 6e61 636f 6e64 610a 7079 7468 6f6e  @anaconda.python
-0000b720: 332d 6361 6972 6f2e 6161 7263 6836 3420  3-cairo.aarch64 
-0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b740: 2020 2020 2020 2020 2020 2020 312e 3139              1.19
-0000b750: 2e31 2d31 2e75 656c 3230 2020 2020 2020  .1-1.uel20      
-0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b770: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000b780: 0a70 7974 686f 6e33 2d63 6f6e 6669 676f  .python3-configo
-0000b790: 626a 2e6e 6f61 7263 6820 2020 2020 2020  bj.noarch       
-0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 2020 2020 352e 302e 362d 3135 2e75        5.0.6-15.u
-0000b7c0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2040 616e 6163 6f6e 6461 0a70 7974 686f   @anaconda.pytho
-0000b7f0: 6e33 2d64 6174 6575 7469 6c2e 6e6f 6172  n3-dateutil.noar
-0000b800: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-0000b810: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-0000b820: 3a32 2e38 2e31 2d34 2e75 656c 3230 2020  :2.8.1-4.uel20  
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b840: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000b850: 6f6e 6461 0a70 7974 686f 6e33 2d64 6275  onda.python3-dbu
-0000b860: 732e 6161 7263 6836 3420 2020 2020 2020  s.aarch64       
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 2020 2020 312e 322e 3136 2d31 2e75        1.2.16-1.u
-0000b890: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8b0: 2040 616e 6163 6f6e 6461 0a70 7974 686f   @anaconda.pytho
-0000b8c0: 6e33 2d64 6563 6f72 6174 6f72 2e6e 6f61  n3-decorator.noa
-0000b8d0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8f0: 342e 342e 322d 312e 7565 6c32 3020 2020  4.4.2-1.uel20   
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000b920: 6e64 610a 7079 7468 6f6e 332d 6469 7374  nda.python3-dist
-0000b930: 726f 2e6e 6f61 7263 6820 2020 2020 2020  ro.noarch       
-0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b950: 2020 2020 2020 312e 352e 302d 312e 7565        1.5.0-1.ue
-0000b960: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 4061 6e61 636f 6e64 610a 7079 7468 6f6e  @anaconda.python
-0000b990: 332d 646e 662e 6e6f 6172 6368 2020 2020  3-dnf.noarch    
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2020 2020 2020 2020 2034 2e32 2e32 332d           4.2.23-
-0000b9c0: 342e 7565 6c32 3020 2020 2020 2020 2020  4.uel20         
-0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9e0: 2020 2020 4061 6e61 636f 6e64 610a 7079      @anaconda.py
-0000b9f0: 7468 6f6e 332d 646e 662d 706c 7567 696e  thon3-dnf-plugin
-0000ba00: 732d 636f 7265 2e6e 6f61 7263 6820 2020  s-core.noarch   
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 2020 2020 2020 2020 2020 342e 302e 3137            4.0.17
-0000ba30: 2d32 2e75 7031 2e75 656c 3230 2020 2020  -2.up1.uel20    
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-0000ba60: 6461 0a70 7974 686f 6e33 2d66 6972 6577  da.python3-firew
-0000ba70: 616c 6c2e 6e6f 6172 6368 2020 2020 2020  all.noarch      
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 2020 2020 2020 2030 2e36 2e36 2d34 2e75         0.6.6-4.u
-0000baa0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2040 616e 6163 6f6e 6461 0a70 7974 686f   @anaconda.pytho
-0000bad0: 6e33 2d67 6f62 6a65 6374 2e61 6172 6368  n3-gobject.aarch
-0000bae0: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-0000bb00: 2e33 362e 312d 322e 7565 6c32 3020 2020  .36.1-2.uel20   
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb20: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000bb30: 6e64 610a 7079 7468 6f6e 332d 676f 626a  nda.python3-gobj
-0000bb40: 6563 742d 6261 7365 2e61 6172 6368 3634  ect-base.aarch64
-0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb60: 2020 2020 2020 2020 2020 2020 2033 2e33               3.3
-0000bb70: 362e 312d 322e 7565 6c32 3020 2020 2020  6.1-2.uel20     
-0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000bba0: 610a 7079 7468 6f6e 332d 6770 676d 652e  a.python3-gpgme.
-0000bbb0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 2020 2020 312e 3134 2e30 2d31 2e75 656c      1.14.0-1.uel
-0000bbe0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000bc00: 616e 6163 6f6e 6461 0a70 7974 686f 6e33  anaconda.python3
-0000bc10: 2d68 6177 6b65 792e 6161 7263 6836 3420  -hawkey.aarch64 
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 2020 2020 2020 2020 302e 3438              0.48
-0000bc40: 2e30 2d32 2e75 656c 3230 2020 2020 2020  .0-2.uel20      
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc60: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000bc70: 0a70 7974 686f 6e33 2d68 656c 702e 6e6f  .python3-help.no
-0000bc80: 6172 6368 2020 2020 2020 2020 2020 2020  arch            
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2033 2e37 2e39 2d31 332e 7565 6c32 3020   3.7.9-13.uel20 
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000bcd0: 636f 6e64 610a 7079 7468 6f6e 332d 6c69  conda.python3-li
-0000bce0: 6263 6f6d 7073 2e61 6172 6368 3634 2020  bcomps.aarch64  
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2030 2e31 2e31             0.1.1
-0000bd10: 302d 322e 7565 6c32 3020 2020 2020 2020  0-2.uel20       
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000bd40: 7079 7468 6f6e 332d 6c69 6264 6e66 2e61  python3-libdnf.a
-0000bd50: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2030 2e34 382e 302d 322e 7565 6c32     0.48.0-2.uel2
-0000bd80: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000bd90: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000bda0: 6e61 636f 6e64 610a 7079 7468 6f6e 332d  naconda.python3-
-0000bdb0: 6c69 6e75 782d 7072 6f63 6673 2e6e 6f61  linux-procfs.noa
-0000bdc0: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 302e 362e 322d 332e 7565 6c32 3020 2020  0.6.2-3.uel20   
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000be10: 6e64 610a 7079 7468 6f6e 332d 7065 7266  nda.python3-perf
-0000be20: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2020 2020 2034 2e31 392e 3930 2d32 3130       4.19.90-210
-0000be50: 362e 332e 302e 3030 3935 2e75 7032 2e75  6.3.0.0095.up2.u
-0000be60: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2040 616e 6163 6f6e 6461 0a70 7974 686f   @anaconda.pytho
-0000be90: 6e33 2d70 6970 2e6e 6f61 7263 6820 2020  n3-pip.noarch   
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2020 2020 2020 2020 3230 2e32 2e32            20.2.2
-0000bec0: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000bef0: 7974 686f 6e33 2d70 7970 6172 7369 6e67  ython3-pyparsing
-0000bf00: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 2020 2020 322e 342e 372d 322e 7565 6c32      2.4.7-2.uel2
-0000bf30: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000bf40: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000bf50: 6e61 636f 6e64 610a 7079 7468 6f6e 332d  naconda.python3-
-0000bf60: 7079 7564 6576 2e6e 6f61 7263 6820 2020  pyudev.noarch   
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 2020 2020 2020 2020 2020 302e 3232 2e30            0.22.0
-0000bf90: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000bfc0: 7974 686f 6e33 2d70 7979 616d 6c2e 6161  ython3-pyyaml.aa
-0000bfd0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 352e 332e 312d 332e 7565 6c32 3020    5.3.1-3.uel20 
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000c020: 636f 6e64 610a 7079 7468 6f6e 332d 7270  conda.python3-rp
-0000c030: 6d2e 6161 7263 6836 3420 2020 2020 2020  m.aarch64       
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 342e 3135 2e31 2d32 382e        4.15.1-28.
-0000c060: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 2020 4061 6e61 636f 6e64 610a 7079 7468    @anaconda.pyth
-0000c090: 6f6e 332d 7270 6d2d 6765 6e65 7261 746f  on3-rpm-generato
-0000c0a0: 7273 2e6e 6f61 7263 6820 2020 2020 2020  rs.noarch       
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 392d 312e 7565 6c32 3020        9-1.uel20 
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000c0f0: 636f 6e64 610a 7079 7468 6f6e 332d 7363  conda.python3-sc
-0000c100: 6865 6475 7469 6c73 2e61 6172 6368 3634  hedutils.aarch64
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 2020 2020 2020 2020 2020 2020 2030 2e36               0.6
-0000c130: 2d36 2e75 656c 3230 2020 2020 2020 2020  -6.uel20        
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2040 616e 6163 6f6e 6461 0a70       @anaconda.p
-0000c160: 7974 686f 6e33 2d73 6574 7570 746f 6f6c  ython3-setuptool
-0000c170: 732e 6e6f 6172 6368 2020 2020 2020 2020  s.noarch        
-0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c190: 2020 2020 2034 342e 312e 312d 312e 7565       44.1.1-1.ue
-0000c1a0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 4061 6e61 636f 6e64 610a 7079 7468 6f6e  @anaconda.python
-0000c1d0: 332d 7369 782e 6e6f 6172 6368 2020 2020  3-six.noarch    
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 2020 2020 2020 2020 2031 2e31 352e 302d           1.15.0-
-0000c200: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 4061 6e61 636f 6e64 610a 7079      @anaconda.py
-0000c230: 7468 6f6e 332d 736c 6970 2e6e 6f61 7263  thon3-slip.noarc
-0000c240: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-0000c250: 2020 2020 2020 2020 2020 2020 2020 302e                0.
-0000c260: 362e 352d 342e 7565 6c32 3020 2020 2020  6.5-4.uel20     
-0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c280: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000c290: 610a 7079 7468 6f6e 332d 756e 626f 756e  a.python3-unboun
-0000c2a0: 642e 6161 7263 6836 3420 2020 2020 2020  d.aarch64       
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 312e 3131 2e30 2d32 2e75        1.11.0-2.u
-0000c2d0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2f0: 2040 616e 6163 6f6e 6461 0a71 7265 6e63   @anaconda.qrenc
-0000c300: 6f64 652e 6161 7263 6836 3420 2020 2020  ode.aarch64     
-0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c320: 2020 2020 2020 2020 342e 302e 322d 322e          4.0.2-2.
-0000c330: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 2020 4061 6e61 636f 6e64 610a 7174 2d73    @anaconda.qt-s
-0000c360: 6574 7469 6e67 732e 6e6f 6172 6368 2020  ettings.noarch  
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2020 2020 2020 2020 2020 2032 392e 312d             29.1-
-0000c390: 332e 7565 6c32 3020 2020 2020 2020 2020  3.uel20         
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 4061 6e61 636f 6e64 610a 7174      @anaconda.qt
-0000c3c0: 352d 7174 6261 7365 2e61 6172 6368 3634  5-qtbase.aarch64
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3e0: 2020 2020 2020 2020 2020 2020 2035 2e31               5.1
-0000c3f0: 312e 312d 3132 2e75 7032 2e75 656c 3230  1.1-12.up2.uel20
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000c420: 6163 6f6e 6461 0a71 7435 2d71 7462 6173  aconda.qt5-qtbas
-0000c430: 652d 636f 6d6d 6f6e 2e6e 6f61 7263 6820  e-common.noarch 
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2020 2020 2020 2020 352e 3131              5.11
-0000c460: 2e31 2d31 322e 7570 322e 7565 6c32 3020  .1-12.up2.uel20 
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000c490: 636f 6e64 610a 7174 352d 7372 706d 2d6d  conda.qt5-srpm-m
-0000c4a0: 6163 726f 732e 6e6f 6172 6368 2020 2020  acros.noarch    
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2035 2e31 342e 322d           5.14.2-
-0000c4d0: 312e 7565 6c32 3020 2020 2020 2020 2020  1.uel20         
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4f0: 2020 2020 4061 6e61 636f 6e64 610a 7265      @anaconda.re
-0000c500: 6164 6c69 6e65 2e61 6172 6368 3634 2020  adline.aarch64  
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 2020 2020 2020 2020 2038 2e30 2d33             8.0-3
-0000c530: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2040 616e 6163 6f6e 6461 0a72 6573     @anaconda.res
-0000c560: 742e 6161 7263 6836 3420 2020 2020 2020  t.aarch64       
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 2020 302e 382e 312d 372e 7565        0.8.1-7.ue
-0000c590: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 4061 6e61 636f 6e64 610a 726e 672d 746f  @anaconda.rng-to
-0000c5c0: 6f6c 732e 6161 7263 6836 3420 2020 2020  ols.aarch64     
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2020 2020 362e 352d 332e 7565          6.5-3.ue
-0000c5f0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c610: 4061 6e61 636f 6e64 610a 726f 6f74 6669  @anaconda.rootfi
-0000c620: 6c65 732e 6e6f 6172 6368 2020 2020 2020  les.noarch      
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 2038 2e31 2d32 352e 7565         8.1-25.ue
-0000c650: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 4061 6e61 636f 6e64 610a 7270 6d2e 6161  @anaconda.rpm.aa
-0000c680: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2020 342e 3135 2e31 2d32 382e 7565 6c32    4.15.1-28.uel2
-0000c6b0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000c6c0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000c6d0: 6e61 636f 6e64 610a 7270 6d2d 6c69 6273  naconda.rpm-libs
-0000c6e0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c700: 2020 2020 2034 2e31 352e 312d 3238 2e75       4.15.1-28.u
-0000c710: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2040 616e 6163 6f6e 6461 0a72 7379 736c   @anaconda.rsysl
-0000c740: 6f67 2e61 6172 6368 3634 2020 2020 2020  og.aarch64      
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 2020 2038 2e32 3030 362e 302d         8.2006.0-
-0000c770: 362e 7565 6c32 3020 2020 2020 2020 2020  6.uel20         
-0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c790: 2020 2020 4061 6e61 636f 6e64 610a 7273      @anaconda.rs
-0000c7a0: 7973 6c6f 672d 6865 6c70 2e6e 6f61 7263  yslog-help.noarc
-0000c7b0: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-0000c7c0: 2020 2020 2020 2020 2020 2020 2020 382e                8.
-0000c7d0: 3230 3036 2e30 2d36 2e75 656c 3230 2020  2006.0-6.uel20  
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7f0: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000c800: 6f6e 6461 0a73 6563 7572 6974 792d 746f  onda.security-to
-0000c810: 6f6c 2e61 6172 6368 3634 2020 2020 2020  ol.aarch64      
-0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c830: 2020 2020 2020 2032 2e30 2d31 2e37 352e         2.0-1.75.
-0000c840: 7570 312e 7565 6c32 3020 2020 2020 2020  up1.uel20       
-0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000c870: 7365 642e 6161 7263 6836 3420 2020 2020  sed.aarch64     
-0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c890: 2020 2020 2020 2020 342e 382d 332e 7565          4.8-3.ue
-0000c8a0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 4061 6e61 636f 6e64 610a 7365 6c69 6e75  @anaconda.selinu
-0000c8d0: 782d 706f 6c69 6379 2e6e 6f61 7263 6820  x-policy.noarch 
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 2020 2020 2020 2020 2020 2020 332e 3134              3.14
-0000c900: 2e32 2d37 352e 7565 6c32 3020 2020 2020  .2-75.uel20     
-0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c920: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000c930: 610a 7365 6c69 6e75 782d 706f 6c69 6379  a.selinux-policy
-0000c940: 2d74 6172 6765 7465 642e 6e6f 6172 6368  -targeted.noarch
-0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c960: 2020 2020 2020 2020 2020 2020 2033 2e31               3.1
-0000c970: 342e 322d 3735 2e75 656c 3230 2020 2020  4.2-75.uel20    
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-0000c9a0: 6461 0a73 6574 7570 2e6e 6f61 7263 6820  da.setup.noarch 
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9c0: 2020 2020 2020 2020 2020 2020 322e 3133              2.13
-0000c9d0: 2e37 2d32 2e75 656c 3230 2020 2020 2020  .7-2.uel20      
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000ca00: 0a73 6733 5f75 7469 6c73 2e61 6172 6368  .sg3_utils.aarch
-0000ca10: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-0000ca30: 2e34 352d 322e 7565 6c32 3020 2020 2020  .45-2.uel20     
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000ca60: 610a 7368 6164 6f77 2e61 6172 6368 3634  a.shadow.aarch64
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2020 2020 2020 2020 2032 3a34               2:4
-0000ca90: 2e38 2e31 2d33 2e75 656c 3230 2020 2020  .8.1-3.uel20    
-0000caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cab0: 2020 2020 2020 2020 2040 616e 6163 6f6e           @anacon
-0000cac0: 6461 0a73 6861 7265 642d 6d69 6d65 2d69  da.shared-mime-i
-0000cad0: 6e66 6f2e 6161 7263 6836 3420 2020 2020  nfo.aarch64     
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2020 2020 2020 312e 3130 2d34 2e75          1.10-4.u
-0000cb00: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb20: 2040 616e 6163 6f6e 6461 0a73 6869 6d2e   @anaconda.shim.
-0000cb30: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb50: 2020 2020 3135 2d32 312e 7570 322e 7565      15-21.up2.ue
-0000cb60: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 4061 6e61 636f 6e64 610a 736c 616e 672e  @anaconda.slang.
-0000cb90: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbb0: 2020 2020 322e 332e 322d 382e 7565 6c32      2.3.2-8.uel2
-0000cbc0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000cbd0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000cbe0: 6e61 636f 6e64 610a 736e 6170 7079 2e61  naconda.snappy.a
-0000cbf0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc10: 2020 2031 2e31 2e38 2d31 2e75 656c 3230     1.1.8-1.uel20
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc30: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000cc40: 6163 6f6e 6461 0a73 716c 6974 652e 6161  aconda.sqlite.aa
-0000cc50: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc70: 2020 332e 3332 2e33 2d32 2e75 656c 3230    3.32.3-2.uel20
-0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000cca0: 6163 6f6e 6461 0a73 7175 6173 6866 732d  aconda.squashfs-
-0000ccb0: 746f 6f6c 732e 6161 7263 6836 3420 2020  tools.aarch64   
-0000ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccd0: 2020 2020 2020 2020 2020 342e 342d 312e            4.4-1.
-0000cce0: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 4061 6e61 636f 6e64 610a 7375 646f    @anaconda.sudo
-0000cd10: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd30: 2020 2020 2031 2e39 2e32 2d33 2e75 656c       1.9.2-3.uel
-0000cd40: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000cd60: 616e 6163 6f6e 6461 0a73 7973 6673 7574  anaconda.sysfsut
-0000cd70: 696c 732e 6161 7263 6836 3420 2020 2020  ils.aarch64     
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 2020 2020 2020 322e 312e 302d 3238          2.1.0-28
-0000cda0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdc0: 2020 2040 616e 6163 6f6e 6461 0a73 7973     @anaconda.sys
-0000cdd0: 7465 6d64 2e61 6172 6368 3634 2020 2020  temd.aarch64    
-0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdf0: 2020 2020 2020 2020 2032 3433 2d33 382e           243-38.
-0000ce00: 7570 362e 7565 6c32 3020 2020 2020 2020  up6.uel20       
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce20: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000ce30: 7379 7374 656d 642d 6865 6c70 2e6e 6f61  systemd-help.noa
-0000ce40: 7263 6820 2020 2020 2020 2020 2020 2020  rch             
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 3234 332d 3338 2e75 7036 2e75 656c 3230  243-38.up6.uel20
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000ce90: 6163 6f6e 6461 0a73 7973 7465 6d64 2d6c  aconda.systemd-l
-0000cea0: 6962 732e 6161 7263 6836 3420 2020 2020  ibs.aarch64     
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 2020 2020 3234 332d 3338 2e75          243-38.u
-0000ced0: 7036 2e75 656c 3230 2020 2020 2020 2020  p6.uel20        
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cef0: 2020 2020 2040 616e 6163 6f6e 6461 0a73       @anaconda.s
-0000cf00: 7973 7465 6d64 2d75 6465 762e 6161 7263  ystemd-udev.aarc
-0000cf10: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 3234 332d 3338 2e75 7036 2e75 656c 3230  243-38.up6.uel20
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf50: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000cf60: 6163 6f6e 6461 0a73 7973 7465 6d74 6170  aconda.systemtap
-0000cf70: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 2020 2020 2034 2e33 2d32 2e75 656c 3230       4.3-2.uel20
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000cfc0: 6163 6f6e 6461 0a73 7973 7465 6d74 6170  aconda.systemtap
-0000cfd0: 2d63 6c69 656e 742e 6161 7263 6836 3420  -client.aarch64 
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 2020 2020 2020 2020 2020 2020 342e 332d              4.3-
-0000d000: 322e 7565 6c32 3020 2020 2020 2020 2020  2.uel20         
-0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d020: 2020 2020 4061 6e61 636f 6e64 610a 7379      @anaconda.sy
-0000d030: 7374 656d 7461 702d 6465 7665 6c2e 6161  stemtap-devel.aa
-0000d040: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 342e 332d 322e 7565 6c32 3020 2020    4.3-2.uel20   
-0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d080: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000d090: 6e64 610a 7379 7374 656d 7461 702d 6865  nda.systemtap-he
-0000d0a0: 6c70 2e61 6172 6368 3634 2020 2020 2020  lp.aarch64      
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 2034 2e33 2d32 2e75 656c         4.3-2.uel
-0000d0d0: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000d0f0: 616e 6163 6f6e 6461 0a73 7973 7465 6d74  anaconda.systemt
-0000d100: 6170 2d72 756e 7469 6d65 2e61 6172 6368  ap-runtime.aarch
-0000d110: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2034                 4
-0000d130: 2e33 2d32 2e75 656c 3230 2020 2020 2020  .3-2.uel20      
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000d160: 0a73 7973 7465 6d74 6170 2d73 6474 2d64  .systemtap-sdt-d
-0000d170: 6576 656c 2e61 6172 6368 3634 2020 2020  evel.aarch64    
-0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 2020 2020 2020 2020 2034 2e33 2d32 2e75           4.3-2.u
-0000d1a0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1c0: 2040 616e 6163 6f6e 6461 0a74 6172 2e61   @anaconda.tar.a
-0000d1d0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1f0: 2020 2032 3a31 2e33 322d 322e 7565 6c32     2:1.32-2.uel2
-0000d200: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000d210: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000d220: 6e61 636f 6e64 610a 7463 6c2e 6161 7263  naconda.tcl.aarc
-0000d230: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d250: 313a 382e 362e 3130 2d33 2e75 656c 3230  1:8.6.10-3.uel20
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000d280: 6163 6f6e 6461 0a74 6869 6e2d 7072 6f76  aconda.thin-prov
-0000d290: 6973 696f 6e69 6e67 2d74 6f6f 6c73 2e61  isioning-tools.a
-0000d2a0: 6172 6368 3634 2020 2020 2020 2020 2020  arch64          
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2c0: 2020 2030 2e39 2e30 2d32 2e75 656c 3230     0.9.0-2.uel20
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2e0: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000d2f0: 6163 6f6e 6461 0a74 6869 6e2d 7072 6f76  aconda.thin-prov
-0000d300: 6973 696f 6e69 6e67 2d74 6f6f 6c73 2d68  isioning-tools-h
-0000d310: 656c 702e 6e6f 6172 6368 2020 2020 2020  elp.noarch      
-0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d330: 2020 2020 2020 2030 2e39 2e30 2d32 2e75         0.9.0-2.u
-0000d340: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2040 616e 6163 6f6e 6461 0a74 696d 6564   @anaconda.timed
-0000d370: 6174 6578 2e61 6172 6368 3634 2020 2020  atex.aarch64    
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 2020 2030 2e36 2d32 2e75           0.6-2.u
-0000d3a0: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3c0: 2040 616e 6163 6f6e 6461 0a74 6b2e 6161   @anaconda.tk.aa
-0000d3d0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3f0: 2020 313a 382e 362e 3130 2d32 2e75 656c    1:8.6.10-2.uel
-0000d400: 3230 2020 2020 2020 2020 2020 2020 2020  20              
-0000d410: 2020 2020 2020 2020 2020 2020 2020 2040                 @
-0000d420: 616e 6163 6f6e 6461 0a74 726f 7573 6572  anaconda.trouser
-0000d430: 732e 6161 7263 6836 3420 2020 2020 2020  s.aarch64       
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 2020 302e 332e 3134 2d34 2e75        0.3.14-4.u
-0000d460: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2040 616e 6163 6f6e 6461 0a74 756e 6564   @anaconda.tuned
-0000d490: 2e6e 6f61 7263 6820 2020 2020 2020 2020  .noarch         
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2020 2020 322e 3130 2e30 2d39 2e75 7031      2.10.0-9.up1
-0000d4c0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2020 2040 616e 6163 6f6e 6461 0a74 756e     @anaconda.tun
-0000d4f0: 6564 2d68 656c 702e 6e6f 6172 6368 2020  ed-help.noarch  
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2020 2020 2032 2e31 302e             2.10.
-0000d520: 302d 392e 7570 312e 7565 6c32 3020 2020  0-9.up1.uel20   
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000d550: 6e64 610a 747a 6461 7461 2e6e 6f61 7263  nda.tzdata.noarc
-0000d560: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-0000d570: 2020 2020 2020 2020 2020 2020 2020 3230                20
-0000d580: 3231 612d 312e 7570 312e 7565 6c32 3020  21a-1.up1.uel20 
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000d5b0: 636f 6e64 610a 7564 6973 6b73 322e 6161  conda.udisks2.aa
-0000d5c0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5e0: 2020 322e 392e 302d 322e 7570 322e 7565    2.9.0-2.up2.ue
-0000d5f0: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 4061 6e61 636f 6e64 610a 756e 626f 756e  @anaconda.unboun
-0000d620: 642d 6c69 6273 2e61 6172 6368 3634 2020  d-libs.aarch64  
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 2020 2020 2020 2020 2031 2e31 312e             1.11.
-0000d650: 302d 322e 7565 6c32 3020 2020 2020 2020  0-2.uel20       
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000d680: 756e 7a69 702e 6161 7263 6836 3420 2020  unzip.aarch64   
-0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6a0: 2020 2020 2020 2020 2020 362e 302d 3435            6.0-45
-0000d6b0: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2040 616e 6163 6f6e 6461 0a75 6f73     @anaconda.uos
-0000d6e0: 2d6c 6963 656e 7365 2d6d 696e 692e 6161  -license-mini.aa
-0000d6f0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d710: 2020 352e 342e 342e 382d 312e 7565 6c32    5.4.4.8-1.uel2
-0000d720: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000d730: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000d740: 6e61 636f 6e64 610a 7573 6572 7370 6163  naconda.userspac
-0000d750: 652d 7263 752e 6161 7263 6836 3420 2020  e-rcu.aarch64   
-0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d770: 2020 2020 2020 2020 2020 302e 3132 2e31            0.12.1
-0000d780: 2d31 2e75 656c 3230 2020 2020 2020 2020  -1.uel20        
-0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7a0: 2020 2020 2040 616e 6163 6f6e 6461 0a75       @anaconda.u
-0000d7b0: 7469 6c2d 6c69 6e75 782e 6161 7263 6836  til-linux.aarch6
-0000d7c0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-0000d7e0: 3335 2e32 2d36 2e75 7031 2e75 656c 3230  35.2-6.up1.uel20
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d800: 2020 2020 2020 2020 2020 2020 2040 616e               @an
-0000d810: 6163 6f6e 6461 0a76 646f 2e61 6172 6368  aconda.vdo.aarch
-0000d820: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2036                 6
-0000d840: 2e32 2e30 2e32 3938 2d31 322e 7570 312e  .2.0.298-12.up1.
-0000d850: 7565 6c32 3020 2020 2020 2020 2020 2020  uel20           
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2020 4061 6e61 636f 6e64 610a 7669 6d2d    @anaconda.vim-
-0000d880: 6d69 6e69 6d61 6c2e 6161 7263 6836 3420  minimal.aarch64 
-0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8a0: 2020 2020 2020 2020 2020 2020 323a 382e              2:8.
-0000d8b0: 322d 312e 7565 6c32 3020 2020 2020 2020  2-1.uel20       
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8d0: 2020 2020 2020 4061 6e61 636f 6e64 610a        @anaconda.
-0000d8e0: 7669 7274 2d77 6861 742e 6161 7263 6836  virt-what.aarch6
-0000d8f0: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-0000d900: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-0000d910: 3230 2d31 2e75 656c 3230 2020 2020 2020  20-1.uel20      
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d930: 2020 2020 2020 2040 616e 6163 6f6e 6461         @anaconda
-0000d940: 0a76 6f6c 756d 655f 6b65 792e 6161 7263  .volume_key.aarc
-0000d950: 6836 3420 2020 2020 2020 2020 2020 2020  h64             
-0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d970: 302e 332e 3132 2d34 2e75 656c 3230 2020  0.3.12-4.uel20  
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 2020 2020 2020 2020 2020 2040 616e 6163             @anac
-0000d9a0: 6f6e 6461 0a77 6179 6c61 6e64 2e61 6172  onda.wayland.aar
-0000d9b0: 6368 3634 2020 2020 2020 2020 2020 2020  ch64            
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9d0: 2031 2e31 372e 302d 322e 7565 6c32 3020   1.17.0-2.uel20 
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000da00: 636f 6e64 610a 7767 6574 2e61 6172 6368  conda.wget.aarch
-0000da10: 3634 2020 2020 2020 2020 2020 2020 2020  64              
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2031                 1
-0000da30: 2e32 302e 332d 332e 7565 6c32 3020 2020  .20.3-3.uel20   
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000da60: 6e64 610a 7768 6963 682e 6161 7263 6836  nda.which.aarch6
-0000da70: 3420 2020 2020 2020 2020 2020 2020 2020  4               
-0000da80: 2020 2020 2020 2020 2020 2020 2020 322e                2.
-0000da90: 3231 2d31 342e 7565 6c32 3020 2020 2020  21-14.uel20     
-0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dab0: 2020 2020 2020 2020 4061 6e61 636f 6e64          @anacond
-0000dac0: 610a 7770 615f 7375 7070 6c69 6361 6e74  a.wpa_supplicant
-0000dad0: 2e61 6172 6368 3634 2020 2020 2020 2020  .aarch64        
-0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daf0: 2020 2020 2031 3a32 2e36 2d32 382e 7565       1:2.6-28.ue
-0000db00: 6c32 3020 2020 2020 2020 2020 2020 2020  l20             
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db20: 4061 6e61 636f 6e64 610a 7866 7370 726f  @anaconda.xfspro
-0000db30: 6773 2e61 6172 6368 3634 2020 2020 2020  gs.aarch64      
-0000db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db50: 2020 2020 2020 2035 2e36 2e30 2d32 2e75         5.6.0-2.u
-0000db60: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db80: 2040 616e 6163 6f6e 6461 0a78 6673 7072   @anaconda.xfspr
-0000db90: 6f67 732d 7866 735f 7363 7275 622e 6161  ogs-xfs_scrub.aa
-0000dba0: 7263 6836 3420 2020 2020 2020 2020 2020  rch64           
-0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbc0: 2020 352e 362e 302d 322e 7565 6c32 3020    5.6.0-2.uel20 
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2020 2020 2020 2020 2020 2020 4061 6e61              @ana
-0000dbf0: 636f 6e64 610a 786b 6579 626f 6172 642d  conda.xkeyboard-
-0000dc00: 636f 6e66 6967 2e6e 6f61 7263 6820 2020  config.noarch   
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2020 2020 2020 2020 322e 3330 2d31            2.30-1
-0000dc30: 2e75 656c 3230 2020 2020 2020 2020 2020  .uel20          
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc50: 2020 2040 616e 6163 6f6e 6461 0a78 7a2e     @anaconda.xz.
-0000dc60: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 2020 2020 352e 322e 352d 312e 7565 6c32      5.2.5-1.uel2
-0000dc90: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000dcb0: 6e61 636f 6e64 610a 787a 2d6c 6962 732e  naconda.xz-libs.
-0000dcc0: 6161 7263 6836 3420 2020 2020 2020 2020  aarch64         
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dce0: 2020 2020 352e 322e 352d 312e 7565 6c32      5.2.5-1.uel2
-0000dcf0: 3020 2020 2020 2020 2020 2020 2020 2020  0               
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 4061                @a
-0000dd10: 6e61 636f 6e64 610a 7975 6d2e 6e6f 6172  naconda.yum.noar
-0000dd20: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2034                 4
-0000dd40: 2e32 2e32 332d 342e 7565 6c32 3020 2020  .2.23-4.uel20   
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 2020 2020 2020 2020 4061 6e61 636f            @anaco
-0000dd70: 6e64 610a 7a69 702e 6161 7263 6836 3420  nda.zip.aarch64 
-0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2020 2020 2020 332e 302d              3.0-
-0000dda0: 3236 2e75 656c 3230 2020 2020 2020 2020  26.uel20        
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 2020 2020 2040 616e 6163 6f6e 6461 0a7a       @anaconda.z
-0000ddd0: 6c69 622e 6161 7263 6836 3420 2020 2020  lib.aarch64     
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 2020 2020 2020 2020 312e 322e 3131 2d31          1.2.11-1
-0000de00: 372e 7565 6c32 3020 2020 2020 2020 2020  7.uel20         
-0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de20: 2020 2020 4061 6e61 636f 6e64 610a 7a73      @anaconda.zs
-0000de30: 7464 2e61 6172 6368 3634 2020 2020 2020  td.aarch64      
-0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2020 2020 2020 2031 2e34 2e35 2d31 2e75         1.4.5-1.u
-0000de60: 656c 3230 2020 2020 2020 2020 2020 2020  el20            
-0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de80: 2040 616e 6163 6f6e 6461                  @anaconda
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json

### Pretty-printed

```diff
@@ -1,154 +1 @@
-[
-    {
-        "autodependency": "true",
-        "name": "tar"
-    },
-    {
-        "autodependency": "true",
-        "name": "gcc"
-    },
-    {
-        "autodependency": "true",
-        "name": "gcc-c++"
-    },
-    {
-        "autodependency": "true",
-        "name": "make"
-    },
-    {
-        "autodependency": "true",
-        "name": "cmake"
-    },
-    {
-        "autodependency": "true",
-        "name": "unzip"
-    },
-    {
-        "autodependency": "true",
-        "info": "need upgrade to match the new openssl form repo",
-        "name": "gnutls"
-    },
-    {
-        "autodependency": "true",
-        "info": "need upgrade to match the new openssl form repo",
-        "name": "openssh"
-    },
-    {
-        "autodependency": "true",
-        "name": "pciutils"
-    },
-    {
-        "autodependency": "true",
-        "name": "net-tools"
-    },
-    {
-        "autodependency": "true",
-        "info": "python cffi",
-        "name": "libffi-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python zlib",
-        "name": "zlib-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python lzma",
-        "name": "xz-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python bz2",
-        "name": "bzip2-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python sqlite",
-        "name": "sqlite-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python ssl",
-        "name": "openssl-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "python ssl",
-        "name": "openssl"
-    },
-    {
-        "autodependency": "true",
-        "info": "python ssl",
-        "name": "python3-libselinux"
-    },
-    {
-        "autodependency": "true",
-        "info": "tensorflow use",
-        "name": "hdf5"
-    },
-    {
-        "autodependency": "true",
-        "info": "tensorflow use",
-        "name": "hdf5-devel"
-    },
-    {
-        "autodependency": "true",
-        "info": "hdf5 need",
-        "name": "libaec"
-    },
-    {
-        "autodependency": "true",
-        "info": "used for edge ha",
-        "name": "expect"
-    },
-    {
-        "autodependency": "true",
-        "info": "docker need",
-        "name": "fuse-overlayfs"
-    },
-    {
-        "autodependency": "true",
-        "info": "docker need",
-        "name": "container-selinux"
-    },
-    {
-        "autodependency": "true",
-        "info": "docker need",
-        "name": "libcgroup"
-    },
-    {
-        "name": "sshpass",
-        "sha256": "9656bf3703739b0b29b68e0574781118e2327a8e2ee11319fd214c74b9d3c336",
-        "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/aarch64/Packages/s/sshpass-1.06-9.el8.aarch64.rpm"
-    },
-    {
-        "name": "inotify-tools",
-        "sha256": "eb4df7f1af81cde3f559800543a052e98f61fec87500742612c689c0329355c6",
-        "url": "https://mirrors.huaweicloud.com/epel/8/Everything/aarch64/Packages/i/inotify-tools-3.14-19.el8.aarch64.rpm"
-    },
-    {
-        "name": "slirp4netns",
-        "sha256": "c3d964fa9cb020cee2efdce3688ef075734b14bf1dd6fde036117d1914d23c3a",
-        "url": "https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/Packages/slirp4netns-0.4.3-4.el7_8.aarch64.rpm"
-    },
-    {
-        "name": "docker-ce-cli",
-        "release": "3.el8",
-        "version": "20.10.8"
-    },
-    {
-        "name": "containerd.io",
-        "release": "3.1.el8",
-        "version": "1.4.9"
-    },
-    {
-        "name": "docker-ce",
-        "release": "3.el8",
-        "version": "20.10.8"
-    },
-    {
-        "name": "docker-ce-rootless-extras",
-        "release": "3.el8",
-        "version": "20.10.8"
-    }
-]
+[]
```

## ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo

```diff
@@ -1,17 +0,0 @@
-00000000: 5b62 6173 655d 0a62 6173 6575 726c 203d  [base].baseurl =
-00000010: 2068 7474 7073 3a2f 2f72 6570 6f2e 6875   https://repo.hu
-00000020: 6177 6569 636c 6f75 642e 636f 6d2f 6f70  aweicloud.com/op
-00000030: 656e 6575 6c65 722f 6f70 656e 4575 6c65  eneuler/openEule
-00000040: 722d 3230 2e30 332d 4c54 532d 5350 322f  r-20.03-LTS-SP2/
-00000050: 4f53 2f61 6172 6368 3634 2f0a 0a5b 6578  OS/aarch64/..[ex
-00000060: 7472 615d 0a62 6173 6575 726c 3d68 7474  tra].baseurl=htt
-00000070: 7073 3a2f 2f6d 6972 726f 7273 2e68 7561  ps://mirrors.hua
-00000080: 7765 6963 6c6f 7564 2e63 6f6d 2f63 656e  weicloud.com/cen
-00000090: 746f 732d 616c 7461 7263 682f 372f 6578  tos-altarch/7/ex
-000000a0: 7472 6173 2f61 6172 6368 3634 2f0a 0a5b  tras/aarch64/..[
-000000b0: 646f 636b 6572 2d63 655d 0a62 6173 6575  docker-ce].baseu
-000000c0: 726c 3d68 7474 7073 3a2f 2f6d 6972 726f  rl=https://mirro
-000000d0: 7273 2e68 7561 7765 6963 6c6f 7564 2e63  rs.huaweicloud.c
-000000e0: 6f6d 2f64 6f63 6b65 722d 6365 2f6c 696e  om/docker-ce/lin
-000000f0: 7578 2f63 656e 746f 732f 382f 6161 7263  ux/centos/8/aarc
-00000100: 6836 342f 7374 6162 6c65 2f0a            h64/stable/.
```

## ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {'109': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '3': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '81': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '82': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '83': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '84': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '89': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '92': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '96': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * 'delete': '[24, 23, 22, 21, 20]',*

 * * 'insert': "[(125, OrderedDict([('name', 'bzip2')])), (126, Ord […]*

```diff
@@ -5,15 +5,16 @@
     {
         "name": "cpp"
     },
     {
         "name": "g++"
     },
     {
-        "name": "libgcc1"
+        "name": "libgcc1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "gcc-7-base"
     },
     {
         "name": "libasan4"
     },
@@ -56,29 +57,14 @@
     {
         "name": "libcurl4"
     },
     {
         "name": "haveged"
     },
     {
-        "name": "libhavege1"
-    },
-    {
-        "name": "libtinfo5"
-    },
-    {
-        "name": "libtinfo-dev"
-    },
-    {
-        "name": "libncurses5-dev"
-    },
-    {
-        "name": "libncurses5"
-    },
-    {
         "name": "libldap-2.4-2"
     },
     {
         "name": "libgssapi3-heimdal"
     },
     {
         "name": "libasn1-8-heimdal"
@@ -254,60 +240,67 @@
     {
         "name": "libperl5.26"
     },
     {
         "name": "libgdbm-compat4"
     },
     {
-        "name": "libgomp1"
+        "name": "libgomp1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "libitm1"
+        "name": "libitm1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "libatomic1"
+        "name": "libatomic1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "liblsan0"
+        "name": "liblsan0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "libisl19"
     },
     {
         "name": "libmpc3"
     },
     {
         "name": "libmpfr6"
     },
     {
         "name": "binutils"
     },
     {
-        "name": "libtsan0"
+        "name": "libtsan0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "linux-libc-dev"
     },
     {
         "name": "libc-dev-bin"
     },
     {
-        "name": "libcc1-0"
+        "name": "libcc1-0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "binutils-aarch64-linux-gnu"
     },
     {
         "name": "libbinutils"
     },
     {
         "name": "binutils-common"
     },
     {
-        "name": "gcc-8-base"
+        "name": "gcc-8-base",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "libselinux1"
     },
     {
         "name": "libselinux1-dev"
     },
@@ -338,15 +331,16 @@
     {
         "name": "libbz2-1.0"
     },
     {
         "name": "liblzma-dev"
     },
     {
-        "name": "libstdc++6"
+        "name": "libstdc++6",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "docker-ce",
         "version": "20.10.21"
     },
     {
         "name": "docker-ce-rootless-extras",
@@ -390,15 +384,144 @@
     {
         "name": "iptables"
     },
     {
         "name": "gzip"
     },
     {
+        "name": "bzip2"
+    },
+    {
+        "name": "libhavege1"
+    },
+    {
+        "name": "libip4tc0"
+    },
+    {
+        "name": "libip6tc0"
+    },
+    {
+        "name": "libiptc0"
+    },
+    {
+        "name": "libxtables12"
+    },
+    {
+        "name": "liblzma5"
+    },
+    {
+        "name": "libpcre3"
+    },
+    {
+        "name": "libsepol1"
+    },
+    {
+        "name": "dbus-user-session"
+    },
+    {
+        "name": "libdbus-1-3"
+    },
+    {
+        "name": "dbus"
+    },
+    {
         "info": "used by mindspore",
         "name": "libgmpxx4ldbl"
     },
     {
         "info": "used by new version docker",
         "name": "libseccomp2"
+    },
+    {
+        "name": "python3-distutils"
+    },
+    {
+        "name": "python3"
+    },
+    {
+        "name": "python3.6"
+    },
+    {
+        "name": "python3-minimal"
+    },
+    {
+        "name": "python3.6-minimal"
+    },
+    {
+        "name": "libpython3-stdlib"
+    },
+    {
+        "name": "libpython3.6-stdlib"
+    },
+    {
+        "name": "libpython3.6"
+    },
+    {
+        "name": "libpython3.6-minimal"
+    },
+    {
+        "name": "python3-lib2to3"
+    },
+    {
+        "name": "libxslt1-dev"
+    },
+    {
+        "name": "libxml2-dev"
+    },
+    {
+        "name": "libxml2"
+    },
+    {
+        "name": "libharfbuzz-dev"
+    },
+    {
+        "name": "libharfbuzz0b"
+    },
+    {
+        "name": "libgraphite2-3"
+    },
+    {
+        "name": "libglib2.0-bin"
+    },
+    {
+        "name": "libglib2.0-dev-bin"
+    },
+    {
+        "name": "libharfbuzz-icu0"
+    },
+    {
+        "name": "libharfbuzz-gobject0"
+    },
+    {
+        "name": "gir1.2-harfbuzz-0.0"
+    },
+    {
+        "name": "libglib2.0-dev"
+    },
+    {
+        "name": "libgraphite2-dev"
+    },
+    {
+        "name": "libicu-dev"
+    },
+    {
+        "name": "libicu60"
+    },
+    {
+        "name": "libiculx60"
+    },
+    {
+        "name": "icu-devtools"
+    },
+    {
+        "name": "libicu-le-hb-dev"
+    },
+    {
+        "name": "libicu-le-hb0"
+    },
+    {
+        "name": "libglib2.0-0"
+    },
+    {
+        "name": "libxslt1.1"
     }
 ]
```

## ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8384615384615385%*

 * *Differences: {'101': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '114': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '119': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '120': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '3': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '86': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '87': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '88': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '89': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '94': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * '97': "{'version': '8.4.0-1ubuntu1~18.04'}",*

 * * 'i […]*

```diff
@@ -5,15 +5,16 @@
     {
         "name": "cpp"
     },
     {
         "name": "g++"
     },
     {
-        "name": "libgcc1"
+        "name": "libgcc1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "gcc-7-base"
     },
     {
         "name": "libasan4"
     },
@@ -254,60 +255,67 @@
     {
         "name": "libperl5.26"
     },
     {
         "name": "libgdbm-compat4"
     },
     {
-        "name": "libgomp1"
+        "name": "libgomp1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "libitm1"
+        "name": "libitm1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "libatomic1"
+        "name": "libatomic1",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "liblsan0"
+        "name": "liblsan0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "libisl19"
     },
     {
         "name": "libmpc3"
     },
     {
         "name": "libmpfr6"
     },
     {
         "name": "binutils"
     },
     {
-        "name": "libtsan0"
+        "name": "libtsan0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "linux-libc-dev"
     },
     {
         "name": "libc-dev-bin"
     },
     {
-        "name": "libcc1-0"
+        "name": "libcc1-0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "binutils-x86-64-linux-gnu"
     },
     {
         "name": "libbinutils"
     },
     {
         "name": "binutils-common"
     },
     {
-        "name": "gcc-8-base"
+        "name": "gcc-8-base",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "libselinux1"
     },
     {
         "name": "libselinux1-dev"
     },
@@ -338,15 +346,16 @@
     {
         "name": "libbz2-1.0"
     },
     {
         "name": "liblzma-dev"
     },
     {
-        "name": "libstdc++6"
+        "name": "libstdc++6",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "docker-ce",
         "version": "20.10.21"
     },
     {
         "name": "docker-ce-rootless-extras",
@@ -357,18 +366,20 @@
         "version": "20.10.21"
     },
     {
         "name": "containerd.io",
         "version": "1.6.10"
     },
     {
-        "name": "libquadmath0"
+        "name": "libquadmath0",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
-        "name": "libmpx2"
+        "name": "libmpx2",
+        "version": "8.4.0-1ubuntu1~18.04"
     },
     {
         "name": "libcilkrts5"
     },
     {
         "name": "libseccomp2"
     },
@@ -509,9 +520,87 @@
         "name": "pigz"
     },
     {
         "name": "dbus"
     },
     {
         "name": "libdbus-1-3"
+    },
+    {
+        "name": "python3-distutils"
+    },
+    {
+        "name": "python3"
+    },
+    {
+        "name": "python3-minimal"
+    },
+    {
+        "name": "libpython3-stdlib"
+    },
+    {
+        "name": "python3-lib2to3"
+    },
+    {
+        "name": "libxslt1-dev"
+    },
+    {
+        "name": "libxml2-dev"
+    },
+    {
+        "name": "libxml2"
+    },
+    {
+        "name": "libharfbuzz-dev"
+    },
+    {
+        "name": "libharfbuzz0b"
+    },
+    {
+        "name": "libgraphite2-3"
+    },
+    {
+        "name": "libglib2.0-bin"
+    },
+    {
+        "name": "libglib2.0-dev-bin"
+    },
+    {
+        "name": "libharfbuzz-icu0"
+    },
+    {
+        "name": "libharfbuzz-gobject0"
+    },
+    {
+        "name": "gir1.2-harfbuzz-0.0"
+    },
+    {
+        "name": "libglib2.0-dev"
+    },
+    {
+        "name": "libgraphite2-dev"
+    },
+    {
+        "name": "libicu-dev"
+    },
+    {
+        "name": "libicu60"
+    },
+    {
+        "name": "libiculx60"
+    },
+    {
+        "name": "icu-devtools"
+    },
+    {
+        "name": "libicu-le-hb-dev"
+    },
+    {
+        "name": "libicu-le-hb0"
+    },
+    {
+        "name": "libglib2.0-0"
+    },
+    {
+        "name": "libxslt1.1"
     }
 ]
```

## ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9617834394904459%*

 * *Differences: {'114': "{'version': '10.34-7'}",*

 * * '115': "{'version': '10.34-7'}",*

 * * '116': "{'version': '10.34-7'}",*

 * * '117': "{'version': '10.34-7'}",*

 * * '119': "{'version': '3.0-1'}",*

 * * '20': "{'version': '6.2-0ubuntu2'}",*

 * * '21': "{'version': '6.2-0ubuntu2'}",*

 * * '23': "{'version': '6.2-0ubuntu2'}",*

 * * 'delete': '[15]',*

 * * 'insert': "[(127, OrderedDict([('name', 'libhavege1')]))]"}*

```diff
@@ -41,17 +41,14 @@
     {
         "name": "libjsoncpp1"
     },
     {
         "name": "libuv1"
     },
     {
-        "name": "libhavege1"
-    },
-    {
         "name": "cmake"
     },
     {
         "name": "cmake-data"
     },
     {
         "name": "curl"
@@ -59,24 +56,27 @@
     {
         "name": "libcurl4"
     },
     {
         "name": "libtinfo5"
     },
     {
-        "name": "libtinfo-dev"
+        "name": "libtinfo-dev",
+        "version": "6.2-0ubuntu2"
     },
     {
-        "name": "libncurses5-dev"
+        "name": "libncurses5-dev",
+        "version": "6.2-0ubuntu2"
     },
     {
         "name": "libncurses5"
     },
     {
-        "name": "libncurses-dev"
+        "name": "libncurses-dev",
+        "version": "6.2-0ubuntu2"
     },
     {
         "name": "libldap-2.4-2"
     },
     {
         "name": "libgssapi3-heimdal"
     },
@@ -341,30 +341,35 @@
     {
         "name": "libselinux1"
     },
     {
         "name": "libselinux1-dev"
     },
     {
-        "name": "libpcre2-dev"
+        "name": "libpcre2-dev",
+        "version": "10.34-7"
     },
     {
-        "name": "libpcre2-16-0"
+        "name": "libpcre2-16-0",
+        "version": "10.34-7"
     },
     {
-        "name": "libpcre2-32-0"
+        "name": "libpcre2-32-0",
+        "version": "10.34-7"
     },
     {
-        "name": "libpcre2-posix2"
+        "name": "libpcre2-posix2",
+        "version": "10.34-7"
     },
     {
         "name": "python3-selinux"
     },
     {
-        "name": "libsepol1-dev"
+        "name": "libsepol1-dev",
+        "version": "3.0-1"
     },
     {
         "name": "libpcre3-dev"
     },
     {
         "name": "libpcre16-3"
     },
@@ -380,14 +385,17 @@
     {
         "name": "dctrl-tools"
     },
     {
         "name": "haveged"
     },
     {
+        "name": "libhavege1"
+    },
+    {
         "name": "libbz2-dev"
     },
     {
         "name": "libbz2-1.0"
     },
     {
         "name": "liblzma-dev"
```

## ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9351351351351351%*

 * *Differences: {'81': "{'version': '2.31-0ubuntu9.14'}",*

 * * '82': "{'version': '2.31-0ubuntu9.14'}",*

 * * 'delete': '[178, 174, 132, 113, 93, 92, 91, 90, 53, 52, 38]'}*

```diff
@@ -110,17 +110,14 @@
     {
         "name": "libsasl2-modules-db"
     },
     {
         "name": "libldap-common"
     },
     {
-        "name": "libnghttp2-14"
-    },
-    {
         "name": "librtmp1"
     },
     {
         "name": "libarchive13"
     },
     {
         "name": "librhash0"
@@ -152,20 +149,14 @@
     {
         "name": "libffi-dev"
     },
     {
         "name": "unzip"
     },
     {
-        "name": "libpci3"
-    },
-    {
-        "name": "pciutils"
-    },
-    {
         "name": "net-tools"
     },
     {
         "name": "libblas-dev"
     },
     {
         "name": "libgfortran-9-dev"
@@ -248,44 +239,34 @@
     {
         "name": "libaec-dev"
     },
     {
         "name": "pkg-config"
     },
     {
-        "name": "libc6-dev"
+        "name": "libc6-dev",
+        "version": "2.31-0ubuntu9.14"
     },
     {
-        "name": "libc6"
+        "name": "libc6",
+        "version": "2.31-0ubuntu9.14"
     },
     {
         "name": "libcrypt-dev"
     },
     {
         "name": "dpkg-dev"
     },
     {
         "name": "patch"
     },
     {
         "name": "libdpkg-perl"
     },
     {
-        "name": "perl"
-    },
-    {
-        "name": "perl-base"
-    },
-    {
-        "name": "perl-modules-5.30"
-    },
-    {
-        "name": "libperl5.30"
-    },
-    {
         "name": "libgdbm-compat4"
     },
     {
         "name": "libgomp1"
     },
     {
         "name": "libitm1"
@@ -335,17 +316,14 @@
     {
         "name": "libctf0"
     },
     {
         "name": "libctf-nobfd0"
     },
     {
-        "name": "gcc-10-base"
-    },
-    {
         "name": "libselinux1"
     },
     {
         "name": "libselinux1-dev"
     },
     {
         "name": "libpcre2-dev"
@@ -392,17 +370,14 @@
     {
         "name": "liblzma-dev"
     },
     {
         "name": "liblzma5"
     },
     {
-        "name": "libstdc++6"
-    },
-    {
         "name": "docker-ce",
         "version": "20.10.8"
     },
     {
         "name": "docker-ce-rootless-extras",
         "version": "20.10.8"
     },
@@ -525,29 +500,23 @@
     {
         "name": "libfile-fcntllock-perl"
     },
     {
         "name": "manpages-dev"
     },
     {
-        "name": "libgcc-s1"
-    },
-    {
         "name": "libncurses6"
     },
     {
         "name": "libncursesw6"
     },
     {
         "name": "libpcre2-8-0"
     },
     {
-        "name": "libpcre3"
-    },
-    {
         "name": "libsasl2-modules"
     },
     {
         "name": "libsepol1"
     },
     {
         "name": "libtinfo6"
```

## ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9214659685863874%*

 * *Differences: {'delete': '[133]',*

 * * 'insert': "[(4, OrderedDict([('name', 'libtirpc-common')])), (5, OrderedDict([('name', "*

 * *           "'libtirpc3')])), (26, OrderedDict([('name', 'gcc-12-base')])), (28, "*

 * *           "OrderedDict([('name', 'libasan5')])), (29, OrderedDict([('name', 'libasan8')])), (32, "*

 * *           "OrderedDict([('name', 'libhavege2')])), (34, OrderedDict([('name', "*

 * *           "'libgcc-12-dev')])), (52, OrderedDict([('name', 'libncurses6')])), (53, "*

 * *           "OrderedDict([('name', 'libncursesw6')])), […]*

```diff
@@ -8,14 +8,20 @@
     {
         "name": "rpcsvc-proto"
     },
     {
         "name": "libtirpc-dev"
     },
     {
+        "name": "libtirpc-common"
+    },
+    {
+        "name": "libtirpc3"
+    },
+    {
         "name": "libnsl-dev"
     },
     {
         "name": "libhwasan0"
     },
     {
         "name": "libgcc-9-dev"
@@ -68,26 +74,41 @@
     {
         "name": "g++"
     },
     {
         "name": "gcc-11-base"
     },
     {
+        "name": "gcc-12-base"
+    },
+    {
         "name": "libasan6"
     },
     {
+        "name": "libasan5"
+    },
+    {
+        "name": "libasan8"
+    },
+    {
         "name": "libubsan1"
     },
     {
         "name": "haveged"
     },
     {
+        "name": "libhavege2"
+    },
+    {
         "name": "libgcc-11-dev"
     },
     {
+        "name": "libgcc-12-dev"
+    },
+    {
         "name": "cpp-11"
     },
     {
         "name": "gcc-11"
     },
     {
         "name": "libstdc++-11-dev"
@@ -131,14 +152,20 @@
     {
         "name": "libncurses-dev"
     },
     {
         "name": "libldap-2.5-0"
     },
     {
+        "name": "libncurses6"
+    },
+    {
+        "name": "libncursesw6"
+    },
+    {
         "name": "libgssapi3-heimdal"
     },
     {
         "name": "libasn1-8-heimdal"
     },
     {
         "name": "libhcrypto4-heimdal"
@@ -365,14 +392,17 @@
     {
         "name": "binutils"
     },
     {
         "name": "libtsan0"
     },
     {
+        "name": "libtsan2"
+    },
+    {
         "name": "linux-libc-dev"
     },
     {
         "name": "libc-dev-bin"
     },
     {
         "name": "libcc1-0"
@@ -395,17 +425,14 @@
     {
         "name": "libctf-nobfd0"
     },
     {
         "name": "gcc-10-base"
     },
     {
-        "name": "libhavege2"
-    },
-    {
         "name": "libselinux1"
     },
     {
         "name": "libselinux1-dev"
     },
     {
         "name": "libpcre2-dev"
@@ -413,14 +440,17 @@
     {
         "name": "libpcre2-16-0"
     },
     {
         "name": "libpcre2-32-0"
     },
     {
+        "name": "libpcre2-8-0"
+    },
+    {
         "name": "libpcre2-posix3"
     },
     {
         "name": "python3-selinux"
     },
     {
         "name": "libsepol-dev"
@@ -431,14 +461,17 @@
     {
         "name": "libpcre16-3"
     },
     {
         "name": "libpcre32-3"
     },
     {
+        "name": "libpcre3"
+    },
+    {
         "name": "libpcrecpp0v5"
     },
     {
         "name": "dkms"
     },
     {
         "name": "dctrl-tools"
@@ -492,26 +525,32 @@
     {
         "name": "gcc-11-cross-base"
     },
     {
         "name": "libasan5-arm64-cross"
     },
     {
+        "name": "libasan6-arm64-cross"
+    },
+    {
         "name": "libatomic1-arm64-cross"
     },
     {
         "name": "libc6-arm64-cross"
     },
     {
         "name": "libc6-dev-arm64-cross"
     },
     {
         "name": "libgcc-9-dev-arm64-cross"
     },
     {
+        "name": "libgcc-s1"
+    },
+    {
         "name": "libgcc-s1-arm64-cross"
     },
     {
         "name": "libgomp1-arm64-cross"
     },
     {
         "name": "libitm1-arm64-cross"
```

## ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.9747474747474747%*

 * *Differences: {'delete': '[132]',*

 * * 'insert': "[(22, OrderedDict([('name', 'procps')])), (23, OrderedDict([('name', "*

 * *           "'lsb-release')])), (24, OrderedDict([('name', 'libncurses6')])), (25, "*

 * *           "OrderedDict([('name', 'libncursesw6')]))]"}*

```diff
@@ -62,14 +62,26 @@
     {
         "name": "libncurses5-dev"
     },
     {
         "name": "libhavege2"
     },
     {
+        "name": "procps"
+    },
+    {
+        "name": "lsb-release"
+    },
+    {
+        "name": "libncurses6"
+    },
+    {
+        "name": "libncursesw6"
+    },
+    {
         "name": "libncurses5"
     },
     {
         "name": "libncurses-dev"
     },
     {
         "name": "libldap-2.5-0"
@@ -392,17 +404,14 @@
     {
         "name": "liblzma-dev"
     },
     {
         "name": "liblzma5"
     },
     {
-        "name": "libstdc++6"
-    },
-    {
         "name": "docker-ce",
         "version": "23.0.1"
     },
     {
         "name": "docker-ce-rootless-extras",
         "version": "23.0.1"
     },
```

## ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json'), "*

 * *           "('sha256', '71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json'), "*

 * *           "('sha256', '4e0f51efe […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/aarch64",
         "filename": "ubuntu_arm64_18.04.tar.gz",
         "sha256": "933d8a4041c2fb92b8d4953a731d927a903f66adb39ba5efacb968537f8ff379",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/mindxdl/baseImages/aarch64/ubuntu_arm64_18.04.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/aarch64",
```

## ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json'), "*

 * *           "('sha256', '71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json'), "*

 * *           "('sha256', '4e0f51efe […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/x86_64",
         "filename": "alpine_amd64_latest.tar.gz",
         "sha256": "95193d0cdfb0d617978ad49d5a4adf0a46aae3cd9acd9416ab860c2b977a2e72",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/mindxdl/baseImages/x86_64/alpine_amd64_latest.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/x86_64",
```

## ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json'), "*

 * *           "('sha256', '71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json'), "*

 * *           "('sha256', '4e0f51efe […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/kubeedge/aarch64",
         "filename": "cloudcore",
         "sha256": "ccba5dfb5d48958517875e40fd1bfe2737bfcc5b8b5aafc0ffeed85b1a571a33",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/kubeedge/aarch64/cloudcore"
     },
     {
         "dest": "resources/mef",
```

## ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json'), "*

 * *           "('sha256', '71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json'), "*

 * *           "('sha256', '4e0f51efe […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/kubeedge/x86_64",
         "filename": "cloudcore",
         "sha256": "700007964724c1a844c939c096f686e802997111466489ab315cdf8a343b7bf6",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/kubeedge/x86_64/cloudcore"
     },
     {
         "dest": "resources/mef",
```

## ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/aarch64",
         "filename": "ubuntu_arm64_18.04.tar.gz",
         "sha256": "933d8a4041c2fb92b8d4953a731d927a903f66adb39ba5efacb968537f8ff379",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/mindxdl/baseImages/aarch64/ubuntu_arm64_18.04.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/aarch64",
```

## ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/x86_64",
         "filename": "alpine_amd64_latest.tar.gz",
         "sha256": "95193d0cdfb0d617978ad49d5a4adf0a46aae3cd9acd9416ab860c2b977a2e72",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/mindxdl/baseImages/x86_64/alpine_amd64_latest.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/x86_64",
```

## ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/kubeedge/aarch64",
         "filename": "cloudcore",
         "sha256": "147ef4e2386319d3a278ed145b4b98a1228c2a672718fbdddf7717ee5e477a5f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/kubeedge/aarch64/cloudcore"
     },
     {
         "dest": "resources/mef",
```

## ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/kubeedge/x86_64",
         "filename": "cloudcore",
         "sha256": "5c931f8c8c3779262390aeb9a3d7becfa6a9e3a94e593111bc07e83d7aa80d91",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/kubeedge/x86_64/cloudcore"
     },
     {
         "dest": "resources/mef",
```

## ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json

### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/aarch64",
         "filename": "ubuntu_arm64_18.04.tar.gz",
         "sha256": "933d8a4041c2fb92b8d4953a731d927a903f66adb39ba5efacb968537f8ff379",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/mindxdl/baseImages/aarch64/ubuntu_arm64_18.04.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/aarch64",
```

## ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json

### Pretty-printed

 * *Similarity: 0.8461538461538461%*

 * *Differences: {'insert': "[(0, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json'), "*

 * *           "('sha256', '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'), "*

 * *           "('dest', 'resources')])), (1, OrderedDict([('filename', 'version.json'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json'), "*

 * *           "('sha256', 'e06716192 […]*

```diff
@@ -1,9 +1,21 @@
 [
     {
+        "dest": "resources",
+        "filename": "version.json",
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
+    },
+    {
+        "dest": "resources/k8s",
+        "filename": "version.json",
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+    },
+    {
         "dest": "resources/mindxdl/baseImages/x86_64",
         "filename": "alpine_amd64_latest.tar.gz",
         "sha256": "95193d0cdfb0d617978ad49d5a4adf0a46aae3cd9acd9416ab860c2b977a2e72",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/mindxdl/baseImages/x86_64/alpine_amd64_latest.tar.gz"
     },
     {
         "dest": "resources/mindxdl/baseImages/x86_64",
```

## ascend_deployer/downloader/software/CANN_7.0.RC1.json

### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "name": "CANN",
     "other": [
         {
             "filename": "Ascend-cann-toolkit_7.0.RC1_linux-aarch64.zip",
             "sha256": "c01e83724631e0e43614b1e3fe72762ffee2ac7662cbcf17110d7e40dd3715dd",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%207.0.RC1/Ascend-cann-toolkit_7.0.RC1_linux-aarch64.zip"
         },
```

## ascend_deployer/downloader/software/DL_5.0.RC3.json

### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "name": "DL",
     "other": [],
     "required_soft": [
         {
             "name": "NPU",
             "version": "23.0.RC3"
         }
```

## ascend_deployer/downloader/software/MindSpore_2.2.0.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "framework_whl": [
         {
             "system": "linux_aarch64",
             "whl": [
                 {
                     "dest": "pylibs/Ascend",
                     "filename": "mindspore-2.2.0-cp39-cp39-linux_aarch64.whl",
```

## ascend_deployer/downloader/software/NPU_23.0.RC3.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "name": "NPU",
     "other": [
         {
             "dest": "resources/npu",
             "filename": "Ascend-hdk-310p-npu_23.0.rc3_linux-aarch64.zip",
             "sha256": "a39e480d30f6f104205ae50d07d39c17633184fa927fd36afa273dd50dbb9a58",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/Ascend%20HDK/Ascend%20HDK%2023.0.RC3/Ascend-hdk-310p-npu_23.0.rc3_linux-aarch64.zip"
```

## ascend_deployer/downloader/software/TensorFlow_2.6.5.json

### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'framework_whl'": "{0: {'whl': {insert: [(1, OrderedDict([('filename', "*

 * *                    "'tensorflow-2.6.5-cp38-cp38-manylinux2014_aarch64.whl'), ('url', "*

 * *                    "'https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow-2.6.5-cp38-cp38-manylinux2014_aarch64.whl'), "*

 * *                    "('dest', 'pylibs'), ('python', 'cp38'), ('sha256', "*

 * *                    "'5b6aae462b051eec7cdd4c1f306c3f521179fd44fc686fc9e342784e9b2c55e0')])), (2, "*

 * *            […]*

```diff
@@ -6,26 +6,54 @@
             "whl": [
                 {
                     "dest": "pylibs",
                     "filename": "tensorflow-2.6.5-cp37-cp37m-manylinux2014_aarch64.whl",
                     "python": "cp37",
                     "sha256": "daf14490ef2b9334c7472d25ca66640e2546bc8e446c6bc1d88e5d4855e75db6",
                     "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow-2.6.5-cp37-cp37m-manylinux2014_aarch64.whl"
+                },
+                {
+                    "dest": "pylibs",
+                    "filename": "tensorflow-2.6.5-cp38-cp38-manylinux2014_aarch64.whl",
+                    "python": "cp38",
+                    "sha256": "5b6aae462b051eec7cdd4c1f306c3f521179fd44fc686fc9e342784e9b2c55e0",
+                    "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow-2.6.5-cp38-cp38-manylinux2014_aarch64.whl"
+                },
+                {
+                    "dest": "pylibs",
+                    "filename": "tensorflow-2.6.5-cp39-cp39-manylinux2014_aarch64.whl",
+                    "python": "cp39",
+                    "sha256": "57a74254bee674b109cba949002920d7896480e83707e8ce4cb9d5a38a365c18",
+                    "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow-2.6.5-cp39-cp39-manylinux2014_aarch64.whl"
                 }
             ]
         },
         {
             "system": "linux_x86_64",
             "whl": [
                 {
                     "dest": "pylibs",
                     "filename": "tensorflow-2.6.5-cp37-cp37m-manylinux2010_x86_64.whl",
                     "python": "cp37",
                     "sha256": "46a9405ba55934b3e76a878626e05ab66f190954e2442f057722271c047020a9",
                     "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow-2.6.5-cp37-cp37m-manylinux2010_x86_64.whl"
+                },
+                {
+                    "dest": "pylibs",
+                    "filename": "tensorflow_cpu-2.6.5-cp38-cp38-manylinux2010_x86_64.whl",
+                    "python": "cp38",
+                    "sha256": "b42429b05cbe8105a45df47435ddcf4e709c510e0a8351f9970c38f1e4a1ba61",
+                    "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow_cpu-2.6.5-cp38-cp38-manylinux2010_x86_64.whl"
+                },
+                {
+                    "dest": "pylibs",
+                    "filename": "tensorflow_cpu-2.6.5-cp39-cp39-manylinux2010_x86_64.whl",
+                    "python": "cp39",
+                    "sha256": "3255a72cb4a3774c4dd05f53a6eff2ad8c8c7c2652cbda6aa724a5538c730d3d",
+                    "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindX/OpenSource/python/packages/tensorflow_cpu-2.6.5-cp39-cp39-manylinux2010_x86_64.whl"
                 }
             ]
         }
     ],
     "name": "TensorFlow",
     "version": "2.6.5"
 }
```

## ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "framework_whl": [
         {
             "system": "linux_aarch64",
             "whl": [
                 {
                     "dest": "pylibs",
                     "filename": "torch-1.11.0-cp37-cp37m-linux_aarch64.whl",
```

## ascend_deployer/group_vars/all.yaml

```diff
@@ -15,14 +15,16 @@
 first_host: "{{ ansible_play_hosts_all[0] }}"
 no_copy_flag: "{{ NO_COPY | default('false') }}"
 use_harbor: "{{ HARBOR_SERVER | length != 0 }}"
 use_mindxdl: "{{ SCENE_NUM != 4 }}"
 HARBOR_HTTP: true
 ascend_deployer_work_dir: "{{ ansible_config_file | dirname }}"
 resource_dir: "{{ ascend_deployer_work_dir }}/resources"
+resource_path: "~/resources"
+resources_dir: "~/resources"
 
 docker_daemonfile_path: "/etc/docker/daemon.json"
 
 # 安装组件名称列表
 DOCKER_COMPONENT: "docker"
 K8S_COMPONENT: "k8s"
 DOCKER_RUNTIME_COMPONENT: "docker-runtime"
@@ -42,14 +44,15 @@
           3: ["{{DOCKER_RUNTIME_COMPONENT}}", "{{DEVICE_PLUGIN_COMPONENT}}"],
           4: ["{{DOCKER_COMPONENT}}", "{{K8S_COMPONENT}}"]
 }
 
 NO_DOCKER_K8S_SCENES: [2, 3]
 SCENE_NUM: 1
 EXTRA_COMPONENT: ""
+NODE_NAME: "{{ set_hostname if set_hostname is defined else ansible_hostname }}"
 
 # NPU
 user: HwHiAiUser
 group: HwHiAiUser
 install_path: /usr/local/Ascend
 
 # K8S
```

## ascend_deployer/playbooks/check.yaml

```diff
@@ -1,23 +1,17 @@
 - hosts:
     - localhost
     - master
     - worker
-  gather_facts: false
-  become: yes
-  vars_files:
-    - roles/mindx.basic/defaults/main.yml
+  name: check status for space, inventory, k8s and driver
   tasks:
-  - include_tasks: roles/mindx.basic/tasks/check.yml
-  - include_tasks: roles/mindx.basic/tasks/check_driver.yml
-
-- hosts:
-    - localhost
-    - master
-    - worker
-  become: yes
-  vars_files:
-    - roles/mindx.basic/defaults/main.yml
-  tasks:
-  - include_tasks: roles/mindx.basic/tasks/k8s_check.yml
-    when:
-      - "K8S_COMPONENT in (SCENES[SCENE_NUM] + EXTRA_COMPONENT.split(','))"
+    - name: check
+      check_status:
+        tags: "{{ ansible_run_tags }}"
+        master_groups: "{{ groups['master'] }}"
+        worker_groups: "{{ groups['worker'] }}"
+        current_hostname: "{{ inventory_hostname }}"
+        kube_vip: "{{ KUBE_VIP }}"
+        k8s_api_server_ip: "{{ k8s_api_server_ip | default('') }}"
+        kube_interface: "{{ kube_interface | default('') }}"
+        pod_network_cidr: "{{ POD_NETWORK_CIDR }}"
+        use_k8s_version: "{{ use_k8s_version }}"
```

## ascend_deployer/playbooks/distribution.yml

```diff
@@ -1,27 +1,18 @@
-- hosts: localhost
+- hosts: "{{hosts_name}}"
+  name: distribution - copy and uncompress
   tasks:
-    - name: make tar package for remote
-      shell: tar -cf ~/resources.tar ../resources
-
-- hosts: '{{ hosts_name }}'
-  tasks:
-    - name: copy to remote hosts
-      copy:
-        src: ~/resources.tar
-        dest: ~/
-      when: ansible_connection != "local"
-
-    - name: clean remote resources
-      file:
-        state: absent
-        path: ~/resources
-      when: ansible_connection != "local"
+    - name: scp to remote hosts
+      scp:
+        ip: "{{inventory_hostname}}"
+        remote_user: "{{ansible_ssh_user}}"
+        passwd: "{{ansible_ssh_pass|default('')}}"
+        src: "~/resources_{{ansible_architecture}}.tar ../resources/{{os_and_arch}}/bzip2* ../resources/{{os_and_arch}}/unzip* ../resources/{{os_and_arch}}/tar*"
+        dest: "~/"
+      delegate_to: localhost
+      when:
+        - inventory_hostname != "localhost"
 
     - name: uncompress on remote
-      unarchive:
-        src: ~/resources.tar
-        dest: ~/
-        copy: no
-        owner: "{{ ansible_ssh_user }}"
-        group: "{{ ansible_ssh_user }}"
-      when: ansible_connection != "local"
+      uncompress_resources:
+        resources_dir: "{{ resource_path }}"
+        tags: "{{ ansible_run_tags }}"
```

## ascend_deployer/playbooks/docker.yaml

```diff
@@ -1,49 +1,51 @@
 ---
 # install docker
 - hosts:
-    - localhost
     - master
     - worker
+  name: docker main
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.docker/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.docker/tasks/main.yml
 
 - hosts:
     - master
     - worker
+  name: docker install
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.docker/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.docker/tasks/install.yml
       when:
         - not docker_installed
+        - not skip_sys_pkg
 
 - hosts:
-    - localhost
     - master
     - worker
+  name: docker install containerd nerdctl
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.docker/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.docker/tasks/install_containerd.yml
       when:
         - not use_old_k8s_version
     - include_tasks: roles/mindx.docker/tasks/install_nerdctl.yml
 
 - hosts:
-    - localhost
     - master
     - worker
+  name: docker post install
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.docker/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.docker/tasks/post_install.yml
```

## ascend_deployer/playbooks/gather_npu_fact.yml

```diff
@@ -1,52 +1,23 @@
-- name: gather facts for all
+- name: sync time
   hosts: all
-  gather_facts: False
-
   tasks:
-    - name: gather facts first
-      setup:
-        fact_path: /notexist
-
     - name: sync time
       import_tasks: sync_time.yml
-      when: ansible_user_uid == 0
+      when: ansible_ssh_user == 'root'
 
     - name: create user if not exist
-      import_tasks: create_user.yml
-      when: ansible_user_uid == 0
-
-    - set_fact: python_minor={{python_version[:-2]}}
-
-    - name: get python version
-      debug: var=python_minor
-
-    - name: set custom fact tasks
-      import_tasks: task_set_custom_fact.yml
+      create_user:
+        group: "{{ group }}"
+        user: "{{ user }}"
+      when: ansible_ssh_user == 'root'
 
-    - name: create facts.d folder
-      file:
-        path: ~/ansible/facts.d/
-        state: directory
-        mode: 0750
-        recurse: yes
-
-    - name: copy npu_info.fact to host
-      template:
-        src: facts/npu_info.fact.j2
-        dest: ~/ansible/facts.d/npu_info.fact
-        mode: "0550"
-
-    - name: gather facts again
-      setup:
-        fact_path: ~/ansible/facts.d/
-
-    - name: set kube_interface
-      set_fact:
-        kube_interface: "{{ ansible_default_ipv4.interface }}"
-        cacheable: yes
-      when:
-        - groups['master'] | length > 1
-        - inventory_hostname in groups['master']
-
-- name: set facts_cache dir permission
-  import_playbook: set_facts_cache_permission.yml
+- name: gather facts for all
+  hosts:
+    - localhost
+    - master
+    - worker
+  tasks:
+    - name: collect basic info
+      collect_info:
+        tags: "{{ ansible_run_tags }}"
+        is_ipv6: "{{working_on_ipv6}}"
```

## ascend_deployer/playbooks/harbor.yaml

```diff
@@ -1,8 +1,15 @@
 - hosts:
     - localhost
     - master
     - worker
   gather_facts: false
-  become: yes
-  roles:
-    - role: mindx.harbor
+  name: config harbor info
+  tasks:
+    - name: login harbor
+      throttle: 1
+      login_harbor:
+        current_hostname: "{{ inventory_hostname }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        ca_file: "{{ HARBOR_CA_FILE }}"
```

## ascend_deployer/playbooks/k8s.yaml

```diff
@@ -2,26 +2,28 @@
 # 检查K8s是否初始化了
 # 分发软件包
 # 基础设置
 - hosts:
     - localhost
     - master
     - worker
+  name: check k8s and init
   max_fail_percentage: 1
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/install/main.yml
 
 # 安装K8s
 - hosts:
     - master
     - worker
+  name: install k8s
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/install/install.yml
       when:
@@ -29,41 +31,44 @@
     - include_tasks: roles/mindx.k8s/tasks/install/os_setting.yml
       when:
         - not k8s_initialized
 
 # init kubevip
 - hosts:
     - master[0]
+  name: init kubevip
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/defaults/main.yml
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/kubevip/main.yml
       when:
         - groups['master'] | length > 2
         - not k8s_initialized
 
 # k8s master init
 - hosts:
     - master[0]
+  name: k8s master init
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/defaults/main.yml
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/master/main.yml
       when:
         - not k8s_initialized
 
 # master join k8s
 - hosts:
     - master
+  name: master join k8s
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/defaults/main.yml
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/master_backup/main.yml
@@ -75,14 +80,15 @@
       when:
         - groups['master'] | length > 2
         - inventory_hostname != groups['master'][0]
         - not k8s_initialized
 
 # worker join k8s
 - hosts: worker
+  name: worker join k8s
   gather_facts: false
   become: yes
   vars_files:
     - roles/mindx.k8s/defaults/main.yml
     - roles/mindx.k8s/vars/main.yml
   tasks:
     - include_tasks: roles/mindx.k8s/tasks/worker/main.yml
```

## ascend_deployer/playbooks/report.yaml

```diff
@@ -1,20 +1,59 @@
 - hosts:
-    - localhost
     - master
     - worker
-  gather_facts: true
-  vars_files:
-    - roles/mindx.rep/defaults/main.yml
+  name: collect package and system info
   tasks:
-    - include_tasks: roles/mindx.rep/tasks/packages_rep.yaml
-      when: (groups['master'] + groups['worker'])|length > 0 and ansible_play_batch|length > 0
+    - name: clean caches
+      shell: "rm {{ playbook_dir }}/../report/cache/ -rf"
+      delegate_to: localhost
+      when: only_package | default('false') != "true"
+      run_once: yes
 
+    - name: collect package and system info
+      system_report:
+        ip: "{{ inventory_hostname }}"
+        only_package: "{{ only_package | default('false') }}"
 
 - hosts:
-    - localhost
-  gather_facts: true
-  vars_files:
-    - roles/mindx.rep/defaults/main.yml
+    - master
+  name: collect k8s info
   tasks:
-    - include_tasks: roles/mindx.rep/tasks/local_rep.yaml
-      when: not only_package and (groups['master'] + groups['worker'])|length > 0 and ansible_play_batch|length > 0
+    - name: collect k8s info
+      script: "../scripts/k8s_rep.py '~/smartkit/reports' {{SCENE_NUM|default('1')}}"
+      when: only_package | default('false') != "true"
+      run_once: yes
+      args:
+        executable: "{{ discovered_interpreter_python }}"
+      environment:
+        http_proxy: ""
+        https_proxy: ""
+        HTTP_PROXY: ""
+        HTTPS_PROXY: ""
+
+    - name: fetch k8s reports
+      fetch:
+        src: "~/smartkit/reports/node_dict.json"
+        dest: "{{ playbook_dir }}/../report/cache/{{ inventory_hostname }}/"
+        flat: yes
+      run_once: yes
+      when: only_package | default('false') != "true"
+      ignore_errors: yes
+
+- name: fetch reports
+  hosts:
+    - master
+    - worker
+  tasks:
+    - name: fetch system reports
+      fetch:
+        src: "~/smartkit/reports/local_info.json"
+        dest: "{{ playbook_dir }}/../report/cache/{{ inventory_hostname }}/"
+        flat: yes
+      when: only_package | default('false') != "true"
+
+    - name: process report
+      shell: "{{ ansible_playbook_python }} ../scripts/create_report.py 
+      '{{ playbook_dir }}/../report/cache/' '{{ playbook_dir }}/../report/' '{{ playbook_dir }}/../inventory_file'"
+      delegate_to: localhost
+      run_once: yes
+      when: only_package | default('false') != "true"
```

## ascend_deployer/playbooks/install/install_ascend-device-plugin.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for ascend-device-plugin
+  tasks:
+    - name: build device-plugin image
+      install_device_plugin:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch device-plugin image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ device_plugin_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/device-plugin"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push ascend-device-plugin image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "device-plugin"
+      when: use_harbor
+
+- hosts:
     - worker
-  become: yes
+  name: install or upgrade ascend-device-plugin
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/deviceplugin.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/device-plugin/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/device-plugin/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install device-plugin
+      install_device_plugin:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply device-plugin
+      throttle: 1
+      install_device_plugin:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ device_plugin_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml

```diff
@@ -1,5 +1,6 @@
-- hosts:
-    - worker
-  become: yes
+- hosts: worker
+  name: install ascend-docker-runtime
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/docker-runtime.yaml
+    - name: install docker runtime
+      install_docker_runtime:
+        resources_dir: "{{ resource_path }}"
```

## ascend_deployer/playbooks/install/install_ascend-operator.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for ascend-operator
+  tasks:
+    - name: build ascend-operator image
+      install_ascend_operator:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch ascend-operator image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ ascend_operator_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/ascend-operator"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push ascend-operator image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "ascend-operator"
+      when: use_harbor
+
+- hosts:
     - master
-  become: yes
+  name: install or upgrade ascend-operator
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/ascend-operator.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/ascend-operator/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/ascend-operator/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install ascend-operator
+      install_ascend_operator:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply ascend-operator
+      throttle: 1
+      install_ascend_operator:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ ascend_operator_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_atlasedge.yml

```diff
@@ -1,11 +1,14 @@
 - hosts: '{{ hosts_name }}'
+  name: install atlasedge
   tasks:
     - name: create user
-      import_tasks: ../create_user.yml
+      create_user:
+        group: "{{ group }}"
+        user: "{{ user }}"
       when: ansible_user_uid == 0
 
     - name: message
       debug:
         msg:
         - "[ASCEND]not support installing atlasedge by non-root user, please switch to root user"
       when: ansible_user_uid != 0
```

## ascend_deployer/playbooks/install/install_docker_images.yml

```diff
@@ -1,8 +1,9 @@
 - hosts: '{{ hosts_name }}'
+  name: install docker_images
   tasks:
     - name: install docker images
       import_tasks: task_docker_images.yml
       when: ansible_user_uid == 0
 
     - name: message
       debug:
```

## ascend_deployer/playbooks/install/install_driver.yml

```diff
@@ -1,46 +1 @@
-- hosts: '{{ hosts_name }}'
-  tasks:
-    - name: is install tool
-      shell: command -v npu-smi | wc -l
-      register: isInstalledTool
-      when: ansible_user_uid == 0
-
-    - name: check health
-      shell: npu-smi info|grep -E '910|710|310P|310'|awk -F' ' '{print $5}'|grep -v '|'
-      register: result_info
-      when:
-        - ansible_user_uid == 0      
-        - isInstalledTool.stdout != "0"
-
-    - name: is everychip ok
-      set_fact: NPUIssue=true
-      when:
-        - ansible_user_uid == 0      
-        - isInstalledTool.stdout != "0"
-        - result_info is defined
-        - item != 'OK'
-      loop: "{{result_info.stdout_lines}}"
-
-    - name: message
-      debug:
-        msg:
-          - "critical issue with NPU, please check it"
-      failed_when: true
-      when:
-        - NPUIssue is defined
-        - force_upgrade_npu == 'false'
-
-    - name: import driver task
-      import_tasks: task_driver.yml
-      when: ansible_user_uid == 0
-
-    - name: message
-      debug:
-        msg:
-        - "[ASCEND]not support installing driver by non-root user, please switch to root user"
-      when: ansible_user_uid != 0
-
-    - name: fail if not root
-      fail:
-        msg: "[ASCEND]can not install with non-root"
-      when: "'driver' in ansible_run_tags and ansible_user_uid != 0"
+PLACEHOLDER
```

## ascend_deployer/playbooks/install/install_firmware.yml

```diff
@@ -1,47 +1 @@
-- hosts: '{{ hosts_name }}'
-  tasks:       
-        
-    - name: is install tool
-      shell: command -v npu-smi | wc -l
-      register: isInstalledTool
-      when: ansible_user_uid == 0
-
-    - name: check health
-      shell: npu-smi info|grep -E '910|710|310P|310'|awk -F' ' '{print $5}'|grep -v '|'
-      register: result_info
-      when: 
-        - ansible_user_uid == 0      
-        - isInstalledTool.stdout != "0"
-
-    - name: is everychip ok
-      set_fact: NPUIssue=true
-      when:
-        - ansible_user_uid == 0      
-        - isInstalledTool.stdout != "0"
-        - result_info is defined
-        - item != 'OK'
-      loop: "{{result_info.stdout_lines}}"
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]critical issue with NPU, please check it"
-      failed_when: true
-      when:
-        - NPUIssue is defined
-        - force_upgrade_npu == 'false'
-
-    - name: import firmware task
-      import_tasks: task_firmware.yml
-      when: ansible_user_uid == 0
-
-    - name: message
-      debug:
-        msg:
-        - "[ASCEND]not support installing firmware by non-root user, please switch to root user"
-      when: ansible_user_uid != 0
-
-    - name: fail if not root
-      fail:
-        msg: "[ASCEND]can not install with non-root"
-      when: "'firmware' in ansible_run_tags and ansible_user_uid != 0"
+PLACEHOLDER
```

## ascend_deployer/playbooks/install/install_ha.yml

```diff
@@ -1,11 +1,14 @@
 - hosts: '{{ hosts_name }}'
+  name: install ha
   tasks:
     - name: create user
-      import_tasks: ../create_user.yml
+      create_user:
+        group: "{{ group }}"
+        user: "{{ user }}"
       when: ansible_user_uid == 0
 
     - name: install ha
       import_tasks: task_ha.yml
       when: ansible_user_uid == 0
 
     - name: message
```

## ascend_deployer/playbooks/install/install_hccl-controller.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for hccl-controller
+  tasks:
+    - name: build hccl-controller image
+      install_hccl_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch hccl-controller image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ hccl_controller_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/hccl-controller"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push hccl-controller image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "hccl-controller"
+      when: use_harbor
+
+- hosts:
     - master
-  become: yes
+  name: install or upgrade hccl-controller
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/hccl.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/hccl-controller/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/hccl-controller/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install hccl-controller
+      install_hccl_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply hccl-controller
+      throttle: 1
+      install_hccl_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ hccl_controller_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_ief.yml

```diff
@@ -1,8 +1,9 @@
 - hosts: '{{ hosts_name }}'
+  name: install ief
   tasks:
     - name: install ief
       import_tasks: task_ief.yml
       when: ansible_user_uid == 0
 
     - name: message
       debug:
```

## ascend_deployer/playbooks/install/install_kernels.yml

```diff
@@ -1,4 +1,17 @@
 - hosts: '{{ hosts_name }}'
+  name: install kernels
   tasks:
     - name: install kernels
-      import_tasks: task_kernels.yml
+      install_cann:
+        pkg_name: "kernels"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+      register: kernels_result
+      failed_when: kernels_result.rc != 0
+
+    - name: message
+      debug:
+        var: kernels_result
+      failed_when: kernels_result.rc != 0
```

## ascend_deployer/playbooks/install/install_mindio.yml

```diff
@@ -1,5 +1,25 @@
-- hosts:
-    - worker
-  become: yes
+- hosts: worker
+  name: install mindio
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/mindio.yaml
+    # 创建用戶組
+    - name: create group HwHiAiUser
+      ansible.builtin.group:
+        name: "HwHiAiUser"
+        state: present
+      ignore_errors: true
+
+    # 创建用戶
+    - name: create user hwMindX
+      ansible.builtin.user:
+        name: "hwMindX"
+        comment: "hwMindX"
+        group: "HwHiAiUser"
+        groups: "HwHiAiUser"
+        append: yes
+        state: present
+        shell: "{{ '/usr/sbin/nologin' if os_name == 'Ubuntu' else '/sbin/nologin' }}"
+      ignore_errors: true
+
+    - name: install mindio
+      install_mindio:
+        resources_dir: "{{ resource_path }}"
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## ascend_deployer/playbooks/install/install_mindspore.yml

```diff
@@ -1,30 +1,9 @@
 - hosts: '{{ hosts_name }}'
+  name: install mindspore
   tasks:
-    - name: check mindspore
-      shell: python3 -m pip list | grep mindspore
-      environment:
-        PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
-        LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
-      failed_when: false
-      changed_when: false
-      register: mindspore_version
-
-    - name: message
-      debug: var=mindspore_version
-      when: mindspore_version.stdout != ""
-
-    - name: message
-      debug:
-        msg:
-          - "mindspore is already installed, mindspore install skipped"
-      when: mindspore_version.stdout != ""
-
-    - name: get cmake version
-      shell: cmake --version | awk -F" " '{print $3;exit}'
-      register: cmake_ver
-      when: mindspore_version.stdout == ''
-
-    - name: install mindspore if not import
-      include_tasks: task_mindspore.yml
-      when:
-        - mindspore_version.stdout == ''
+    - name: install mindspore
+      process_framework:
+        resource_dir: "{{resource_path}}"
+        pkg_name: "mindspore"
+        python_version: "{{python_version}}"
+        ansible_run_tags: "{{ansible_run_tags}}"
```

## ascend_deployer/playbooks/install/install_mindstudio.yml

```diff
@@ -1,8 +1,9 @@
 - hosts: '{{ hosts_name }}'
+  name: install mindstudio
   tasks:
     - name: find mindstudio dir
       find:
         path: "{{ resources_dir }}"
         recurse: no
         file_type: directory
         use_regex: yes
@@ -48,83 +49,82 @@
       set_fact:
         ms: "{{mindstudio_pkg}}"
         cacheable: yes
       when: mindstudio_pkg.matched is defined and mindstudio_pkg.matched > 0
 
     - name: copy py_compile
       ansible.builtin.copy:
-        src: /usr/local/{{ python_version }}/lib/{{ python_minor }}/py_compile.py
-        dest: /usr/lib/{{ python_minor }}/
+        src: /usr/local/{{ python_version }}/lib/{{ python_version[:-2] }}/py_compile.py
+        dest: /usr/lib/{{ python_version[:-2] }}/
         remote_src: no
       when:
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - ansible_user_uid == 0
 
     - name: check ubuntu desktop
       shell: dpkg -l ubuntu-desktop | wc -l
       register: ubuntu_desktop
       changed_when: false
       when: 
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - "'Ubuntu' in os_and_arch"
         - ansible_user_uid == 0
 
     - name: install system packages ubuntu desktop
-      shell: export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ mindstudio_dir }}/{{ os_and_arch }}/desktop/*.deb
+      shell: "export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ mindstudio_dir }}/{{ os_and_arch }}/desktop/*.deb"
       register: apt_desktop_result
       environment:
         PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
         LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
       when:
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - "'Ubuntu' in os_and_arch"
         - ubuntu_desktop is not skipped and ubuntu_desktop.stdout=='0'
         - ansible_user_uid == 0
 
     - name: message
       debug: var=apt_desktop_result
       when: apt_desktop_result.changed
 
     - name: install system packages apt
-      shell: export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ mindstudio_dir }}/{{ os_and_arch }}/*.deb
+      shell: "export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ mindstudio_dir }}/{{ os_and_arch }}/*.deb"
       register: apt_result
       environment:
         PATH: /usr/local/{{ python_version }}/bin:{{ ansible_env.PATH }}
         LD_LIBRARY_PATH: /usr/local/{{ python_version }}/lib:/usr/local/gcc7.3.0/lib64
       when:
-        - ms.matched > 0
-        - ansible_pkg_mgr == 'apt'
+        - ms is defined and ms.matched > 0
+        - not use_rpm_command
         - ansible_user_uid == 0
 
     - name: message
       debug: var=apt_result
       when: apt_result.changed
 
     - name: install system packages rpm
-      shell: rpm -ivh --force --nodeps --replacepkgs {{ mindstudio_dir }}/{{ os_and_arch }}/*.rpm
+      shell: "rpm -ivh --force --nodeps --replacepkgs {{ mindstudio_dir }}/{{ os_and_arch }}/*.rpm"
       register: yum_result
       when:
-        - ms.matched > 0
-        - ansible_pkg_mgr == 'yum'
+        - ms is defined and ms.matched > 0
+        - use_rpm_command
         - ansible_user_uid == 0
 
     - name: message
       debug: var=yum_result
       when: yum_result.changed
 
     - name: install python libs for mindstudio
-      shell: "{{ python_minor }} -m pip install --force-reinstall {{ item }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}"
+      shell: "python3 -m pip install --force-reinstall {{ item }} --no-index --find-links {{ resources_dir }}/pylibs"
       environment:
         PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
         LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/lib64:{{ local_path }}/gcc7.3.0/lib64"
       failed_when: false
-      when: ms.matched > 0
+      when: ms is defined and ms.matched > 0
       with_items:
         - grpcio
-        - grpcio-tools
         - protobuf
         - decorator
         - sympy
         - psutil
         - requests
         - pandas
         - xlrd
@@ -150,15 +150,15 @@
 
     - name: unarchive MindStudio
       unarchive:
         src: "{{ ms.files[0].path }}"
         dest: ~/
         copy: no
         mode: 0750
-      when: ms.matched > 0
+      when: ms is defined and ms.matched > 0
 
     - name: find jdk-aarch64 package
       find:
         paths: "{{ mindstudio_dir }}"
         recurse: no
         file_type: file
         use_regex: yes
@@ -168,15 +168,15 @@
     - name: unarchive jdk for aarch64
       unarchive:
         src: "{{ jdk_aarch64_dir.files[0].path }}"
         dest: ~/MindStudio
         copy: no
         mode: 0750
       when:
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - ansible_architecture == 'aarch64'
         - jdk_aarch64_dir.matched > 0
 
     - name: find jdk-x64 package
       find:
         paths: "{{ mindstudio_dir }}"
         recurse: no
@@ -187,35 +187,35 @@
 
     - name: unarchive jdk for x86_64
       unarchive:
         src: "{{ jdk_x64_dir.files[0].path }}"
         dest: ~/MindStudio
         copy: no
       when:
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - ansible_architecture == 'x86_64'
         - jdk_x64_dir.matched > 0
 
     - name: chmod MindStudio to 750
       file:
         path: ~/MindStudio
         mode: 0750
         recurse: yes
-      when: ms.matched > 0
+      when: ms is defined and ms.matched > 0
 
     - name: set MINDSTUDIO_JDK
       shell: sed -i "2 i\export MINDSTUDIO_JDK=~/MindStudio/jbr" ~/MindStudio/bin/MindStudio.sh
       failed_when: false
       when:
-        - ms.matched > 0
+        - ms is defined and ms.matched > 0
         - ansible_architecture == 'aarch64'
 
     - name: message
       debug:
         msg:
         - "[ASCEND]can not find mindstudio package, mindstudio install skipped"
-      when: ms.matched == 0
+      when: ms is defined and ms.matched == 0
 
     - name: fail if this install
       fail:
         msg: "[ASCEND]fail to install mindstudio"
-      when: "'mindstudio' in ansible_run_tags and ms.matched == 0"
+      when: "'mindstudio' in ansible_run_tags and ms is defined and ms.matched == 0"
```

## ascend_deployer/playbooks/install/install_nnae.yml

```diff
@@ -1,4 +1,17 @@
 - hosts: '{{ hosts_name }}'
+  name: install nnae
   tasks:
     - name: install nnae
-      import_tasks: task_nnae.yml
+      install_cann:
+        pkg_name: "nnae"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+      register: nnae_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnae_result
+      failed_when: nnae_result.rc != 0
```

## ascend_deployer/playbooks/install/install_nnrt.yml

```diff
@@ -1,4 +1,17 @@
 - hosts: '{{ hosts_name }}'
+  name: install nnrt
   tasks:
     - name: install nnrt
-      import_tasks: task_nnrt.yml
+      install_cann:
+        pkg_name: "nnrt"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+      register: nnrt_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnrt_result
+      failed_when: nnrt_result.rc != 0
```

## ascend_deployer/playbooks/install/install_noded.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for noded
+  tasks:
+    - name: build noded image
+      install_noded:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch noded image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ noded_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/noded"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push noded image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "noded"
+      when: use_harbor
+
+- hosts:
     - worker
-  become: yes
+  name: install or upgrade noded
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/noded.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/noded/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/noded/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install noded
+      install_noded:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply noded
+      throttle: 1
+      install_noded:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ noded_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_npu-exporter.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for npu-exporter
+  tasks:
+    - name: build npu-exporter image
+      install_npu_exporter:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch npu-exporter image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ npu_exporter_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/npu-exporter"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push npu-exporter image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "npu-exporter"
+      when: use_harbor
+
+- hosts:
     - worker
-  become: yes
+  name: install or upgrade npu-exporter
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/npu-exporter.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/npu-exporter/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/npu-exporter/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install npu-exporter
+      install_npu_exporter:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply npu-exporter
+      throttle: 1
+      install_npu_exporter:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ npu_exporter_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_npu.yml

```diff
@@ -1,49 +1,14 @@
 - hosts: '{{ hosts_name }}'
+  name: install npu
   tasks:
-    - name: is install tool
-      shell: command -v npu-smi | wc -l
-      register: isInstalledTool
-      when: ansible_user_uid == 0
+    - name: install npu
+      process_npu:
+        force_upgrade_npu: "{{ force_upgrade_npu }}"
+        resource_dir: "{{ resource_path }}"
+        cus_npu_info: "{{ cus_npu_info | default('') }}"
+        ansible_run_tags: "{{ ansible_run_tags }}"
+      register: install_npu_result
 
-    - name: check health
-      shell: npu-smi info|grep -E '910|710|310P|310'|awk -F' ' '{print $5}'|grep -v '|'
-      register: result_info
-      when: 
-        - ansible_user_uid == 0
-        - isInstalledTool.stdout != "0"
-
-    - name: is everychip ok
-      set_fact: NPUIssue=true
-      when:
-        - ansible_user_uid == 0
-        - isInstalledTool.stdout != "0"
-        - result_info is defined
-        - item != 'OK'
-      loop: "{{result_info.stdout_lines}}"
-
-    - name: message
-      debug:
-        msg:
-          - "critical issue with NPU, please check it"
-      failed_when: true
-      when:
-        - NPUIssue is defined
-        - force_upgrade_npu == 'false'
-
-    - name: import firmware task
-      import_tasks: task_firmware.yml
-      when: ansible_user_uid == 0 and isInstalledTool.stdout != "0"
-
-    - name: import all driver task
-      import_tasks: task_driver.yml
-      when: ansible_user_uid == 0
-
-    - name: import firmware task
-      import_tasks: task_firmware.yml
-      when: ansible_user_uid == 0 and isInstalledTool.stdout == "0"
-
-    - name: message
+    - name: show reboot message
       debug:
-        msg:
-        - "not support installing npu by non-root user, please switch to root user"
-      when: ansible_user_uid != 0
+        var: install_npu_result.stdout_lines
```

## ascend_deployer/playbooks/install/install_python.yml

```diff
@@ -1,4 +1,8 @@
 - hosts: '{{ hosts_name }}'
+  name: install python3.x.x
   tasks:
     - name: install python3.x.x
-      import_tasks: task_python.yml
+      install_python:
+        resources_dir: "{{resource_path}}"
+        python_tar: "{{python_tar}}"
+        os_and_arch: "{{os_and_arch}}"
```

## ascend_deployer/playbooks/install/install_pytorch.yml

```diff
@@ -1,87 +1,10 @@
 - hosts: '{{ hosts_name }}'
+  name: install pytorch
   tasks:
-    - name: try import pytorch
-      shell: python3 -c "import torch; print(torch.__version__)"
-      environment:
-        PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
-        LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/lib64:{{ ascend_install_path }}/nnae/latest/fwkacllib/lib64:{{ local_path }}/gcc7.3.0/lib64"
-      failed_when: false
-      changed_when: false
-      register: import_torch
+    - name: install pytorch
+      process_framework:
+        resource_dir: "{{resource_path}}"
+        pkg_name: "pytorch"
+        python_version: "{{python_version}}"
+        ansible_run_tags: "{{ansible_run_tags}}"
 
-    - name: message
-      debug: var=import_torch
-      when: import_torch.rc == 0
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]pytorch is already installed, pytorch install skipped"
-      when: import_torch.rc == 0
-
-    - name: stat gcc-7.3.0
-      stat:
-        path: "{{ local_path }}/gcc7.3.0"
-      register: gcc_stat
-      when: import_torch.rc != 0
-
-    - name: install gcc 7.3 for CentOS 7.6
-      import_tasks: task_gcc.yml
-      when:
-        - import_torch.rc != 0
-        - not gcc_stat.stat.exists
-        - "'CentOS_7.6' in os_and_arch"
-
-    - name: find pytorch whl package
-      find:
-        paths: "{{ resources_dir }}/pylibs"
-        recurse: no
-        file_type: file
-        use_regex: yes
-        patterns: ".*torch-.*{{ ansible_architecture }}.whl"
-      register: pytorch_whl
-      when: import_torch.rc != 0
-
-    - name: find torch_npu whl package
-      find:
-        paths: "{{ resources_dir }}/pylibs"
-        recurse: no
-        file_type: file
-        use_regex: yes
-        patterns: ".*torch_npu.*{{ ansible_architecture }}.whl"
-      register: torch_npu_whl
-      when: import_torch.rc != 0
-
-    - name: find apex whl package
-      find:
-        paths: "{{ resources_dir }}/pylibs"
-        recurse: no
-        file_type: file
-        use_regex: yes
-        patterns: ".*apex.*{{ ansible_architecture }}.whl"
-      register: apex_whl
-      when: import_torch.rc != 0
-
-    - name: install pytorch if not import
-      include_tasks: task_pytorch.yml
-      when:
-        - import_torch.rc != 0
-        - pytorch_whl.matched > 0
-        - torch_npu_whl.matched > 0
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]can not find torch or torch_npu whl package"
-          - "[ASCEND]please put the files in the directory: ascend_deployer/resources/pylibs/"
-      when:
-        - import_torch.rc != 0
-        - pytorch_whl.matched == 0 or torch_npu_whl.matched == 0
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]can not find apex whl package"
-          - "[ASCEND]please put the files in the directory: ascend_deployer/resources/pylibs/"
-      when:
-        - import_torch.rc != 0 and apex_whl.matched == 0
```

## ascend_deployer/playbooks/install/install_resilience-controller.yml

```diff
@@ -1,5 +1,67 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for resilience-controller
+  tasks:
+    - name: build resilience-controller image
+      install_resilience_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch resilience-controller image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resilience_controller_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/resilience-controller"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push resilience-controller image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "resilience-controller"
+      when: use_harbor
+
+- hosts:
     - master
-  become: yes
+  name: install or upgrade resilience-controller
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/resilience-controller.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/resilience-controller/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/resilience-controller/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install resilience-controller
+      install_resilience_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply resilience-controller
+      throttle: 1
+      install_resilience_controller:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ resilience_controller_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/install_sys_pkg.yml

```diff
@@ -1,17 +1,36 @@
 - hosts: '{{ hosts_name }}'
+  name: install system dependencies for ascend packages
   tasks:
+    - name: check nexus status
+      check_nexus_status:
+        os_and_arch: "{{os_and_arch}}"
+      delegate_to: localhost
+      register: nexus_status
+      failed_when: nexus_status.rc != 0
+      when: ansible_ssh_user == 'root'
+
+    - name: copy file to host
+      copy:
+        src: "{{item.src}}"
+        dest: "{{item.dest}}"
+        force: yes
+        mode: 0644
+      when:
+        - "'gpg' not in item.dest or 'Ubuntu' in os_and_arch"
+        - ansible_ssh_user == 'root'
+      loop:
+        - { src: "{{inventory_dir}}/scripts/nexus_config.json", dest: "~/nexus/" }
+        - { src: "{{inventory_dir}}/downloader/config/{{os_and_arch}}/pkg_info.json", dest: "~/nexus/" }
+        - { src: "{{inventory_dir}}/resources/nexus/nexus_pub.asc", dest: "/etc/apt/trusted.gpg.d/" }
+
     - name: install system packages
-      import_tasks: task_sys_pkg.yml
-      when: ansible_user_uid == 0
+      install_sys_pkg:
+        nexus_url: "{{nexus_url|default('')}}"
+        ansible_run_tags: "{{ansible_run_tags}}"
+        resources_dir: "{{resource_path}}"
+      register: sys_pkg_result
+      failed_when: sys_pkg_result.rc != 0
 
     - name: message
       debug:
-        msg:
-        - "[ASCEND]not support installing sys_pkg by non-root user, please switch to root user"
-      when: ansible_user_uid != 0
-
-    - name: fail if not root
-      fail:
-        msg: "[ASCEND]can not install with non-root"
-      when: "'sys_pkg' in ansible_run_tags and ansible_user_uid != 0"
-
+        var: sys_pkg_result.stdout_lines
```

## ascend_deployer/playbooks/install/install_tensorflow.yml

```diff
@@ -1,98 +1,9 @@
 - hosts: '{{ hosts_name }}'
+  name: install tensorflow
   tasks:
-    - name: try import tensorflow
-      shell: python3 -c "import tensorflow as tf; print(tf.__version__)"
-      environment:
-        PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
-        LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ ascend_install_path }}/ascend-toolkit/latest/fwkacllib/lib64:{{ local_path }}/gcc7.3.0/lib64"
-      failed_when: false
-      changed_when: false
-      register: import_tensorflow
-
-    - name: message
-      debug: var=import_tensorflow
-      when: import_tensorflow.rc == 0
-
-    - name: message
-      debug:
-        msg:
-          - "tensorflow is already installed, tensorflow install skipped"
-      when: import_tensorflow.rc == 0
-
-    - name: stat gcc-7.3.0
-      stat:
-        path: "{{ local_path }}/gcc7.3.0"
-      register: gcc_stat
-      when: import_tensorflow.rc != 0
-
-    - name: install gcc 7.3 for centos 7.6 if not exist
-      import_tasks: task_gcc.yml
-      when:
-        - import_tensorflow.rc != 0
-        - not gcc_stat.stat.exists
-        - "'CentOS_7.6' in os_and_arch"
-
-    - name: find tensorflow 1.15.0 whl package
-      find:
-        paths: "{{ resources_dir }}/pylibs"
-        recurse: no
-        file_type: file
-        use_regex: yes
-        patterns: ".*tensorflow.*1.15.0.*{{ ansible_architecture }}.whl"
-      register: tf1_whl
-      when:
-        - import_tensorflow.rc != 0
-
-    - name: install tensorflow 1.15.0
-      include_tasks: task_tensorflow.yml
-      vars:
-        tensorflow_version: "1.15.0"
-      when:
-        - import_tensorflow.rc != 0
-        - tf1_whl.matched is defined and tf1_whl.matched > 0
-        - python_minor == "python3.7"
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]can not find tensorflow 1.15.0 whl package or python not compatible, install skipped"
-          - "please put the file in the directory: ascend-deployer/resources/pylibs/"
-      when:
-        - import_tensorflow.rc != 0
-        - (tf1_whl.matched is defined and tf1_whl.matched == 0) or python_minor != "python3.7"
-
-    - name: find tensorflow 2.6.5 whl package
-      find:
-        paths: "{{ resources_dir }}/pylibs"
-        recurse: no
-        file_type: file
-        use_regex: yes
-        patterns: ".*tensorflow.*2.6.5.*{{ ansible_architecture }}.whl"
-      register: tf2_whl
-      when:
-        - import_tensorflow.rc != 0
-
-    - name: install tensorflow 2.6.5
-      include_tasks: task_tensorflow.yml
-      vars:
-        tensorflow_version: "2.6.5"
-      when:
-        - import_tensorflow.rc != 0
-        - tf2_whl.matched is defined and tf2_whl.matched > 0
-
-    - name: message
-      debug:
-        msg:
-          - "[ASCEND]can not find tensorflow 2.6.5 whl package, install skipped"
-          - "please put the file in the directory: ascend-deployer/resources/pylibs/"
-      when:
-        - import_tensorflow.rc != 0
-        - tf2_whl.matched is defined and tf2_whl.matched == 0
-
-    - name: fail if exactly at this install
-      fail:
-        msg: "[ASCEND]failed to install tensorflow"
-      when:
-        - "'tensorflow' in ansible_run_tags"
-        - import_tensorflow.rc != 0
-        - (tf2_whl.matched is defined and tf2_whl.matched == 0) and (tf1_whl.matched is defined and tf1_whl.matched == 0)
+    - name: install tensorflow
+      process_framework:
+        resource_dir: "{{resource_path}}"
+        pkg_name: "tensorflow"
+        python_version: "{{python_version}}"
+        ansible_run_tags: "{{ansible_run_tags}}"
```

## ascend_deployer/playbooks/install/install_tfplugin.yml

```diff
@@ -1,4 +1,17 @@
 - hosts: '{{ hosts_name }}'
+  name: install tfplugin
   tasks:
     - name: install tfplugin
-      import_tasks: task_tfplugin.yml
+      install_cann:
+        pkg_name: "tfplugin"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+      register: tfplugin_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: tfplugin_result
+      failed_when: tfplugin_result.rc != 0
```

## ascend_deployer/playbooks/install/install_toolbox.yml

```diff
@@ -1,4 +1,17 @@
 - hosts: '{{ hosts_name }}'
+  name: install toolbox
   tasks:
     - name: install toolbox
-      import_tasks: task_toolbox.yml
+      install_cann:
+        pkg_name: "toolbox"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+      register: toolbox_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: toolbox_result
+      failed_when: toolbox_result.rc != 0
```

## ascend_deployer/playbooks/install/install_toolkit.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: install toolkit
   tasks:
     - name: install toolkit
-      import_tasks: task_toolkit.yml
+      install_cann:
+        pkg_name: "toolkit"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        is_ipv6: "{{working_on_ipv6}}"
+      register: toolkit_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: toolkit_result
+      failed_when: toolkit_result.rc != 0
```

## ascend_deployer/playbooks/install/install_volcano.yml

```diff
@@ -1,6 +1,68 @@
 - hosts:
+    - master[0]
+    - other_build_image
+  name: build image for volcano
+  tasks:
+    - name: build volcano image
+      install_volcano:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'build'
+
+    - name: fetch volcano image
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ volcano_images }}"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/volcano"
+        fetch: 'true'
+      delegate_to: localhost
+
+- hosts:
+    - localhost
+  name: push volcano image to harbor
+  tasks:
+    - name: push to harbor
+      push_image:
+        harbor_server: "{{ HARBOR_SERVER }}"
+        project_name: "mindx"
+        public: "{{ HARBOR_PUBLIC_PROJECT }}"
+        user: "{{ HARBOR_ADMIN_USER }}"
+        password: "{{ HARBOR_ADMIN_PASSWORD }}"
+        image_dir: "{{ resource_path }}/mindxdl/dlImages/"
+        component_name: "volcano"
+      when: use_harbor
+
+- hosts:
     - master
     - worker
-  become: yes
+  name: install or upgrade volcano
   tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/volcano.yaml
+    - name: push images to remote
+      scp:
+        ip: "{{ inventory_hostname }}"
+        remote_user: "{{ ansible_ssh_user }}"
+        passwd: "{{ ansible_ssh_pass|default('') }}"
+        src: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/volcano/*"
+        dest: "{{ resource_path }}/mindxdl/dlImages/{{ ansible_architecture }}/volcano/"
+      delegate_to: localhost
+      when: not use_harbor
+
+    - name: install volcano
+      install_volcano:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'install'
+
+    - name: apply volcano
+      throttle: 1
+      install_volcano:
+        resources_dir: "{{ resource_path }}"
+        harbor_server: "{{ HARBOR_SERVER }}"
+        step: 'apply'
+        node_name: "{{ NODE_NAME }}"
+        master_node: "{{ inventory_hostname in groups['master'] }}"
+        worker_node: "{{ inventory_hostname in groups['worker'] }}"
+        labels: "{{ volcano_labels }}"
+      delegate_to: "{{ groups['master'][0] }}"
```

## ascend_deployer/playbooks/install/task_atlasedge.yml

```diff
@@ -5,15 +5,15 @@
 - name: find atlasedge path
   find:
     paths: "{{ resources_dir }}/run_from_cann_zip"
     recurse: no
     file_type: directory
     use_regex: yes
     patterns: ".*atlasedge.*{{ansible_architecture}}"
-  when: (ansible_local.npu_info.scene == 'infer' or ansible_local.npu_info.scene == 'a300i') and a500pro_exist.stdout != ""
+  when: (npu_info.scene == 'infer' or npu_info.scene == 'a300i') and a500pro_exist.stdout != ""
   register: atlasedge
 
 - name: install atlasedge
   shell: "bash {{ atlasedge.files[0].path }}/install.sh --install_dir=/usr/local/"
   register: atlasedge_result
   when: atlasedge.matched is defined and atlasedge.matched > 0
   failed_when: "atlasedge_result.rc !=0 and 'has been installed' not in atlasedge_result.stdout"
@@ -29,12 +29,15 @@
     msg:
       - "[ASCEND]can not find atlasedge package, atlasedge install skipped"
   when: atlasedge.matched is defined and atlasedge.matched == 0
 
 - name: fail if this install
   fail:
     msg: "[ASCEND]failed to install atlasedge"
-  when: "'atlasedge' in ansible_run_tags and atlasedge_result.rc !=0 and 'has been installed' not in atlasedge_result.stdout"
+  when:
+    - atlasedge in ansible_run_tags
+    - atlasedge.matched is defined and atlasedge.matched > 0
+    - atlasedge_result.rc !=0 and 'has been installed' not in atlasedge_result.stdout
 
 - name: atlasedge install message
   debug: var=atlasedge_result
   when: atlasedge_result.changed is defined and atlasedge_result.changed
```

## ascend_deployer/playbooks/install/task_dl.yml

```diff
@@ -1,47 +1,7 @@
-- name: gather fact info for dl
-  import_playbook: ../gather_facts.yaml
-
-- name: install basic packages
-  import_playbook: ../basic.yaml
-
 - name: basic check
   import_playbook: ../check.yaml
 
-- name: check docker, containerd and nerdctl
-  import_playbook: ../docker.yaml
-
 - name: config harbor info
   import_playbook: ../harbor.yaml
   when:
     - use_harbor
-
-- hosts:
-    - master
-    - worker
-  gather_facts: false
-  become: yes
-  tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/dl_common.yaml
-
-- hosts:
-    - localhost
-    - master[0]
-    - other_build_image
-  become: yes
-  tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/distribute_soft_package.yaml
-    - include_tasks: ../roles/mindx.dl/tasks/build_collect_images.yaml
-
-- hosts:
-    - master
-  gather_facts: false
-  become: yes
-  tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/label_master.yaml
-
-- hosts:
-    - worker
-  gather_facts: false
-  become: yes
-  tasks:
-    - include_tasks: ../roles/mindx.dl/tasks/label_worker.yaml
```

## ascend_deployer/playbooks/install/task_docker_images.yml

```diff
@@ -1,10 +1,7 @@
-- name: install system packages
-  include_tasks: "task_sys_{{ansible_pkg_mgr}}.yml"
-
 - name: find docker command
   shell: command -v docker | wc -l
   register: docker_exists
 
 - name: restart docker
   shell: "systemctl restart docker"
   when: docker_exists.stdout != '0'
```

## ascend_deployer/playbooks/install/task_ha.yml

```diff
@@ -5,15 +5,15 @@
 - name: find ha path
   find:
     paths: "{{ resources_dir }}/run_from_cann_zip"
     recurse: no
     file_type: directory
     use_regex: yes
     patterns: ".*ha.*{{ansible_architecture}}"
-  when: ansible_local.npu_info.scene == 'infer' and a500pro_exist.stdout != ""
+  when: npu_info.scene == 'infer' and a500pro_exist.stdout != ""
   register: ha
 
 - name: install ha
   shell: "bash {{ ha.files[0].path }}/install.sh -f -p /usr/local/"
   register: ha_result
   when: ha.matched is defined and ha.matched > 0
   failed_when: "ha_result.rc !=0 and 'has been installed' not in ha_result.stdout"
@@ -29,12 +29,16 @@
     msg:
       - "[ASCEND]can not find ha package, ha install skipped"
   when: ha.matched is defined and ha.matched == 0
 
 - name: fail if not success
   fail:
     msg: "[ASCEND]failed to install ha"
-  when: "ha_result.rc !=0 or 'has been installed' not in ha_result.stdout and 'ha' in ansible_run_tags"
+  when:
+    - ha.matched is defined and ha.matched > 0
+    - ha_result.rc !=0 or 'has been installed' not in ha_result.stdout and 'ha' in ansible_run_tags
 
 - name: ha install message
   debug: var=ha_result
-  when: ha_result.changed is defined and ha_result.changed
+  when:
+    - ha.matched is defined and ha.matched > 0
+    - ha_result.changed is defined and ha_result.changed
```

## ascend_deployer/playbooks/install/patch/install_nnae.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: install nnae patch
   tasks:
     - name: install nnae patch
-      import_tasks: task_nnae.yml
+      install_cann:
+        pkg_name: "nnae"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "patch"
+      register: nnae_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnae_result
+      failed_when: nnae_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/install_nnrt.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: install nnrt patch
   tasks:
     - name: install nnrt patch
-      import_tasks: task_nnrt.yml
+      install_cann:
+        pkg_name: "nnrt"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "patch"
+      register: nnrt_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnrt_result
+      failed_when: nnrt_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/install_tfplugin.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: install tfplugin patch
   tasks:
     - name: install tfplugin patch
-      import_tasks: task_tfplugin.yml
+      install_cann:
+        pkg_name: "tfplugin"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "patch"
+      register: tfplugin_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: tfplugin_result
+      failed_when: tfplugin_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/install_toolkit.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: install toolkit patch
   tasks:
     - name: install toolkit patch
-      import_tasks: task_toolkit.yml
+      install_cann:
+        pkg_name: "toolkit"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "patch"
+      register: toolkit_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: toolkit_result
+      failed_when: toolkit_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/rollback_nnae.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: rollback nnae
   tasks:
     - name: rollback nnae
-      import_tasks: task_rollback_nnae.yml
+      install_cann:
+        pkg_name: "nnae"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "rollback"
+      register: nnae_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnae_result
+      failed_when: nnae_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/rollback_nnrt.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: rollback nnrt
   tasks:
     - name: rollback nnrt
-      import_tasks: task_rollback_nnrt.yml
+      install_cann:
+        pkg_name: "nnrt"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "rollback"
+      register: nnrt_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: nnrt_result
+      failed_when: nnrt_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: rollback tfplugin
   tasks:
     - name: rollback tfplugin
-      import_tasks: task_rollback_tfplugin.yml
+      install_cann:
+        pkg_name: "tfplugin"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "rollback"
+      register: tfplugin_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: tfplugin_result
+      failed_when: tfplugin_result.rc != 0
```

## ascend_deployer/playbooks/install/patch/rollback_toolkit.yml

```diff
@@ -1,4 +1,18 @@
 - hosts: '{{ hosts_name }}'
+  name: rollback toolkit
   tasks:
     - name: rollback toolkit
-      import_tasks: task_rollback_toolkit.yml
+      install_cann:
+        pkg_name: "toolkit"
+        run_tags: "{{ansible_run_tags}}"
+        python_version: "{{python_version}}"
+        resources_dir: "{{resource_path}}"
+        npu_info: "{{npu_info}}"
+        action: "rollback"
+      register: toolkit_result
+      failed_when: false
+
+    - name: message
+      debug:
+        var: toolkit_result
+      failed_when: toolkit_result.rc != 0
```

## ascend_deployer/playbooks/process/process_check.yml

```diff
@@ -1,12 +1,6 @@
-- name: gather fact info
-  import_playbook: ../gather_npu_fact.yml
-  tags: always
-
 - hosts: all
-  vars:
-    script_path: "{{ playbook_dir }}/../../tools/check.py"
-    fact_path_dir: "{{ playbook_dir }}/../../facts_cache"
-    check_tags: "{{ ansible_run_tags | join(',') }}"
+  tags: always
   tasks:
-    - include_tasks: ../roles/mindx.check/tasks/compatibility_check.yml
-  tags: always
+    - name: check compatibility
+      check_compatibility:
+        tags: "{{ ansible_run_tags }}"
```

## ascend_deployer/playbooks/process/process_install.yml

```diff
@@ -1,76 +1,35 @@
 - name: gather fact info
   import_playbook: ../gather_npu_fact.yml
   tags: always
 
-- name: create nexus
-  import_playbook: ../create_nexus.yml
-  tags:
-    - sys_pkg
-
-- name: check packages for run and zip
-  import_playbook: ../check_pkgs.yml
-  tags:
-    - atlasedge
-    - docker_images
-    - driver
-    - firmware
-    - gcc
-    - ha
-    - ief
-    - kernels
-    - mindspore
-    - mindstudio
-    - nnae
-    - nnrt
-    - npu
-    - python
-    - pytorch
-    - sys_pkg
-    - tensorflow
-    - tfplugin
-    - toolbox
-    - toolkit
-
 - name: copy resources to remote servers
   import_playbook: ../distribution.yml
   tags: copy
 
 - name: install sys pkg
   import_playbook: ../install/install_sys_pkg.yml
   tags: sys_pkg
 
 - name: install python
   import_playbook: ../install/install_python.yml
   tags: python
 
 - name: install npu
   import_playbook: ../install/install_npu.yml
-  tags: npu
-
-- name: install firmware
-  import_playbook: ../install/install_firmware.yml
-  tags: firmware
-
-- name: install driver
-  import_playbook: ../install/install_driver.yml
-  tags: driver
+  tags: driver,firmware,npu
 
 - name: install atlasedge
   import_playbook: ../install/install_atlasedge.yml
   tags: atlasedge
 
 - name: install docker images
   import_playbook: ../install/install_docker_images.yml
   tags: docker_images
 
-- name: install gcc
-  import_playbook: ../install/install_gcc.yml
-  tags: gcc
-
 - name: install ha
   import_playbook: ../install/install_ha.yml
   tags: ha
 
 - name: install ief
   import_playbook: ../install/install_ief.yml
   tags: ief
@@ -158,14 +117,10 @@
   import_playbook: ../install/install_ascend-docker-runtime.yml
   tags: ascend-docker-runtime
 
 - name: install mindio
   import_playbook: ../install/install_mindio.yml
   tags: mindio
 
-- name: clean nexus
-  import_playbook: ../clean_nexus.yml
-  tags: sys_pkg
-
 - name: generate report
   import_playbook: ../report.yaml
   tags: always
```

## ascend_deployer/playbooks/process/process_patch.yml

```diff
@@ -1,19 +1,11 @@
 - name: gather fact info
   import_playbook: ../gather_npu_fact.yml
   tags: always
 
-- name: check packages for run and zip
-  import_playbook: ../check_pkgs.yml
-  tags:
-    - nnae
-    - nnrt
-    - tfplguin
-    - toolkit
-
 - name: copy resources to remote servers
   import_playbook: ../distribution.yml
   tags: copy
 
 - name: install patch nnae
   import_playbook: ../install/patch/install_nnae.yml
   tags: nnae
```

## ascend_deployer/playbooks/process/process_patch_rollback.yml

```diff
@@ -1,19 +1,11 @@
 - name: gather fact info
   import_playbook: ../gather_npu_fact.yml
   tags: always
 
-- name: check packages for run and zip
-  import_playbook: ../check_pkgs.yml
-  tags:
-    - nnae
-    - nnrt
-    - tfplguin
-    - toolkit
-
 - name: copy resources to remote servers
   import_playbook: ../distribution.yml
   tags: copy
 
 - name: install patch nnae
   import_playbook: ../install/patch/rollback_nnae.yml
   tags: nnae
```

## ascend_deployer/playbooks/process/process_scene.yml

```diff
@@ -1,41 +1,11 @@
 - name: gather fact info
   import_playbook: ../gather_npu_fact.yml
   tags: always
 
-- name: create nexus
-  import_playbook: ../create_nexus.yml
-  tags:
-    - auto
-    - edge
-    - mindspore
-    - offline_dev
-    - offline_run
-    - pytorch_dev
-    - pytorch_run
-    - tensorflow_dev
-    - tensorflow_run
-    - vmhost
-    - dl
-
-- name: check packages for run and zip
-  import_playbook: ../check_pkgs.yml
-  tags:
-    - auto
-    - edge
-    - mindspore
-    - offline_dev
-    - offline_run
-    - pytorch_dev
-    - pytorch_run
-    - tensorflow_dev
-    - tensorflow_run
-    - vmhost
-    - dl
-
 - name: copy resources to remote servers
   import_playbook: ../distribution.yml
   tags: copy
 
 - name: install scene auto
   import_playbook: ../scene/scene_auto.yml
   tags: auto
@@ -80,25 +50,10 @@
   import_playbook: ../scene/scene_dl.yml
   tags: dl
 
 - name: install mef
   import_playbook: ../scene/scene_mef.yml
   tags: mef
 
-- name: clean nexus
-  import_playbook: ../clean_nexus.yml
-  tags:
-    - auto
-    - edge
-    - mindspore
-    - offline_dev
-    - offline_run
-    - pytorch_dev
-    - pytorch_run
-    - tensorflow_dev
-    - tensorflow_run
-    - vmhost
-    - dl
-
 - name: generate report
   import_playbook: ../report.yaml
   tags: always
```

## ascend_deployer/playbooks/process/process_test.yml

```diff
@@ -1,51 +1,9 @@
-- name: gather fact info
-  import_playbook: ../gather_npu_fact.yml
-  tags: always
-
-- name: test all
-  import_playbook: ../test/test_all.yml
-  tags: whole
-
-- name: test driver
-  import_playbook: ../test/test_driver.yml
-  tags: driver
-
-- name: test firmware
-  import_playbook: ../test/test_firmware.yml
-  tags: firmware
-
-- name: test mindspore
-  import_playbook: ../test/test_mindspore.yml
-  tags: mindspore
-
-- name: nnae
-  import_playbook: ../test/test_nnae.yml
-  tags: nnae
-
-- name: test nnrt
-  import_playbook: ../test/test_nnrt.yml
-  tags: nnrt
-
-- name: test pytorch
-  import_playbook: ../test/test_pytorch.yml
-  tags: pytorch
-
-- name: test tensorflow
-  import_playbook: ../test/test_tensorflow.yml
-  tags: tensorflow
-
-- name: test tfplugin
-  import_playbook: ../test/test_tfplugin.yml
-  tags: tfplugin
-
-- name: test toolbox
-  import_playbook: ../test/test_toolbox.yml
-  tags: toolbox
-
-- name: test toolkit
-  import_playbook: ../test/test_toolkit.yml
-  tags: toolkit
-
-- name: show result
-  import_playbook: ../test/test_exhibit.yml
+- hosts:
+    - worker
+  tasks:
+    - name: do test
+      process_test:
+        ansible_run_tags: "{{ ansible_run_tags }}"
+        cus_npu_info: "{{ cus_npu_info | default('') }}"
+        python_version: "{{ python_version | default('python3.7.5')}}"
   tags: always
```

## ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml

```diff
@@ -1,12 +1,12 @@
 # 使用dpkg作为包管理器
 - name: install docker-ce
-  shell: dpkg --force-all -i {{ docker_pkg_dir }}/{{ ansible_architecture }}/*.deb
+  shell: "dpkg --force-all -i {{ docker_pkg_dir }}/{{ ansible_architecture }}/*.deb"
   environment:
     DEBIAN_FRONTEND: noninteractive
     DEBIAN_PRIORITY: critical
   when: not use_rpm_command
 
 # 使用rpm作为包管理器
 - name: install docker-ce
-  shell: rpm -iUv {{ docker_pkg_dir }}/{{ ansible_architecture }}/*.rpm --nodeps --force
+  shell: "rpm -iUv {{ docker_pkg_dir }}/{{ ansible_architecture }}/*.rpm --nodeps --force"
   when: use_rpm_command
```

## ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml

```diff
@@ -1,14 +1,40 @@
 # 使用dpkg作为包管理器
 - name: install containerd
-  shell: dpkg --force-all -i {{ docker_pkg_dir }}/{{ ansible_architecture }}/containerd.io*.deb
+  shell: "dpkg --force-all -i {{ docker_pkg_dir }}/{{ ansible_architecture }}/containerd.io*.deb"
   throttle: 1
   environment:
     DEBIAN_FRONTEND: noninteractive
     DEBIAN_PRIORITY: critical
-  when: not use_rpm_command
+  when: not use_rpm_command and not skip_sys_pkg
 
 # 使用rpm作为包管理器
 - name: install containerd
-  shell: rpm -iUv {{ docker_pkg_dir }}/{{ ansible_architecture }}/containerd.io*.rpm --nodeps --force
+  shell: "rpm -iUv {{ docker_pkg_dir }}/{{ ansible_architecture }}/containerd.io*.rpm --nodeps --force"
   throttle: 1
-  when: use_rpm_command
+  when: use_rpm_command and not skip_sys_pkg
+
+- name: generate config for containerd
+  shell: containerd config default > /etc/containerd/config.toml
+  register: config_result
+
+- name: change config
+  shell:
+    cmd:
+      sed -i "s#registry.k8s.io/pause:3.6#registry.k8s.io/pause:3.8#g" /etc/containerd/config.toml;
+      sed -i "s#SystemdCgroup = false#SystemdCgroup = true#g" /etc/containerd/config.toml;
+  register: fix_result
+
+
+- name: add harbor config
+  shell:
+    cmd:
+      sed -i "s#registry.k8s.io/pause:3.8#{{ HARBOR_SERVER }}/registry.k8s.io/pause:3.8#g" /etc/containerd/config.toml;
+  when: use_harbor
+
+
+- name: restart containerd
+  systemd:
+    daemon_reload: yes
+    name: "containerd"
+    enabled: true
+    state: restarted
```

## ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml

```diff
@@ -18,26 +18,32 @@
 
 - name: message
   debug:
     msg: "docker is running already. The script won't install docker."
   when: docker_installed
   changed_when: false
 
+- name: failed when skip sys_pkg but docker not ok
+  fail:
+    msg: "docker is not ok and we can not install sys_pkg under this OS!"
+  when: not docker_installed and skip_sys_pkg
+
 - name: message
   debug:
     msg: "*************************start install docker***************************"
   when: not docker_installed
 
 - name: message
   debug:
     msg: "containerd need reinstall, the script will install containerd."
-  when: not use_old_k8s_version
+  when: not use_old_k8s_version and not skip_sys_pkg
 
 - name: message
   debug:
     msg: "************************start install containerd**********************"
-  when: not use_old_k8s_version
+  when: not use_old_k8s_version and not skip_sys_pkg
 
 - name: include copy task
   include_tasks: copy.yml
+  when: not skip_sys_pkg
```

## ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml

```diff
@@ -1,32 +1,7 @@
-- name: find npu-smi command
-  shell: command -v npu-smi
-  register: npu_smi_exists
-  failed_when: false
-
-- name: find hccn_tool command
-  shell: command -v hccn_tool
-  register: hccn_tool_exists
-  failed_when: false
-
-- name: copy hccn.py to remote hosts
-  copy:
-    src: "{{ playbook_dir }}/../tools/hccn.py"
-    dest: "{{ ansible_env.HOME}}/"
-    mode: 0700
-    force: yes
-
 - name: hccn_tool configures IP address
-  shell: "{{ discovered_interpreter_python }}  {{ ansible_env.HOME }}/hccn.py '{{ deviceip }}-{{ detectip }}-{{ gateways }}-{{ netmask }}-{{ roce_port }}-{{ bitmap }}-{{ dscp_tc }}-{{ common_network }}'"
-  register: hccn_result
+  script:
+    cmd: ../../../../tools/hccn.py '{{ deviceip }}-{{ detectip }}-{{ gateways }}-{{ netmask }}-{{ roce_port }}-{{ bitmap }}-{{ dscp_tc }}-{{ common_network }}'
+  args:
+    executable: "{{ discovered_interpreter_python }}"
   environment:
-    LD_LIBRARY_PATH: "/usr/local/Ascend/nnrt/latest/lib64:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:/usr/local/Ascend/nnae/latest/lib64:/usr/local/Ascend/nnae/latest/lib64/plugin/opskernel:/usr/local/Ascend/nnae/latest/lib64/plugin/nnengine:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:/usr/local/Ascend/ascend-toolkit/latest/lib64:/usr/local/Ascend/ascend-toolkit/latest/lib64/plugin/opskernel:/usr/local/Ascend/ascend-toolkit/latest/lib64/plugin/nnengine:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:"
-
-- name: print lossing parts
-  debug:
-    msg: "[ASCEND][WARNING]: Can not find npu-smi, maybe driver not installed, or env not right"
-  when: npu_smi_exists.rc != 0
-
-- debug:
-    msg: "[ASCEND][WARNING]: Can not find hccn_tool, maybe driver not installed or supported, or env not right"
-  when: hccn_result.rc != 0 or hccn_tool_exists.rc != 0
-  name: print lossing parts
+    LD_LIBRARY_PATH: "/usr/local/Ascend/nnrt/latest/lib64:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:/usr/local/Ascend/nnae/latest/lib64:/usr/local/Ascend/nnae/latest/lib64/plugin/opskernel:/usr/local/Ascend/nnae/latest/lib64/plugin/nnengine:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:/usr/local/Ascend/ascend-toolkit/latest/lib64:/usr/local/Ascend/ascend-toolkit/latest/lib64/plugin/opskernel:/usr/local/Ascend/ascend-toolkit/latest/lib64/plugin/nnengine:/usr/local/Ascend/driver/lib64:/usr/local/Ascend/driver/lib64/common:/usr/local/Ascend/driver/lib64/driver:"
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml

```diff
@@ -3,14 +3,20 @@
   file:
     path: "{{ k8s_image_dir }}"
     state: directory
     mode: 0750
   when:
     - no_copy_flag != "true"
 
+- name: clean image dir
+  file:
+    path: "{{ k8s_image_dir }}/{{ ansible_architecture }}"
+    state: absent
+
+
 # 复制k8s镜像包到远端并解压
 - name: unarchive k8s base images on remote for k8s 1.19.16
   ansible.builtin.unarchive:
     src: "{{ k8s_image_dir }}/{{ ansible_architecture }}.tar.gz"
     dest: "{{ k8s_image_dir }}"
     remote_src: no
   when:
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml

```diff
@@ -2,14 +2,19 @@
   file:
     path: "{{ k8s_pkg_dir }}"
     state: directory
     mode: 0750
   when:
     - no_copy_flag != "true"
 
+- name: clean image dir
+  file:
+    path: "{{ k8s_pkg_dir }}/{{ ansible_architecture }}"
+    state: absent
+
 # 复制k8s软件包到远端并解压
 - name: unarchive k8s software on remote for 1.19.16
   ansible.builtin.unarchive:
     src: "{{ k8s_pkg_dir }}/{{ ansible_architecture }}.tar.gz"
     dest: "{{ k8s_pkg_dir }}"
     mode: 0750
     remote_src: no
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml

```diff
@@ -1,33 +1,32 @@
 # 使用dpkg作为包管理器
 - name: install k8s
-  shell: dpkg --force-all -i {{ k8s_pkg_dir }}/{{ ansible_architecture }}/*.deb
+  shell: "dpkg --force-all -i {{ k8s_pkg_dir }}/{{ ansible_architecture }}/*.deb"
   environment:
     DEBIAN_FRONTEND: noninteractive
     DEBIAN_PRIORITY: critical
-  when: not use_rpm_command
+  when: not use_rpm_command and not skip_sys_pkg
 
 # 使用rpm作为包管理器
 - name: install k8s
-  shell: rpm -iUv {{ k8s_pkg_dir }}/{{ ansible_architecture }}/*.rpm --nodeps --force
-  when: use_rpm_command
+  shell: "rpm -iUv {{ k8s_pkg_dir }}/{{ ansible_architecture }}/*.rpm --nodeps --force"
+  when: use_rpm_command and not skip_sys_pkg
 
 - name: modify kubeadm.conf file
-  shell: |
-    cat {{ KUBEADM_CONFIG_FILE }} | grep 'cgroup-driver' || sed -i 's/KUBELET_KUBECONFIG_ARGS=/KUBELET_KUBECONFIG_ARGS=--cgroup-driver=systemd /' {{ KUBEADM_CONFIG_FILE }}
+  shell: "cat {{ KUBEADM_CONFIG_FILE }} | grep 'cgroup-driver' || sed -i 's/KUBELET_KUBECONFIG_ARGS=/KUBELET_KUBECONFIG_ARGS=--cgroup-driver=systemd /' {{ KUBEADM_CONFIG_FILE }}"
   when:
     - os_name|lower == 'ubuntu'
 
 - name: create /etc/default/kubelet
   shell: echo 'KUBELET_EXTRA_ARGS=--node-ip=::' > /etc/default/kubelet && chmod 644 /etc/default/kubelet
-  when: working_on_ipv6 and not use_rpm_command
+  when: working_on_ipv6=="true" and not use_rpm_command
 
 - name: create /etc/sysconfig/kubelet
   shell: echo 'KUBELET_EXTRA_ARGS=--node-ip=::' > /etc/sysconfig/kubelet && chmod 644 /etc/sysconfig/kubelet
-  when: working_on_ipv6 and use_rpm_command
+  when: working_on_ipv6=="true" and use_rpm_command
 
 - name: enable kubelet
   systemd:
     name: "kubelet"
     enabled: true
     state: started
     daemon_reload: yes
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml

```diff
@@ -14,21 +14,15 @@
     - not k8s_installed
 
 - name: include copy software task
   include_tasks: copy_software.yml
   when:
     - in_k8s_group
     - not k8s_installed
-
-- name: init containerd
-  include_tasks: containerd.yml
-  when: 
-    - in_k8s_group
-    - not k8s_initialized
-    - not use_old_k8s_version
+    - not skip_sys_pkg
 
 # 复制离线镜像到各节点
 - name: include copy image task
   include_tasks: copy_image.yml
   when:
     - in_k8s_group
     - not k8s_initialized
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml

```diff
@@ -64,16 +64,16 @@
   when:
     - "'/' in item.stdout "
 
 - name: clean old manifest
   shell:
     cmd:
       manifest_name="{{ HARBOR_SERVER }}/{{ item.stdout.replace('_'+master_arch+':', ':') }}";
-      chmod 755 {{ docker_20_bin_dir }}/docker-{{ ansible_architecture }};
-      {{ docker_20_bin_dir }}/docker-{{ ansible_architecture }} manifest rm "${manifest_name}" > /dev/null 2>&1 || true
+      chmod 755 "{{ docker_20_bin_dir }}/docker-{{ ansible_architecture }}";
+      "{{ docker_20_bin_dir }}/docker-{{ ansible_architecture }}" manifest rm "${manifest_name}" > /dev/null 2>&1 || true
   loop: "{{ k8s_base_images['results'] }}"
   environment:
     DOCKER_CLI_EXPERIMENTAL: enabled
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
@@ -84,16 +84,16 @@
 # 开启实验特性再使用manifest
 # 先将原始镜像推送到harbor，再创建manifest
 # item.stdout格式 xxxxx_架构:tag
 # 一定要用annotate，不然推送导入的arm镜像在x86服务器上会被标记为x86架构
 - name: create manifest master node arch
   shell:
     cmd:
-      manifest_name="{{ HARBOR_SERVER }}/{{ item.stdout.replace('_'+master_arch+':', ':') }}";
-      master_image="{{ HARBOR_SERVER }}/{{ item.stdout }}";
+      manifest_name={{ HARBOR_SERVER }}/{{ item.stdout.replace('_'+master_arch+':', ':') }};
+      master_image={{ HARBOR_SERVER }}/{{ item.stdout }};
       docker push "${master_image}";
       docker manifest create --insecure "${manifest_name}"  --amend "${master_image}";
       docker manifest annotate --arch "{{ 'arm64' if master_arch == 'aarch64' else 'amd64' }}" "${manifest_name}" "${master_image}";
   loop: "{{ k8s_base_images['results'] }}"
   environment:
     DOCKER_CLI_EXPERIMENTAL: enabled
     http_proxy: ""
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml

```diff
@@ -30,15 +30,15 @@
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when:
     - use_harbor
 
 - name: generate kube-vip.yaml
   shell: |
-    nerdctl run --network host --namespace k8s.io --rm {{ HARBOR_SERVER+'/' if use_harbor else '' }}{{ KUBE_VIP_IMAGE }}:{{ KVVERSION }} manifest pod \
+    nerdctl run --network host --namespace k8s.io --rm "{{ HARBOR_SERVER+'/' if use_harbor else '' }}{{ KUBE_VIP_IMAGE }}:{{ KVVERSION }}" manifest pod \
     --interface {{ kube_interface }} \
     --address {{ KUBE_VIP }} \
     --controlplane \
     --services \
     --enableLoadBalancer \
     --arp \
     --leaderElection | tee /etc/kubernetes/manifests/kube-vip.yaml
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml

```diff
@@ -102,25 +102,29 @@
   when: not use_old_k8s_version
 
 - name: set calico_325 yaml on ipv6
   template:
     src: "../../templates/calico_{{calico_version_3_25}}.ipv6.yaml"
     dest: "{{ CALICO_YAML_DIR }}/calico_{{calico_version_3_25}}.yaml"
     mode: 0640
-  when: not use_old_k8s_version and working_on_ipv6
+  when: not use_old_k8s_version and working_on_ipv6=="true"
 
 - name: apply 3.20 calico
   shell: "kubectl apply -f {{ CALICO_YAML_DIR }}/calico_{{calico_version_3_20}}.yaml"
   environment:
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when: use_old_k8s_version
 
+- name: change image to harbor for calico on 3.25
+  shell: "sed -i 's#image: docker.io/calico#image: {{ HARBOR_SERVER }}/calico#g' {{ CALICO_YAML_DIR }}/calico_{{ calico_version_3_25 }}.yaml"
+  when: not use_old_k8s_version and use_harbor
+
 - name: apply 3.25 calico
   shell: "kubectl apply -f {{ CALICO_YAML_DIR }}/calico_{{calico_version_3_25}}.yaml"
   environment:
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
```

## ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml

```diff
@@ -52,23 +52,23 @@
     dest: "/root/.kube/config"
     mode: "0640"
     owner: "root"
     group: "root"
     remote_src: yes
 
 - name: taint nodes
-  shell: kubectl taint nodes {{NODE_NAME}} node-role.kubernetes.io/master-
+  shell: "kubectl taint nodes {{NODE_NAME}} node-role.kubernetes.io/master-"
   environment:
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when: use_old_k8s_version
 
 - name: taint nodes
-  shell: kubectl taint nodes {{NODE_NAME}} node-role.kubernetes.io/control-plane-
+  shell: "kubectl taint nodes {{NODE_NAME}} node-role.kubernetes.io/control-plane-"
   environment:
     http_proxy: ""
     https_proxy: ""
     HTTP_PROXY: ""
     HTTPS_PROXY: ""
   when: not use_old_k8s_version
```

## ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml

```diff
@@ -150,12 +150,12 @@
 - name: message
   fail:
     msg: "install kubeedge failed"
   when: cloudcore_status.stdout != 'active'
 
 - name: install MEF
   shell: |
-    unzip -o {{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter*{{ansible_architecture}}.zip -d {{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter &&
-    cd {{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter && mkdir -p Ascend-mindxedge-mefcenter &&
-    tar -C ${PWD}/Ascend-mindxedge-mefcenter -xzvf {{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter/Ascend-mindxedge-mefcenter*{{ansible_architecture}}.tar.gz &&
-    cd  {{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter/Ascend-mindxedge-mefcenter/installer &&
+    unzip -o "{{ansible_env.HOME}}"/resources/mef-pushing/Ascend-mindxedge-mefcenter*"{{ansible_architecture}}.zip" -d "{{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter" &&
+    cd "{{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter" && mkdir -p Ascend-mindxedge-mefcenter &&
+    tar -C "${PWD}/Ascend-mindxedge-mefcenter" -xzvf "{{ansible_env.HOME}}"/resources/mef-pushing/Ascend-mindxedge-mefcenter/Ascend-mindxedge-mefcenter*"{{ansible_architecture}}".tar.gz &&
+    cd  "{{ansible_env.HOME}}/resources/mef-pushing/Ascend-mindxedge-mefcenter/Ascend-mindxedge-mefcenter/installer" &&
     bash install.sh && bash /usr/local/MEF-Center/mef-center/run.sh start all
```

## ascend_deployer/playbooks/scene/scene_dl.yml

```diff
@@ -1,28 +1,48 @@
+- name: check if need bypass system package installation
+  import_playbook: ../gather_installation_facts.yml
+
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
+  when: not skip_sys_pkg
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
-- name: gather fact info for dl
-  import_playbook: ../gather_facts.yaml
-
-- name: install basic packages
-  import_playbook: ../basic.yaml
-
 - name: basic check
   import_playbook: ../check.yaml
 
 - name: install docker
   import_playbook: ../docker.yaml
 
 - name: config harbor info
   import_playbook: ../harbor.yaml
   when:
     - use_harbor
 
 - name: install k8s
   import_playbook: ../k8s.yaml
+  when: not skip_k8s_install
+
+- name: install ascend-docker-runtime
+  import_playbook: ../install/install_ascend-docker-runtime.yml
+
+- name: install volcano
+  import_playbook: ../install/install_volcano.yml
+
+- name: install hccl-controller
+  import_playbook: ../install/install_hccl-controller.yml
+
+- name: install ascend-operator
+  import_playbook: ../install/install_ascend-operator.yml
+
+- name: install resilience-controller
+  import_playbook: ../install/install_resilience-controller.yml
+
+- name: install ascend-device-plugin
+  import_playbook: ../install/install_ascend-device-plugin.yml
+
+- name: install noded
+  import_playbook: ../install/install_noded.yml
 
-- name: install dl
-  import_playbook: ../mindxdl.yaml
+- name: install npu-exporter
+  import_playbook: ../install/install_npu-exporter.yml
```

## ascend_deployer/playbooks/scene/scene_mef.yml

```diff
@@ -1,15 +1,12 @@
-- name: gather fact info for dl
-  import_playbook: ../gather_facts.yaml
-
-- name: install basic packages
-  import_playbook: ../basic.yaml
+- name: install system dependencies
+  import_playbook: ../install/install_sys_pkg.yml
 
 - name: basic check
-  import_playbook: ../check_mef.yaml
+  import_playbook: ../check.yaml
 
 - name: install docker
   import_playbook: ../docker.yaml
 
 - name: install k8s
   import_playbook: ../k8s.yaml
```

## ascend_deployer/scripts/nexus.py

```diff
@@ -13,194 +13,187 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import base64
 import glob
 import json
+import logging
 import os
 import platform
-import re
-import secrets
+import random
 import shlex
 import shutil
 import string
 import subprocess
+import sys
 import time
-from urllib import parse, request
+
+sys.path.append(os.path.dirname(os.path.dirname(__file__)))
+
+from utils import ROOT_PATH
+
+try:
+    from urllib.parse import urljoin
+    from urllib.request import Request, urlopen
+
+    PY3 = True
+except ImportError:
+    from urllib2 import Request, urlopen
+    from urlparse import urljoin
+
+    PY3 = False
+
+LOG = logging.getLogger("ascend_deployer.scripts.nexus")
 
 
 def get_passwd():
-    return "".join(
-        secrets.choice(string.digits + string.ascii_letters)
-        for _ in range(16)
-    )
+    rand = random.SystemRandom()
+    return "".join(rand.choice(string.digits + string.ascii_letters) for _ in range(16))
 
 
 class OsRepository:
     NEXUS_USER = "admin"
-    NEXUS_RUN_PORT = 58081
     nexus_passwd = get_passwd()
     gpg_passwd = get_passwd()
 
-    def __init__(self):
+    def __init__(self, ip=None, port=58081):
         try:
-            self.nexus_run_ip = os.environ["SSH_CONNECTION"].split()[2]
+            self.nexus_run_ip = ip or os.environ["SSH_CONNECTION"].split()[2]
+            self.nexus_run_port = port
             self.working_on_ipv6 = False
             if ":" in self.nexus_run_ip:  # ipv6格式需要用括号包住域名部分
                 self.nexus_run_ip = "[%s]" % self.nexus_run_ip
                 self.working_on_ipv6 = True
         except KeyError:
-            raise RuntimeError("Do not switch users after SSH connection")
-        self.root_dir = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-        self.config = f"{self.root_dir}/scripts/nexus_config.json"
+            raise RuntimeError("Get environment variable SSH_CONNECTION failed,maybe switch users after SSH connection")
+        self.nexus_url = "http://{}:{}".format(self.nexus_run_ip, self.nexus_run_port)
+        self.config = "{}/scripts/nexus_config.json".format(ROOT_PATH)
         self.arch = platform.machine()
         os.environ.pop("http_proxy", "")
         os.environ.pop("https_proxy", "")
-        with open(self.config, "r", encoding="utf-8") as f:
+        with open(self.config, "r") as f:
             self.config_content = json.load(f)
         self.nexus_data_dir = os.path.join("/tmp", "nexus-data")
         self.nexus_image_name = self.config_content.get("image")
+        nexus_dir = os.path.join(ROOT_PATH, "resources", "nexus")
         try:
-            self.nexus_image = glob.glob(
-                f'{os.path.join(self.root_dir, "resources", "nexus")}/nexus*{self.arch}.tar'
-            )[0]
+            self.nexus_image = glob.glob("{}/nexus*{}.tar".format(nexus_dir, self.arch))[0]
         except IndexError:
-            raise FileNotFoundError("nexus image does not exist") from None
-        auth = base64.b64encode(
-            f"{self.NEXUS_USER}:{self.nexus_passwd}".encode("utf-8")
-        ).decode("utf-8")
+            raise RuntimeError(
+                "The nexus image does not exist. Ensure that the nexus image is in the {} directory.".format(nexus_dir)
+            )
+        auth = base64.b64encode("{}:{}".format(self.NEXUS_USER, self.nexus_passwd).encode()).decode()
         self.post_headers = {
             "Content-Type": "application/json",
-            "Authorization": f"Basic {auth}",
+            "Authorization": "Basic {}".format(auth),
         }
         self.upload_headers = {
-            "Authorization": f"Basic {auth}",
+            "Authorization": "Basic {}".format(auth),
             "Content-Type": "application/octet-stream",
         }
 
     @staticmethod
-    def _delete_nexus_container():
-        container_info = "docker ps -a"
-        try:
-            info_result = subprocess.run(
-                shlex.split(container_info),
-                shell=False,
-                encoding="utf-8",
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                check=True,
-            )
-        except FileNotFoundError:
-            raise FileNotFoundError("Please install Docker first")
-        except subprocess.CalledProcessError:
-            raise RuntimeError("Docker not available")
-        else:
-            if "nexus" in info_result.stdout.split():
-                delete_cmd = "docker rm -f nexus"
-                subprocess.run(
-                    shlex.split(delete_cmd),
-                    shell=False,
-                    stdout=subprocess.DEVNULL,
-                    stderr=subprocess.DEVNULL,
-                )
-            subprocess.run(
-                shlex.split("docker network rm ip6net_nexus"),
-                shell=False,
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-            )
+    def _run_cmd(cmd, ignore_errors=False, log=True):
+        if log:
+            LOG.info("nexus: {}".format(cmd).center(120, "-"))
+        result = subprocess.Popen(
+            shlex.split(cmd),
+            shell=False,
+            universal_newlines=True,
+            stderr=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+        )
+        out, err = result.communicate()
+        if result.returncode != 0 and not ignore_errors:
+            raise RuntimeError("run cmd: {} failed, reason: {}".format(cmd, err))
+        if log:
+            for line in out.splitlines():
+                LOG.info(line)
+        return out, err
 
     @staticmethod
-    def _check_nexus_status():
-        check_cmd = "docker logs nexus"
-        timeout = 0
-        while True:
-            time.sleep(10)
-            timeout += 10
-            nexus_status = subprocess.run(
-                shlex.split(check_cmd),
-                shell=False,
-                stdout=subprocess.PIPE,
-                encoding="utf-8",
-                check=True,
-            )
-            if "Nexus OSS" in nexus_status.stdout:
-                break
-            if timeout >= 120:
-                raise TimeoutError("Nexus startup timeout")
+    def _run_request(url, data, headers, method, timeout=20):
+        if PY3:
+            req = Request(url=url, data=data, headers=headers, method=method)
+        else:
+            req = Request(url=url, data=data, headers=headers)
+            req.get_method = lambda: method
+        urlopen(req, timeout=timeout)
 
     def init_nexus(self):
         self._run_nexus()
         self._check_nexus_status()
-        tmp_passwd_file = f"{self.nexus_data_dir}/admin.password"
-        with open(tmp_passwd_file, "r", encoding="utf-8") as f:
+        tmp_passwd_file = "{}/admin.password".format(self.nexus_data_dir)
+        with open(tmp_passwd_file, "r") as f:
             old_passwd = f.read()
-        auth = base64.b64encode(
-            f"{self.NEXUS_USER}:{old_passwd}".encode("utf-8")
-        ).decode("utf-8")
+        auth = base64.b64encode("{}:{}".format(self.NEXUS_USER, old_passwd).encode()).decode()
         headers = {
             "accept": "application/json",
             "Content-Type": "text/plain",
-            "Authorization": f"Basic {auth}",
+            "Authorization": "Basic {}".format(auth),
         }
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/security/users/admin/change-password"
-        req = request.Request(
-            url,
-            data=self.nexus_passwd.encode("utf-8"),
-            headers=headers,
-            method="PUT",
-        )
-        request.urlopen(req)
+        url = "{}/service/rest/v1/security/users/admin/change-password".format(self.nexus_url)
+        self._run_request(url, data=self.nexus_passwd.encode("utf-8"), headers=headers, method="PUT")
 
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/security/anonymous"
+        url = "{}/service/rest/v1/security/anonymous".format(self.nexus_url)
         data = {
             "enabled": True,
             "userId": "anonymous",
             "realmName": "NexusAuthorizingRealm",
         }
-        req = request.Request(
-            url,
-            data=json.dumps(data).encode("utf-8"),
-            headers=self.post_headers,
-            method="PUT",
-        )
-        request.urlopen(req)
+        self._run_request(url, data=json.dumps(data).encode("utf-8"), headers=self.post_headers, method="PUT")
 
-    def get_download_os_info(self):
-        os_list_dir = f"{self.root_dir}/resources"
-        os_list = [os_item for os_item in glob.glob(f"{os_list_dir}/*aarch64")]
-        os_list.extend(os_item for os_item in glob.glob(f"{os_list_dir}/*x86_64"))
+    @staticmethod
+    def get_download_os_info():
+        os_list_dir = "{}/resources".format(ROOT_PATH)
+        os_list = [os_item for os_item in glob.glob("{}/*aarch64".format(os_list_dir))]
+        os_list.extend(os_item for os_item in glob.glob("{}/*x86_64".format(os_list_dir)))
         return os_list
 
-    def get_os_files(self, os_dir):
+    def _delete_nexus_container(self):
+        out, err = self._run_cmd("docker ps -a", ignore_errors=True)
+        if "daemon running" in err:
+            self._run_cmd("systemctl daemon-reload")
+            self._run_cmd("systemctl restart docker")
+            out, _ = self._run_cmd("docker ps -a")
+        if "nexus" in out.split():
+            self._run_cmd("docker rm -f nexus")
+        self._run_cmd("docker network rm ip6net_nexus", ignore_errors=True)
+
+    def _check_nexus_status(self):
+        timeout = 0
+        while True:
+            time.sleep(1)
+            timeout += 1
+            out, _ = self._run_cmd("docker logs nexus", log=False)
+            if "Nexus OSS" in out:
+                break
+            if timeout >= 300:
+                raise RuntimeError("Nexus startup timeout")
+
+    def _get_os_files(self, os_dir):
         files = []
         for file_name in os.listdir(os_dir):
             file_path = os.path.join(os_dir, file_name)
             if os.path.isdir(file_path):
-                files.extend(self.get_os_files(file_path))
+                files.extend(self._get_os_files(file_path))
             else:
                 files.append(file_path)
         return files
 
     def _create_data_dir(self):
-        try:
-            os.makedirs(self.nexus_data_dir, mode=0o700)
-        except FileExistsError:
+        if os.path.exists(self.nexus_data_dir):
             try:
                 shutil.rmtree(self.nexus_data_dir)
             except OSError:
-                umount_data_dir_cmd = f"umount {self.nexus_data_dir}"
-                subprocess.run(shlex.split(umount_data_dir_cmd), shell=False, stderr=subprocess.DEVNULL)
+                self._run_cmd("umount {}".format(self.nexus_data_dir))
                 shutil.rmtree(self.nexus_data_dir)
-            finally:
-                os.makedirs(self.nexus_data_dir, mode=0o700)
-        os.chown(self.nexus_data_dir, 200, 200)
-        mount_data_dir_cmd = f"mount -t tmpfs tmpfs {self.nexus_data_dir}"
-        subprocess.run(shlex.split(mount_data_dir_cmd), shell=False, check=True)
+        os.makedirs(self.nexus_data_dir, mode=0o700)
+        self._run_cmd("mount -t tmpfs tmpfs {}".format(self.nexus_data_dir))
 
     def _run_nexus(self):
         self._delete_nexus_container()
         self._create_data_dir()
         network_command_opt = ""
         if self.working_on_ipv6:
             if not os.path.exists("/etc/docker/daemon.json"):
@@ -209,42 +202,33 @@
                     json.dump({}, fid, indent=1)
             with open("/etc/docker/daemon.json") as fid:
                 docker_settings = json.load(fid)
             docker_settings["experimental"] = True
             docker_settings["ip6tables"] = True
             with open("/etc/docker/daemon.json", "w") as fid:
                 json.dump(docker_settings, fid, indent=1)
-            subprocess.getoutput("systemctl restart docker")
-            subprocess.getoutput("docker network create --ipv6 --subnet 2001:0DB8::/112 ip6net_nexus")
+            self._run_cmd("systemctl daemon-reload")
+            self._run_cmd("systemctl restart docker")
+            self._run_cmd("docker network create --ipv6 --subnet 2001:0DB8::/112 ip6net_nexus")
             network_command_opt = "--network ip6net_nexus"
-        load_cmd = f"docker load -i {self.nexus_image}"
-        subprocess.run(shlex.split(load_cmd), shell=False, stdout=subprocess.DEVNULL)
-        run_cmd = (
-            f"docker run -d --name nexus {network_command_opt} -p {self.NEXUS_RUN_PORT}:8081 "
-            f"-v {self.nexus_data_dir}:/nexus-data {self.nexus_image_name}"
-        )
-        subprocess.run(
-            shlex.split(run_cmd), shell=False, check=True, stdout=subprocess.DEVNULL
+        self._run_cmd("docker load -i {}".format(self.nexus_image))
+        start_nexus_cmd = "docker run -d --privileged --name nexus {} -p {}:8081 -v {}:/nexus-data {}".format(
+            network_command_opt, self.nexus_run_port, self.nexus_data_dir, self.nexus_image_name
         )
+        self._run_cmd(start_nexus_cmd)
 
 
 class YumRepository(OsRepository):
     def create_blob(self):
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/blobstores/file"
+        url = "{}/service/rest/v1/blobstores/file".format(self.nexus_url)
         data = {"softQuota": None, "path": "/nexus-data/blobs/yum", "name": "yum"}
-        req = request.Request(
-            url,
-            data=json.dumps(data).encode("utf-8"),
-            headers=self.post_headers,
-            method="POST",
-        )
-        request.urlopen(req)
+        self._run_request(url, data=json.dumps(data).encode("utf-8"), headers=self.post_headers, method="POST")
 
     def create_repository(self):
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/repositories/yum/hosted"
+        url = "{}/service/rest/v1/repositories/yum/hosted".format(self.nexus_url)
         os_info = self.get_download_os_info()
         for i in os_info:
             repository_name = os.path.basename(i)
             if repository_name in self.config_content["rpm_os"]:
                 data = {
                     "name": repository_name,
                     "online": True,
@@ -255,106 +239,86 @@
                     },
                     "cleanup": None,
                     "component": {
                         "proprietaryComponents": False,
                     },
                     "yum": {"repodataDepth": 0, "deployPolicy": "STRICT"},
                 }
-                req = request.Request(
-                    url,
-                    data=json.dumps(data).encode("utf-8"),
-                    headers=self.post_headers,
-                    method="POST",
-                )
-                request.urlopen(req)
+                self._run_request(url, data=json.dumps(data).encode("utf-8"), headers=self.post_headers, method="POST")
 
     def upload_rpm(self):
-        base_url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/repository/"
+        base_url = "{}/repository/".format(self.nexus_url)
         download_os_list = self.get_download_os_info()
-        for i in download_os_list:
-            os_name = os.path.basename(i)
+        for download_os in download_os_list:
+            os_name = os.path.basename(download_os)
             if os_name not in self.config_content["rpm_os"]:
                 continue
-            os_deps = self.get_os_files(i)
-            if "CentOS_7.6" in os_name:
-                # centos 7需要强制安装固定版本的包，不需要加入源中
-                os_deps = [os_dep for os_dep in os_deps if not re.search(r"openssl.*1\.1\.1", os_dep)
-                           and not re.search(r"kernel.*4\.14", os_dep)
-                           and not re.search(r"kernel.*3\.10\.0-957", os_dep)]
-            for j in os_deps:
-                with open(j, "rb") as f:
+            os_deps = self._get_os_files(download_os)
+            for os_dep in os_deps:
+                with open(os_dep, "rb") as f:
                     file_content = f.read()
-                url = parse.urljoin(
-                    base_url, f"{os.path.basename(i)}/{os.path.basename(j)}"
-                )
-                req = request.Request(
-                    url, data=file_content, headers=self.upload_headers, method="PUT"
-                )
-                request.urlopen(req)
+                url = urljoin(base_url, "{}/{}".format(os.path.basename(download_os), os.path.basename(os_dep)))
+                self._run_request(url, data=file_content, headers=self.upload_headers, method="PUT")
 
 
 class AptRepository(OsRepository):
     def generate_gpg_key(self):
-        gpg_dir = f"{os.environ['HOME']}/.gnupg"
+        gpg_dir = os.path.expanduser("~/.gnupg")
         if os.path.exists(gpg_dir):
             shutil.rmtree(gpg_dir)
         base_cmd = "gpg --gen-key --batch"
-        gpg_data = f"""Key-Type: RSA
+        gpg_data = """Key-Type: RSA
         Key-Length: 3072
         Name-Real: nexus
         Expire-Date: 3d
-        Passphrase: {self.gpg_passwd}
-        """
-        subprocess.run(
+        Passphrase: {}
+        """.format(
+            self.gpg_passwd
+        )
+        result = subprocess.Popen(
             shlex.split(base_cmd),
-            input=gpg_data.encode("utf-8"),
             shell=False,
-            check=True,
+            universal_newlines=True,
+            stderr=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stdin=subprocess.PIPE,
         )
+        result.communicate(input=gpg_data)
+        if result.returncode != 0:
+            raise RuntimeError("GPG key generation failed")
 
     def export_gpg_key(self):
         gpg_key_dir = os.path.dirname(self.nexus_image)
-        gpg_pub_key = f"{gpg_key_dir}/nexus_pub.asc"
-        gpg_pri_key = f"{gpg_key_dir}/nexus_pri.asc"
+        gpg_pub_key = "{}/nexus_pub.asc".format(gpg_key_dir)
+        gpg_pri_key = "{}/nexus_pri.asc".format(gpg_key_dir)
         if os.path.exists(gpg_pub_key):
             os.unlink(gpg_pub_key)
         if os.path.exists(gpg_pri_key):
             os.unlink(gpg_pri_key)
-        export_public_key_cmd = f"gpg -a -o {gpg_pub_key} --export nexus"
+        export_public_key_cmd = "gpg -a -o {} --export nexus".format(gpg_pub_key)
         export_private_key_cmd = (
-            f"gpg --batch --pinentry-mode=loopback --yes --passphrase {self.gpg_passwd} "
-            f"-a -o {gpg_pri_key} --export-secret-key nexus"
-        )
-        subprocess.run(
-            shlex.split(export_public_key_cmd),
-            shell=False,
-            check=True,
-        )
-        subprocess.run(
-            shlex.split(export_private_key_cmd),
-            shell=False,
-            check=True,
+            "gpg --batch --pinentry-mode=loopback --yes --passphrase {} "
+            "-a -o {} --export-secret-key nexus".format(self.gpg_passwd, gpg_pri_key)
         )
-        with open(gpg_pri_key, "r", encoding="utf-8") as f:
+        centos_release = "/etc/centos-release"
+        if os.path.exists(centos_release):
+            export_private_key_cmd = "gpg -a -o {} --export-secret-key nexus".format(gpg_pri_key)
+        self._run_cmd(export_public_key_cmd)
+        self._run_cmd(export_private_key_cmd, log=False)
+        with open(gpg_pri_key, "r") as f:
             gpg_pri_content = f.read()
         return gpg_pri_content
 
     def create_blob(self):
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/blobstores/file"
+        url = "{}/service/rest/v1/blobstores/file".format(self.nexus_url)
         data = {"softQuota": None, "path": "/nexus-data/blobs/apt", "name": "apt"}
-        req = request.Request(
-            url,
-            data=json.dumps(data).encode("utf-8"),
-            headers=self.post_headers,
-            method="POST",
-        )
-        request.urlopen(req)
+        self._run_request(url, data=json.dumps(data).encode("utf-8"), headers=self.post_headers, method="POST")
 
     def create_repository(self, keypair):
-        url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/service/rest/v1/repositories/apt/hosted"
+        url = "{}/service/rest/v1/repositories/apt/hosted".format(self.nexus_url)
         os_info = self.get_download_os_info()
         for i in os_info:
             repository_name = os.path.basename(i)
             if repository_name in self.config_content["deb_os"]:
                 codename = self.config_content["codename"][repository_name]
                 data = {
                     "name": repository_name,
@@ -367,66 +331,42 @@
                     "cleanup": None,
                     "component": {
                         "proprietaryComponents": False,
                     },
                     "apt": {"distribution": codename},
                     "aptSigning": {"keypair": keypair, "passphrase": self.gpg_passwd},
                 }
-                req = request.Request(
-                    url,
-                    data=json.dumps(data).encode("utf-8"),
-                    headers=self.post_headers,
-                    method="POST",
-                )
-                request.urlopen(req)
+                self._run_request(url, data=json.dumps(data).encode("utf-8"), headers=self.post_headers, method="POST")
 
     def upload_deb(self):
-        base_url = f"http://{self.nexus_run_ip}:{self.NEXUS_RUN_PORT}/repository/"
+        base_url = "{}/repository/".format(self.nexus_url)
         download_os_list = self.get_download_os_info()
-        for i in download_os_list:
-            if os.path.basename(i) not in self.config_content["deb_os"]:
+        for download_os in download_os_list:
+            if os.path.basename(download_os) not in self.config_content["deb_os"]:
                 continue
-            os_deps = self.get_os_files(i)
-            for j in os_deps:
-                with open(j, "rb") as f:
+            os_deps = self._get_os_files(download_os)
+            for os_dep in os_deps:
+                with open(os_dep, "rb") as f:
                     file_content = f.read()
-                url = parse.urljoin(base_url, f"{os.path.basename(i)}/")
-                req = request.Request(
-                    url,
-                    data=file_content,
-                    headers=self.upload_headers,
-                    method="POST",
-                )
-                request.urlopen(req)
-
-
-def main():
-    yum_repository = YumRepository()
-    download_os_list = [
-        os.path.basename(i)
-        for i in yum_repository.get_download_os_info()
-    ]
-    have_rpm = any(
-        os_item in yum_repository.config_content["rpm_os"]
-        for os_item in download_os_list
-    )
-    have_deb = any(
-        os_item in yum_repository.config_content["deb_os"]
-        for os_item in download_os_list
-    )
+                url = urljoin(base_url, "{}/".format(os.path.basename(download_os)))
+                self._run_request(url, data=file_content, headers=self.upload_headers, method="POST")
+
+
+def main(ip=None, port=58081):
+    yum_repository = YumRepository(ip, port)
+    download_os_list = [os.path.basename(os_name) for os_name in yum_repository.get_download_os_info()]
+    have_rpm = any(os_item in yum_repository.config_content["rpm_os"] for os_item in download_os_list)
+    have_deb = any(os_item in yum_repository.config_content["deb_os"] for os_item in download_os_list)
     yum_repository.init_nexus()
     if have_rpm:
         yum_repository.create_blob()
         yum_repository.create_repository()
         yum_repository.upload_rpm()
     if have_deb:
-        centos_release = "/etc/centos-release"
-        if os.path.exists(centos_release):
-            return
-        apt_repository = AptRepository()
+        apt_repository = AptRepository(ip, port)
         apt_repository.create_blob()
         apt_repository.generate_gpg_key()
         gpg_pair_key = apt_repository.export_gpg_key()
         if gpg_pair_key == "":
             raise RuntimeError("The file content is empty")
         apt_repository.create_repository(gpg_pair_key)
         apt_repository.upload_deb()
```

## ascend_deployer/scripts/nexus_config.json

### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'common_docker'": '{delete: [4]}'}*

```diff
@@ -7,16 +7,15 @@
         "Ubuntu_22.04_aarch64": "jammy",
         "Ubuntu_22.04_x86_64": "jammy"
     },
     "common_docker": [
         "docker-ce-cli",
         "containerd.io",
         "docker-ce-rootless-extras",
-        "docker-ce",
-        "docker-scan-plugin"
+        "docker-ce"
     ],
     "deb_os": [
         "Ubuntu_18.04_aarch64",
         "Ubuntu_18.04_x86_64",
         "Ubuntu_20.04_aarch64",
         "Ubuntu_20.04_x86_64",
         "Ubuntu_22.04_aarch64",
```

## ascend_deployer/tools/hccn.py

```diff
@@ -35,15 +35,15 @@
 DSCP_TC_TEMPLATE = "dscp_tc_%s=%s\n"
 BITMAP_TEMPLATE = "bitmap_%s=%s\n"
 
 GATEWAY_TEMPLATE = "gateway_%s=%s\n"
 IPV6_GATEWAY_TEMPLATE = "IPv6gateway_%s=%s\n"
 ARP_TEMPLATE = "arp_%s=-i eth%s -s %s %s\n"
 
-RET_ERROR_CODE = -1
+RET_ERROR_CODE = 127
 FIRST_CARD_IN_SECOND_GROUP = 4
 FIRST_GROUP = (0, 1, 2, 3)
 SECOND_GROUP = (4, 5, 6, 7)
 
 
 def is_ipv6(address):
     return ":" in address
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_aarch64.json`

 * *Files 7% similar despite different names*

### Pretty-printed

 * *Similarity: 0.5916666666666667%*

 * *Differences: {'0': "{'filename': 'aarch64.tar.gz', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/aarch64.tar.gz', "*

 * *      "'sha256': '0961649ba32d2841e99eb35e3606ea1d02c5b36ea6108337c0791739e3e6029c', 'dest': "*

 * *      "'resources/basic/OpenEuler_22.03_LTS'}",*

 * * '1': "{'filename': 'hccn-x86_64', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64', "*

 * *      "'sha256': '66cd8d314b004e9e776 […]*

```diff
@@ -1,37 +1,43 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
+        "dest": "resources/basic/OpenEuler_22.03_LTS",
+        "filename": "aarch64.tar.gz",
+        "sha256": "0961649ba32d2841e99eb35e3606ea1d02c5b36ea6108337c0791739e3e6029c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/aarch64.tar.gz"
     },
     {
-        "dest": "resources/basic/CentOS_7.6",
-        "filename": "aarch64.tar.gz",
-        "sha256": "b45569ca4cf608a757d7297b0f1188e0badbc9308c83fc793ba097682cdd26a9",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/aarch64.tar.gz"
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-x86_64",
+        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "aarch64.tar.gz",
-        "sha256": "53a7790afa41981eb9aafa998eb50a1226084bb289d8ad3998da94d213f2c58c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/aarch64.tar.gz"
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64.tar.gz",
         "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz"
     },
     {
-        "dest": "resources/k8s/CentOS_7.6",
+        "dest": "resources/k8s/OpenEuler_22.03_LTS",
+        "filename": "aarch64.tar.gz",
+        "sha256": "9af656931f3a0b513582cb75f5ced99c5dba4eef074d19bfab97adfe4de0c9d9",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/aarch64.tar.gz"
+    },
+    {
+        "dest": "resources/k8s/OpenEuler_22.03_LTS",
         "filename": "aarch64_125.tar.gz",
         "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/aarch64_125.tar.gz"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/aarch64_125.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz"
     },
@@ -39,48 +45,30 @@
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-aarch64",
         "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-aarch64"
     },
     {
         "dest": "resources/tool/hccn",
-        "filename": "hccn-x86_64",
-        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
-    },
-    {
-        "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/CentOS_7.6",
+        "dest": "resources/docker/OpenEuler_22.03_LTS",
         "filename": "aarch64.tar.gz",
-        "sha256": "ca7e176d6fb4092daa3c737b2b5ecfef0586a96b77e83d1720f05da5d58e8d54",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/aarch64.tar.gz"
+        "sha256": "27d009ea84a868f116aaa8b529feddc0671986082ace26c2036630a71b2acdc8",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
-    },
-    {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_x86_64.json`

 * *Files 10% similar despite different names*

### Pretty-printed

 * *Similarity: 0.6166666666666667%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/x86_64.tar.gz', "*

 * *      "'sha256': '00cd150464b15f58da158e631dee301f09e774b9942f95345ac4bc9693dcd490', 'dest': "*

 * *      "'resources/basic/OpenEuler_22.03_LTS'}",*

 * * '2': "{'filename': 'calico_v3.25.0.yaml', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml', "*

 * *      "'sha256': '0b642c65295d7d80af8600da87e1d80924 […]*

```diff
@@ -1,86 +1,74 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/CentOS_7.6",
-        "filename": "x86_64.tar.gz",
-        "sha256": "d60a97c169d92dcb33e34c6c7ecf93cbf8e03c3893bc01540a8e2ce9fe772ddc",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/CentOS_7.6",
+        "dest": "resources/basic/OpenEuler_22.03_LTS",
         "filename": "x86_64.tar.gz",
-        "sha256": "5659e7b8bb1afdb1e32385083ba84ada396f94316942d2bce3e0ac6ba753c47a",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/x86_64.tar.gz"
+        "sha256": "00cd150464b15f58da158e631dee301f09e774b9942f95345ac4bc9693dcd490",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64.tar.gz",
         "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64.tar.gz"
     },
     {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "x86_64_125.tar.gz",
-        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/x86_64_125.tar.gz"
-    },
-    {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
+        "dest": "resources/k8s/OpenEuler_22.03_LTS",
+        "filename": "x86_64_125.tar.gz",
+        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/x86_64_125.tar.gz"
+    },
+    {
         "dest": "resources/k8s/image",
         "filename": "x86_64_125.tar.gz",
         "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
+        "dest": "resources/k8s/OpenEuler_22.03_LTS",
+        "filename": "x86_64.tar.gz",
+        "sha256": "bc8448a40d4943ba3b73f308104c373f6f77eb4c81b7c4be5a603ff08869050f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/x86_64.tar.gz"
+    },
+    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-x86_64",
         "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-x86_64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/docker/CentOS_7.6",
+        "dest": "resources/docker/OpenEuler_22.03_LTS",
         "filename": "x86_64.tar.gz",
-        "sha256": "59788bffd89e4e03c95cf7a7e048dba3d88a147abaaa4d0cc9e3454e0fbd1420",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/x86_64.tar.gz"
+        "sha256": "50c5047685563ae9c46f69d23107ae36e70ec2fb697f0802d7eb9d771ae7d3d1",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_aarch64.json`

 * *Files 14% similar despite different names*

### Pretty-printed

 * *Similarity: 0.53125%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_22.04/aarch64.tar.gz', "*

 * *      "'sha256': '9d7ce6479fc06d4409be732cd87fa3c6c7863cc2ea6f63a9f945d6839e2fb4f0', 'dest': "*

 * *      "'resources/basic/Ubuntu_22.04'}",*

 * * '3': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz', "*

 * *      "'sha256': '453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b', 'dest': "*

 * *       […]*

```diff
@@ -1,86 +1,74 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/Kylin_V10",
-        "filename": "aarch64.tar.gz",
-        "sha256": "5b12caba5d2b90820716af394d48268964777accaeac5a98f6b657fb9dc6abf5",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Kylin_V10/aarch64.tar.gz"
-    },
-    {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-x86_64",
-        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
-    },
-    {
-        "dest": "resources/k8s/Kylin_V10",
+        "dest": "resources/basic/Ubuntu_22.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "e35c4d06bb3d81c7bba91bd3c70032f1eaa5d4649c0ce4bd89231a9b13a87c51",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Kylin_V10/aarch64.tar.gz"
+        "sha256": "9d7ce6479fc06d4409be732cd87fa3c6c7863cc2ea6f63a9f945d6839e2fb4f0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_22.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64.tar.gz",
         "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz"
     },
     {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/Kylin_V10",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Kylin_V10/aarch64_125.tar.gz"
-    },
-    {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz"
     },
     {
+        "dest": "resources/k8s/Ubuntu_22.04",
+        "filename": "aarch64_125.tar.gz",
+        "sha256": "9a539919c113beeae353a61342ad5cd9ad6ba4d96f7340671aa7901f377a7da8",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/aarch64_125.tar.gz"
+    },
+    {
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-x86_64",
+        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
+    },
+    {
+        "dest": "resources/k8s/Ubuntu_22.04",
+        "filename": "aarch64.tar.gz",
+        "sha256": "61cca1afc331bf719169f1e22710600c30d965dc627254e6dda40f346c8798e8",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/aarch64.tar.gz"
+    },
+    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-aarch64",
         "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-aarch64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/Kylin_V10",
+        "dest": "resources/docker/Ubuntu_22.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "f33ba8b8bb240449b87f627a4a287cc811783f6401c9ff12f4b909988a6ecb58",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Kylin_V10/aarch64.tar.gz"
+        "sha256": "7acc79a78e3804cf5a764e2c6320199e74d17d91a2cad5a6c059a6e90aaca937",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_22.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json` & `ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_x86_64.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.5390625%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/x86_64.tar.gz', "*

 * *      "'sha256': 'd60a97c169d92dcb33e34c6c7ecf93cbf8e03c3893bc01540a8e2ce9fe772ddc', 'dest': "*

 * *      "'resources/basic/CentOS_7.6'}",*

 * * '1': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/x86_64.tar.gz', "*

 * *      "'sha256': '5659e7b8bb1afdb1e32385083ba84ada396f94316942d2bce3e0ac6ba753c47a', 'dest': "*

 * *      "'res […]*

```diff
@@ -1,86 +1,74 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/Kylin_V10",
+        "dest": "resources/basic/CentOS_7.6",
         "filename": "x86_64.tar.gz",
-        "sha256": "790bf9c94fc86976703bf8526ea9ad7587f2ddefe4b7e2bb92384487cb7e5d3f",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Kylin_V10/x86_64.tar.gz"
+        "sha256": "d60a97c169d92dcb33e34c6c7ecf93cbf8e03c3893bc01540a8e2ce9fe772ddc",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/x86_64.tar.gz"
     },
     {
-        "dest": "resources/k8s/Kylin_V10",
+        "dest": "resources/k8s/CentOS_7.6",
         "filename": "x86_64.tar.gz",
-        "sha256": "fb67d25ddf6f8e6318afa40d13025ca7788952400322cd5a5add0f8f59588326",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Kylin_V10/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
-    },
-    {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-aarch64",
-        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
+        "sha256": "5659e7b8bb1afdb1e32385083ba84ada396f94316942d2bce3e0ac6ba753c47a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64.tar.gz",
         "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64.tar.gz"
     },
     {
-        "dest": "resources/k8s/Kylin_V10",
+        "dest": "resources/k8s/CentOS_7.6",
         "filename": "x86_64_125.tar.gz",
         "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Kylin_V10/x86_64_125.tar.gz"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/x86_64_125.tar.gz"
+    },
+    {
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64_125.tar.gz",
         "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-aarch64",
+        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
+    },
+    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-x86_64",
         "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-x86_64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/docker/Kylin_V10",
+        "dest": "resources/docker/CentOS_7.6",
         "filename": "x86_64.tar.gz",
-        "sha256": "acbc31887d44ebfdfeaa80c36106d595b8979d1568f316f829efc9b5226dd764",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Kylin_V10/x86_64.tar.gz"
+        "sha256": "59788bffd89e4e03c95cf7a7e048dba3d88a147abaaa4d0cc9e3454e0fbd1420",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_aarch64.json`

 * *Files 5% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[12, 0]'}*

```diff
@@ -1,15 +1,9 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
         "dest": "resources/basic/OpenEuler_20.03_LTS",
         "filename": "aarch64.tar.gz",
         "sha256": "5de0559e24e843dea8ffe5a13fbb7f86a33665ce58642840829570db812ef232",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_20.03_LTS/aarch64.tar.gz"
     },
     {
         "dest": "resources/k8s/OpenEuler_20.03_LTS",
@@ -68,19 +62,13 @@
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_x86_64.json`

 * *Files 4% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[12, 0]'}*

```diff
@@ -1,15 +1,9 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
         "dest": "resources/basic/OpenEuler_20.03_LTS",
         "filename": "x86_64.tar.gz",
         "sha256": "ab97ee4b1f5b7dcff49be1e391ef21c214cf08aef647c08539ec89f5a0022bc5",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_20.03_LTS/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/OpenEuler_20.03_LTS",
@@ -68,19 +62,13 @@
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_aarch64.json`

 * *Files 15% similar despite different names*

### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_18.04/aarch64.tar.gz', "*

 * *      "'sha256': '96055ac3d6cfeddac66e775864b53055893fd3ea25361be449f49cdc9e1ff0b0', 'dest': "*

 * *      "'resources/basic/Ubuntu_18.04'}",*

 * * '4': "{'filename': 'aarch64_125.tar.gz', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz', "*

 * *      "'sha256': '453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd33344 […]*

```diff
@@ -1,86 +1,74 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/OpenEuler_22.03_LTS",
+        "dest": "resources/basic/Ubuntu_18.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "0961649ba32d2841e99eb35e3606ea1d02c5b36ea6108337c0791739e3e6029c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/aarch64.tar.gz"
+        "sha256": "96055ac3d6cfeddac66e775864b53055893fd3ea25361be449f49cdc9e1ff0b0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_18.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
-    },
-    {
         "dest": "resources/k8s/image",
         "filename": "aarch64.tar.gz",
         "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz"
     },
     {
-        "dest": "resources/k8s/OpenEuler_22.03_LTS",
-        "filename": "aarch64.tar.gz",
-        "sha256": "9af656931f3a0b513582cb75f5ced99c5dba4eef074d19bfab97adfe4de0c9d9",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/aarch64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/OpenEuler_22.03_LTS",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/aarch64_125.tar.gz"
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz"
     },
     {
+        "dest": "resources/k8s/Ubuntu_18.04",
+        "filename": "aarch64_125.tar.gz",
+        "sha256": "9a539919c113beeae353a61342ad5cd9ad6ba4d96f7340671aa7901f377a7da8",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_18.04/aarch64_125.tar.gz"
+    },
+    {
+        "dest": "resources/k8s/Ubuntu_18.04",
+        "filename": "aarch64.tar.gz",
+        "sha256": "b2fba0341e2b99d338580859d8877303af828bb442e277659a45f1ec152d6dca",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_18.04/aarch64.tar.gz"
+    },
+    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-aarch64",
         "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-aarch64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/OpenEuler_22.03_LTS",
+        "dest": "resources/docker/Ubuntu_18.04",
         "filename": "aarch64.tar.gz",
-        "sha256": "27d009ea84a868f116aaa8b529feddc0671986082ace26c2036630a71b2acdc8",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/aarch64.tar.gz"
+        "sha256": "d3761acb25a39ba9ba89928e29a8f2c55b2d3fbd7d3e2149e8c469483a4bf5aa",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_18.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_x86_64.json`

 * *Files 18% similar despite different names*

### Pretty-printed

 * *Similarity: 0.6964285714285714%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_20.04/x86_64.tar.gz', "*

 * *      "'sha256': '51e05d46e794179fd343e7e1578df0e487da71d092ed6e5c82085d2950709ad1', 'dest': "*

 * *      "'resources/basic/Ubuntu_20.04'}",*

 * * '3': "{'filename': 'x86_64.tar.gz', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_20.04/x86_64.tar.gz', "*

 * *      "'sha256': '889b7f69b812b4b92767964296473466616899db48474ac47cae0 […]*

```diff
@@ -1,86 +1,74 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/OpenEuler_22.03_LTS",
+        "dest": "resources/basic/Ubuntu_20.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "00cd150464b15f58da158e631dee301f09e774b9942f95345ac4bc9693dcd490",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/OpenEuler_22.03_LTS/x86_64.tar.gz"
+        "sha256": "51e05d46e794179fd343e7e1578df0e487da71d092ed6e5c82085d2950709ad1",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_20.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64.tar.gz",
         "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64.tar.gz"
     },
     {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/OpenEuler_22.03_LTS",
-        "filename": "x86_64_125.tar.gz",
-        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/x86_64_125.tar.gz"
+        "dest": "resources/k8s/Ubuntu_20.04",
+        "filename": "x86_64.tar.gz",
+        "sha256": "889b7f69b812b4b92767964296473466616899db48474ac47cae0c7382facac9",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_20.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64_125.tar.gz",
         "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
+        "dest": "resources/k8s/Ubuntu_20.04",
+        "filename": "x86_64_125.tar.gz",
+        "sha256": "33507c061fd2dcdb9357d3e1253b922779a2ddc8faf7cb7620134091f94b4284",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_20.04/x86_64_125.tar.gz"
+    },
+    {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/k8s/OpenEuler_22.03_LTS",
-        "filename": "x86_64.tar.gz",
-        "sha256": "bc8448a40d4943ba3b73f308104c373f6f77eb4c81b7c4be5a603ff08869050f",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/OpenEuler_22.03_LTS/x86_64.tar.gz"
-    },
-    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-x86_64",
         "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-x86_64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/docker/OpenEuler_22.03_LTS",
+        "dest": "resources/docker/Ubuntu_20.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "50c5047685563ae9c46f69d23107ae36e70ec2fb697f0802d7eb9d771ae7d3d1",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/OpenEuler_22.03_LTS/x86_64.tar.gz"
+        "sha256": "fc3d51e849a79bc3332acf0e493e1ad0aabad3e705f8a299c0630c32021c5c91",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_20.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_aarch64.json`

 * *Files 14% similar despite different names*

### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/aarch64.tar.gz', "*

 * *      "'sha256': 'b45569ca4cf608a757d7297b0f1188e0badbc9308c83fc793ba097682cdd26a9', 'dest': "*

 * *      "'resources/basic/CentOS_7.6'}",*

 * * '1': "{'filename': 'aarch64.tar.gz', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/aarch64.tar.gz', "*

 * *      "'sha256': '53a7790afa41981eb9aafa998eb50a1226084bb289d8ad3998da94d2 […]*

```diff
@@ -1,85 +1,73 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/Ubuntu_18.04",
+        "dest": "resources/basic/CentOS_7.6",
         "filename": "aarch64.tar.gz",
-        "sha256": "96055ac3d6cfeddac66e775864b53055893fd3ea25361be449f49cdc9e1ff0b0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_18.04/aarch64.tar.gz"
+        "sha256": "b45569ca4cf608a757d7297b0f1188e0badbc9308c83fc793ba097682cdd26a9",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/CentOS_7.6/aarch64.tar.gz"
     },
     {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-x86_64",
-        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
+        "dest": "resources/k8s/CentOS_7.6",
+        "filename": "aarch64.tar.gz",
+        "sha256": "53a7790afa41981eb9aafa998eb50a1226084bb289d8ad3998da94d213f2c58c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/aarch64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64.tar.gz",
         "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz"
     },
     {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
+        "dest": "resources/k8s/CentOS_7.6",
+        "filename": "aarch64_125.tar.gz",
+        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/CentOS_7.6/aarch64_125.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz"
     },
     {
-        "dest": "resources/k8s/Ubuntu_18.04",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "9a539919c113beeae353a61342ad5cd9ad6ba4d96f7340671aa7901f377a7da8",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_18.04/aarch64_125.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/Ubuntu_18.04",
-        "filename": "aarch64.tar.gz",
-        "sha256": "b2fba0341e2b99d338580859d8877303af828bb442e277659a45f1ec152d6dca",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_18.04/aarch64.tar.gz"
-    },
-    {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-aarch64",
         "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-aarch64"
     },
     {
         "dest": "resources/tool/hccn",
+        "filename": "hccn-x86_64",
+        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
+    },
+    {
+        "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/Ubuntu_18.04",
+        "dest": "resources/docker/CentOS_7.6",
         "filename": "aarch64.tar.gz",
-        "sha256": "d3761acb25a39ba9ba89928e29a8f2c55b2d3fbd7d3e2149e8c469483a4bf5aa",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_18.04/aarch64.tar.gz"
+        "sha256": "ca7e176d6fb4092daa3c737b2b5ecfef0586a96b77e83d1720f05da5d58e8d54",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/CentOS_7.6/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_x86_64.json`

 * *Files 12% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[12, 0]'}*

```diff
@@ -1,15 +1,9 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
         "dest": "resources/basic/Ubuntu_18.04",
         "filename": "x86_64.tar.gz",
         "sha256": "bce1498d0cb2e8487ed7d9d37271ddb669fdd24d8f0b6a9c7b1f6ab11ea14fa3",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_18.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
@@ -68,19 +62,13 @@
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_aarch64.json`

 * *Files 20% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {'delete': '[12, 0]'}*

```diff
@@ -1,15 +1,9 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
         "dest": "resources/basic/Ubuntu_20.04",
         "filename": "aarch64.tar.gz",
         "sha256": "760abc2c443c0b847ecb0870b3c07703e612cdfb3971270d7d6cc9b9e6f9c701",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_20.04/aarch64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
@@ -68,19 +62,13 @@
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json` & `ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_x86_64.json`

 * *Files 19% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7589285714285714%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_22.04/x86_64.tar.gz', "*

 * *      "'sha256': '535e0d3ec59cf3690efc975be78a4ae2a4dd683d2ee3ce898e5a852b12f610d4', 'dest': "*

 * *      "'resources/basic/Ubuntu_22.04'}",*

 * * '3': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/x86_64.tar.gz', "*

 * *      "'sha256': '734e7f55654e433e6dad5749e761bfbc4809cd2fedfd7720290fe6ac528a2a46', 'dest': "*

 * *      […]*

```diff
@@ -1,49 +1,43 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/Ubuntu_20.04",
+        "dest": "resources/basic/Ubuntu_22.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "51e05d46e794179fd343e7e1578df0e487da71d092ed6e5c82085d2950709ad1",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_20.04/x86_64.tar.gz"
+        "sha256": "535e0d3ec59cf3690efc975be78a4ae2a4dd683d2ee3ce898e5a852b12f610d4",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_22.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64.tar.gz",
         "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64.tar.gz"
     },
     {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/Ubuntu_20.04",
+        "dest": "resources/k8s/Ubuntu_22.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "889b7f69b812b4b92767964296473466616899db48474ac47cae0c7382facac9",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_20.04/x86_64.tar.gz"
+        "sha256": "734e7f55654e433e6dad5749e761bfbc4809cd2fedfd7720290fe6ac528a2a46",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "x86_64_125.tar.gz",
         "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
-        "dest": "resources/k8s/Ubuntu_20.04",
+        "dest": "resources/k8s/Ubuntu_22.04",
         "filename": "x86_64_125.tar.gz",
         "sha256": "33507c061fd2dcdb9357d3e1253b922779a2ddc8faf7cb7620134091f94b4284",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_20.04/x86_64_125.tar.gz"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/x86_64_125.tar.gz"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
     },
@@ -56,31 +50,25 @@
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/docker/Ubuntu_20.04",
+        "dest": "resources/docker/Ubuntu_22.04",
         "filename": "x86_64.tar.gz",
-        "sha256": "fc3d51e849a79bc3332acf0e493e1ad0aabad3e705f8a299c0630c32021c5c91",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_20.04/x86_64.tar.gz"
+        "sha256": "e3f7e79931aa249fd4e7f98ae38716b40d8033356841d6d87fb8db98b0a135a8",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_22.04/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
     },
     {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
-    },
-    {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json` & `ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_x86_64.json`

 * *Files 22% similar despite different names*

### Pretty-printed

 * *Similarity: 0.5982142857142857%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json', "*

 * *      "'sha256': '84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f'}",*

 * * '1': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml'}",*

 * * '2': "{'filename': 'hccn-aarch64', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64', "*

 * *      "'sha25 […]*

```diff
@@ -1,85 +1,67 @@
 [
     {
         "dest": "resources",
         "filename": "version.json",
-        "sha256": "71ca707dc902abf22a0d6137c59af487793080d440cd46d4ecf443d41d3dadff",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/version.json"
-    },
-    {
-        "dest": "resources/basic/Ubuntu_22.04",
-        "filename": "x86_64.tar.gz",
-        "sha256": "535e0d3ec59cf3690efc975be78a4ae2a4dd683d2ee3ce898e5a852b12f610d4",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/basic/Ubuntu_22.04/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/image",
-        "filename": "x86_64.tar.gz",
-        "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64.tar.gz"
+        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
     },
     {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/Ubuntu_22.04",
-        "filename": "x86_64.tar.gz",
-        "sha256": "734e7f55654e433e6dad5749e761bfbc4809cd2fedfd7720290fe6ac528a2a46",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/x86_64.tar.gz"
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-aarch64",
+        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/k8s/image",
+        "dest": "resources/k8s/CTyunOS_22.06",
         "filename": "x86_64_125.tar.gz",
-        "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/x86_64_125.tar.gz"
+        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/x86_64_125.tar.gz"
     },
     {
-        "dest": "resources/k8s/Ubuntu_22.04",
+        "dest": "resources/k8s/image",
         "filename": "x86_64_125.tar.gz",
-        "sha256": "33507c061fd2dcdb9357d3e1253b922779a2ddc8faf7cb7620134091f94b4284",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/Ubuntu_22.04/x86_64_125.tar.gz"
-    },
-    {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-aarch64",
-        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-aarch64"
+        "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
         "dest": "resources/tool/report",
         "filename": "k8s_status_report-x86_64",
         "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/report/k8s_status_report-x86_64"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-x86_64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/hccn/hccn-x86_64"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/docker/Ubuntu_22.04",
+        "dest": "resources/docker/CTyunOS_22.06",
         "filename": "x86_64.tar.gz",
-        "sha256": "e3f7e79931aa249fd4e7f98ae38716b40d8033356841d6d87fb8db98b0a135a8",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/docker/Ubuntu_22.04/x86_64.tar.gz"
+        "sha256": "4ee3ce4e5a039a1274a460b0ff60a87909d61902c78731a748e47a49e454ab94",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/OpenEuler_20.03_LTS/01/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-x86_64",
         "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-x86_64"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-x86_64"
     },
     {
         "dest": "resources/k8s",
         "filename": "version.json",
-        "sha256": "4e0f51efea5b490accc177fdfbf96d7bf0309a00b73ecb727266f33393c152fb",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/version.json"
+        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
     },
     {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
         "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_aarch64/resource.json` & `ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_aarch64.json`

 * *Files identical despite different names*

## Comparing `ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_x86_64/resource.json` & `ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_x86_64.json`

 * *Files identical despite different names*

## Comparing `ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_aarch64/resource.json` & `ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_x86_64.json`

 * *Files 23% similar despite different names*

### Pretty-printed

 * *Similarity: 0.5357142857142857%*

 * *Differences: {'1': "{'filename': 'calico_v3.25.0.yaml', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml', "*

 * *      "'sha256': '0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110', 'dest': "*

 * *      "'resources/templates'}",*

 * * '10': "{'filename': 'nerdctl-1.4.0-linux-amd64.tar.gz', 'url': "*

 * *       "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz', "*

 * *       "'sha256': 'd […]*

```diff
@@ -2,85 +2,67 @@
     {
         "dest": "resources",
         "filename": "version.json",
         "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
     },
     {
-        "dest": "resources/basic/CentOS_7.6",
-        "filename": "aarch64.tar.gz",
-        "sha256": "b45569ca4cf608a757d7297b0f1188e0badbc9308c83fc793ba097682cdd26a9",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/basic/CentOS_7.6/aarch64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "aarch64.tar.gz",
-        "sha256": "53a7790afa41981eb9aafa998eb50a1226084bb289d8ad3998da94d213f2c58c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/CentOS_7.6/aarch64.tar.gz"
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/image",
-        "filename": "aarch64.tar.gz",
-        "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64.tar.gz"
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-aarch64",
+        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/CentOS_7.6/aarch64_125.tar.gz"
+        "dest": "resources/k8s/CTyunOS_22.06",
+        "filename": "x86_64_125.tar.gz",
+        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/x86_64_125.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64_125.tar.gz"
+        "filename": "x86_64_125.tar.gz",
+        "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/x86_64_125.tar.gz"
     },
     {
         "dest": "resources/tool/report",
-        "filename": "k8s_status_report-aarch64",
-        "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-aarch64"
+        "filename": "k8s_status_report-x86_64",
+        "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-x86_64"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-aarch64",
-        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
-    },
-    {
-        "dest": "resources/docker/CentOS_7.6",
-        "filename": "aarch64.tar.gz",
-        "sha256": "ca7e176d6fb4092daa3c737b2b5ecfef0586a96b77e83d1720f05da5d58e8d54",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/CentOS_7.6/aarch64.tar.gz"
+        "dest": "resources/docker/CTyunOS_22.06",
+        "filename": "x86_64.tar.gz",
+        "sha256": "4ee3ce4e5a039a1274a460b0ff60a87909d61902c78731a748e47a49e454ab94",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/OpenEuler_20.03_LTS/01/x86_64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
-        "filename": "docker-aarch64",
-        "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-aarch64"
-    },
-    {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
+        "filename": "docker-x86_64",
+        "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-x86_64"
     },
     {
         "dest": "resources/k8s",
         "filename": "version.json",
         "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
     },
     {
         "dest": "resources/tool",
-        "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
-        "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
+        "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
+        "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_x86_64/resource.json` & `ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_aarch64.json`

 * *Files 27% similar despite different names*

### Pretty-printed

 * *Similarity: 0.5178571428571429%*

 * *Differences: {'1': "{'filename': 'calico_v3.25.0.yaml', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml', "*

 * *      "'sha256': '0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110', 'dest': "*

 * *      "'resources/templates'}",*

 * * '10': "{'filename': 'nerdctl-1.4.0-linux-arm64.tar.gz', 'url': "*

 * *       "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz', "*

 * *       "'sha256': '0 […]*

```diff
@@ -2,85 +2,67 @@
     {
         "dest": "resources",
         "filename": "version.json",
         "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
     },
     {
-        "dest": "resources/basic/CentOS_7.6",
-        "filename": "x86_64.tar.gz",
-        "sha256": "d60a97c169d92dcb33e34c6c7ecf93cbf8e03c3893bc01540a8e2ce9fe772ddc",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/basic/CentOS_7.6/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "x86_64.tar.gz",
-        "sha256": "5659e7b8bb1afdb1e32385083ba84ada396f94316942d2bce3e0ac6ba753c47a",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/CentOS_7.6/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/image",
-        "filename": "x86_64.tar.gz",
-        "sha256": "d31d1f546055cbbf18ad13001b84e20f66418fc462300a2a6ab78fdd9309ef7d",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/x86_64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/CentOS_7.6",
-        "filename": "x86_64_125.tar.gz",
-        "sha256": "44cda0e87e0c56a00d066279a7638613d0716821aa2a639a0ec1dd46cc61cc53",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/CentOS_7.6/x86_64_125.tar.gz"
-    },
-    {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/image",
-        "filename": "x86_64_125.tar.gz",
-        "sha256": "c91bf681fa21a8f72def91ad78333379352a87000f2396e441ecd8dc6b3dc8f3",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/x86_64_125.tar.gz"
+        "dest": "resources/tool/hccn",
+        "filename": "hccn-x86_64",
+        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-aarch64",
-        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
+        "dest": "resources/k8s/CTyunOS_22.06",
+        "filename": "aarch64_125.tar.gz",
+        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/aarch64_125.tar.gz"
+    },
+    {
+        "dest": "resources/k8s/image",
+        "filename": "aarch64_125.tar.gz",
+        "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64_125.tar.gz"
     },
     {
         "dest": "resources/tool/report",
-        "filename": "k8s_status_report-x86_64",
-        "sha256": "062ee2c028cdb28964c98b6da50d9c95c9ac65c8424c458b8a2d10db2d6c2f5c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-x86_64"
+        "filename": "k8s_status_report-aarch64",
+        "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-aarch64"
     },
     {
         "dest": "resources/tool/hccn",
-        "filename": "hccn-x86_64",
-        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
+        "filename": "hccn-aarch64",
+        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/CentOS_7.6",
-        "filename": "x86_64.tar.gz",
-        "sha256": "59788bffd89e4e03c95cf7a7e048dba3d88a147abaaa4d0cc9e3454e0fbd1420",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/CentOS_7.6/x86_64.tar.gz"
+        "dest": "resources/docker/CTyunOS_22.06",
+        "filename": "aarch64.tar.gz",
+        "sha256": "149b1a9986ce7e3e175f73005b51ee3286776fa0fbb137485cd134e23218f2bf",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/OpenEuler_20.03_LTS/01/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
-        "filename": "docker-x86_64",
-        "sha256": "41ce1d1306ae9776d09d3286e90e2124b9acd51860f6405414a52144027fde47",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-x86_64"
+        "filename": "docker-aarch64",
+        "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-aarch64"
     },
     {
         "dest": "resources/k8s",
         "filename": "version.json",
         "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
     },
     {
         "dest": "resources/tool",
-        "filename": "nerdctl-1.4.0-linux-amd64.tar.gz",
-        "sha256": "d8dcd4e270ae76ab294be3a451a2d8299010e69dce6ae559bc3193535610e4cc",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-amd64.tar.gz"
+        "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
+        "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
 ]
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json` & `ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_aarch64.json`

 * *Files 19% similar despite different names*

### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {'1': "{'filename': 'calico_v3.25.0.yaml', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml', "*

 * *      "'sha256': '0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110', 'dest': "*

 * *      "'resources/templates'}",*

 * * '3': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/aarch64_125.tar.gz', "*

 * *      "'dest': 'resources/k8s/CTyunOS_22.06'}",*

 * * '7': "{'url': "*

 * * […]*

```diff
@@ -2,48 +2,30 @@
     {
         "dest": "resources",
         "filename": "version.json",
         "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
     },
     {
-        "dest": "resources/basic/Kylin_V10",
-        "filename": "aarch64.tar.gz",
-        "sha256": "5b12caba5d2b90820716af394d48268964777accaeac5a98f6b657fb9dc6abf5",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/basic/Kylin_V10/aarch64.tar.gz"
+        "dest": "resources/templates",
+        "filename": "calico_v3.25.0.yaml",
+        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
     },
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-x86_64",
         "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
     },
     {
-        "dest": "resources/k8s/Kylin_V10",
-        "filename": "aarch64.tar.gz",
-        "sha256": "e35c4d06bb3d81c7bba91bd3c70032f1eaa5d4649c0ce4bd89231a9b13a87c51",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/Kylin_V10/aarch64.tar.gz"
-    },
-    {
-        "dest": "resources/k8s/image",
-        "filename": "aarch64.tar.gz",
-        "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64.tar.gz"
-    },
-    {
-        "dest": "resources/templates",
-        "filename": "calico_v3.25.0.yaml",
-        "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
-    },
-    {
-        "dest": "resources/k8s/Kylin_V10",
+        "dest": "resources/k8s/CTyunOS_22.06",
         "filename": "aarch64_125.tar.gz",
         "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/Kylin_V10/aarch64_125.tar.gz"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/aarch64_125.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64_125.tar.gz"
     },
@@ -56,18 +38,18 @@
     {
         "dest": "resources/tool/hccn",
         "filename": "hccn-aarch64",
         "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
     },
     {
-        "dest": "resources/docker/Kylin_V10",
+        "dest": "resources/docker/CTyunOS_22.06",
         "filename": "aarch64.tar.gz",
-        "sha256": "f33ba8b8bb240449b87f627a4a287cc811783f6401c9ff12f4b909988a6ecb58",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/Kylin_V10/aarch64.tar.gz"
+        "sha256": "149b1a9986ce7e3e175f73005b51ee3286776fa0fbb137485cd134e23218f2bf",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/OpenEuler_20.03_LTS/01/aarch64.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-aarch64"
     },
```

## Comparing `ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_aarch64/resource.json` & `ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/UOS_20-1050e_aarch64.json`

 * *Files 27% similar despite different names*

### Pretty-printed

 * *Similarity: 0.375%*

 * *Differences: {'0': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml'}",*

 * * '1': "{'filename': 'aarch64.tar.gz', 'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz', "*

 * *      "'sha256': '0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73', 'dest': "*

 * *      "'resources/k8s/image'}",*

 * * '2': "{'url': "*

 * *      "'https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0. […]*

```diff
@@ -1,67 +1,31 @@
 [
     {
-        "dest": "resources",
-        "filename": "version.json",
-        "sha256": "84ed289713bfea135bdd3e19c7f17e1495714351758e2fe3428cf323ff28f10f",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/version.json"
-    },
-    {
         "dest": "resources/templates",
         "filename": "calico_v3.25.0.yaml",
         "sha256": "0b642c65295d7d80af8600da87e1d8092433f8e25a71f2444cb0e26a301e8110",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/templates/calico_v3.25.0.yaml"
-    },
-    {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-x86_64",
-        "sha256": "66cd8d314b004e9e77600567beaa2384e427a2e0d05921b036b197b03529f0d0",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-x86_64"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/templates/calico_v3.25.0.yaml"
     },
     {
-        "dest": "resources/k8s/CTyunOS_22.06",
-        "filename": "aarch64_125.tar.gz",
-        "sha256": "8a1f2d7aeedfb87c33f4e5b4d3760642a5877c9307b16bcd2dcc4ef252f6bbef",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/OpenEuler_20.03_LTS/aarch64_125.tar.gz"
+        "dest": "resources/k8s/image",
+        "filename": "aarch64.tar.gz",
+        "sha256": "0140e5d3ae7d482db7d4007dd686a727318d7bb59a87986b1101f047efae4e73",
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64.tar.gz"
     },
     {
         "dest": "resources/k8s/image",
         "filename": "aarch64_125.tar.gz",
         "sha256": "453a2d9d56e25a6d9cf4410b1056e639e0421ba3dffd333443ec8d4497f2e17b",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/image/aarch64_125.tar.gz"
-    },
-    {
-        "dest": "resources/tool/report",
-        "filename": "k8s_status_report-aarch64",
-        "sha256": "39fd4d21f25f247c9880c7dba8fb8f71693da0dc162e308852b37f87da2c0f3f",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/report/k8s_status_report-aarch64"
-    },
-    {
-        "dest": "resources/tool/hccn",
-        "filename": "hccn-aarch64",
-        "sha256": "1a8a8819150fb3f7c1558155062ae83c073562eb7768ceb5dfc2d1b8d00f860c",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/tool/hccn/hccn-aarch64"
-    },
-    {
-        "dest": "resources/docker/CTyunOS_22.06",
-        "filename": "aarch64.tar.gz",
-        "sha256": "149b1a9986ce7e3e175f73005b51ee3286776fa0fbb137485cd134e23218f2bf",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/docker/OpenEuler_20.03_LTS/01/aarch64.tar.gz"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/k8s/image/aarch64_125.tar.gz"
     },
     {
         "dest": "resources/do-not-change",
         "filename": "docker-aarch64",
         "sha256": "8f91a544c72c77ae1aac237697b07304bbdced1a75abc3517b3ee24d46d55b6a",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/do-not-change/docker-aarch64"
-    },
-    {
-        "dest": "resources/k8s",
-        "filename": "version.json",
-        "sha256": "e06716192511de8fd9389c71b17f331a3a75ff7a0352892b8ec097cc8be9f68a",
-        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC2/resources/k8s/version.json"
+        "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/do-not-change/docker-aarch64"
     },
     {
         "dest": "resources/tool",
         "filename": "nerdctl-1.4.0-linux-arm64.tar.gz",
         "sha256": "0edb064a7d68d0425152ed59472ce7566700b4e547afb300481498d4c7fc6cf1",
         "url": "https://ascend-repo-modelzoo.obs.myhuaweicloud.com/MindXDL/5.0.RC1/resources/tool/nerdctl-1.4.0-linux-arm64.tar.gz"
     }
```

## Comparing `ascend_deployer/playbooks/roles/mindx.dl/templates/drc.conf` & `ascend_deployer/templates/mindio/drc.conf`

 * *Files identical despite different names*

## Comparing `ascend_deployer/playbooks/roles/mindx.dl/templates/memfs.conf` & `ascend_deployer/templates/mindio/memfs.conf`

 * *Files identical despite different names*

## Comparing `ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py` & `ascend_deployer/scripts/create_report.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #!/usr/bin/env python3
 # coding: utf-8
-# Copyright 2023 Huawei Technologies Co., Ltd
+# Copyright 2024 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
+import glob
 import json
-import csv
-import os.path
+import os
 import sys
+import csv
+
+from ansible.inventory.manager import InventoryManager
+from ansible.parsing.dataloader import DataLoader
 
 
 def solve_value_list(value_list):
     res_iter = (item.get("name", "") + ":" + item.get("version", "") for item in value_list if isinstance(item, dict))
     return "\n".join(res_iter)
 
 
@@ -30,38 +34,74 @@
         return 'NA'
     for hccn in hccn_list:
         if isinstance(hccn, str) and 'success' not in hccn.lower():
             return 'fail'
     return 'ok'
 
 
-def main(path):
-    with open(path) as f:
-        data = json.load(f)
-        dir_name = os.path.dirname(path)
-        ips = list(data.keys())
-
-        fieldsname = ["IP", "Node name", "Node type", "Node status", "Npu numbers", "Software package version",
-                      "HCCN health check", "Running pods", "MindX-DL status"]
-        flags = os.O_WRONLY | os.O_CREAT
-        with os.fdopen(os.open(dir_name + '/report.csv', flags, 0o644), 'w', newline='') as wf:
-            writer = csv.DictWriter(wf, fieldnames=fieldsname)
-            writer.writeheader()
-            for ip in ips:
-                row = [ip]
-                npu = data.get(ip, {}).get('npu', 'NA')
-                packages = solve_value_list(data.get(ip, {}).get('packages', []))
-                hccn_list = data.get(ip, {}).get('hccn', [])
-                hccn_info = get_hccn(hccn_list)
-                node_name = data.get(ip, {}).get('node name', 'NA')
-                node_type = data.get(ip, {}).get('node type', 'NA')
-                status = data.get(ip, {}).get('status', 'NA')
-                ready_pods = "\n".join(data.get(ip, {}).get('ready pods', []))
-                result = data.get(ip, {}).get('dl result', 'NA')
-                row.extend(
-                    [node_name, node_type, status, npu, packages or 'NA', hccn_info, ready_pods or 'NA',
-                     result or 'NA'])
-                writer.writerow(dict(zip(fieldsname, row)))
+def write_csv(merged_data, dir_name):
+    ips = list(merged_data.keys())
+
+    field_names = ["IP", "Node name", "Node type", "Node status", "Npu numbers", "Software package version",
+                   "HCCN health check", "Running pods", "MindX-DL status"]
+    flags = os.O_WRONLY | os.O_CREAT
+    with os.fdopen(os.open(dir_name + '/report.csv', flags, 0o644), 'w') as wf:
+        writer = csv.DictWriter(wf, fieldnames=field_names)
+        writer.writeheader()
+        for ip in ips:
+            row = [ip]
+            npu = merged_data.get(ip, {}).get('npu', 'NA')
+            packages = solve_value_list(merged_data.get(ip, {}).get('packages', []))
+            hccn_list = merged_data.get(ip, {}).get('hccn', [])
+            hccn_info = get_hccn(hccn_list)
+            node_name = merged_data.get(ip, {}).get('node name', 'NA')
+            node_type = merged_data.get(ip, {}).get('node type', 'NA')
+            status = merged_data.get(ip, {}).get('status', 'NA')
+            ready_pods = "\n".join(merged_data.get(ip, {}).get('ready pods', []))
+            result = merged_data.get(ip, {}).get('dl result', 'NA')
+            row.extend(
+                [node_name, node_type, status, npu, packages or 'NA', hccn_info, ready_pods or 'NA',
+                 result or 'NA'])
+            writer.writerow(dict(zip(field_names, row)))
+
+
+def main(jsons_path, output_path, inventory_file_path):
+    inventory = InventoryManager(loader=DataLoader(), sources=[inventory_file_path, ], parse=True)
+    workers = inventory.get_hosts(pattern='worker')
+    masters = inventory.get_hosts(pattern='master')
+    all_hosts = set(workers + masters)
+
+    json_files = []
+    for parent, _, files in os.walk(jsons_path):
+        for file in files:
+            if file.endswith(".json"):
+                json_files.append(os.path.join(parent, file))
+    merged_data = {}
+    localhost_data = {}
+    for file in json_files:
+        with open(file, 'r') as f:
+            data = json.load(f)
+            for ip in data.keys():
+                data_value = data.get(ip, {})
+                if ip == 'localhost':
+                    localhost_data.update(data_value)
+                    continue
+                merged_data.setdefault(ip, {}).update(data_value)
+    if localhost_data and len(merged_data) == 0:
+        merged_data['localhost'] = localhost_data
+
+    for host in all_hosts:
+        if str(host) not in merged_data and str(host) != 'localhost':
+            merged_data[str(host)] = {}
+
+    flags = os.O_WRONLY | os.O_CREAT
+    with os.fdopen(os.open(output_path + '/report.json', flags, 0o644), 'w') as f:
+        json.dump(merged_data, f)
+
+    write_csv(merged_data, output_path)
 
 
 if __name__ == '__main__':
-    main(sys.argv[1])
+    from_path = sys.argv[1]
+    to_path = sys.argv[2]
+    inventory_file = sys.argv[3]
+    main(from_path, to_path, inventory_file)
```

## Comparing `ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py` & `ascend_deployer/scripts/k8s_rep.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,226 +1,258 @@
-#!/usr/bin/env python3
-# coding: utf-8
-# Copyright 2023 Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ===========================================================================firmware_ver
-import os.path
-import subprocess
-import json
-import sys
-from collections import OrderedDict
-
-require_by_all = ["calico-node", "kube-proxy", ]
-master_by_scene = {'1': ["etcd", "kube-apiserver", "kube-controller-manager", "kube-scheduler"],
-                   '2': ["etcd", "kube-apiserver", "kube-scheduler"],
-                   '3': ["etcd", "kube-apiserver", "kube-scheduler"],
-                   '4': ["etcd", "kube-apiserver", "kube-controller-manager", "kube-scheduler", "ascend-cert",
-                         "ascend-edge", "ascend-ngnix"]
-                   }
-
-all_master_together_by_scene = {'1': ["calico-kube-controllers", "coredns", "hccl-controller", "ascend-operator",
-                                      "resilience-controller", "volcano-scheduler", "volcano-controllers"],
-                                '2': ["calico-kube-controllers", "coredns",
-                                      "volcano-scheduler", "volcano-controllers", ],
-                                '3': ["calico-kube-controllers", "coredns"],
-                                '4': ["calico-kube-controllers", "coredns"]
-                                }
-
-worker_by_scene = {
-    '1': ["ascend-device-plugin", "noded", "npu-exporter", ],
-    '2': ["ascend-device-plugin", ],
-    '3': ["ascend-device-plugin", ]
-}
-
-
-def get_nodes_info():
-    result = subprocess.check_output(['kubectl', 'get', 'nodes', '-o', 'json'], encoding="utf-8")
-    nodes_info = json.loads(result)
-    k8s_node = {}
-    for node_json in nodes_info.get("items", {}):
-        node = K8sNode(**node_json)
-        ip_address = node.get_ip()
-        property_dict = OrderedDict()
-        property_dict['node name'] = node.get_name()
-        property_dict['node type'] = node.get_type()
-        property_dict['status'] = node.get_status()
-        k8s_node[ip_address] = property_dict
-    return k8s_node
-
-
-def get_pods_info(nodes_dict):
-    result = subprocess.check_output(['kubectl', 'get', 'pods', '-A', '-o', 'json'], encoding="utf-8")
-    pods_info = json.loads(result)
-    for pod_json in pods_info.get("items", {}):
-        pod = K8sPod(**pod_json)
-        ip = pod.get_ip()
-        property_dict = nodes_dict.get(ip, {})
-        name = pod.get_name()
-        if pod.get_status():
-            property_dict.setdefault('ready pods', [])
-            property_dict.get('ready pods', []).append(name)
-        else:
-            property_dict.setdefault('failed pods', [])
-            property_dict.get('failed pods', []).append(name)
-
-    return nodes_dict
-
-
-def check_if_missing(info, require_list):
-    already_pods = info.get("ready pods", [])
-    for require_pod in require_list:
-        flag = False
-        for ready_pod in already_pods:
-            if ready_pod.startswith(require_pod):
-                flag = True
-                break
-        if not flag:
-            info.get("missing pods", []).append(require_pod)
-
-
-def missing_add_to_all_master(temp_dict, node_dict):
-    for ip, info in node_dict.items():
-        character = info.get("node type", "")
-        if "master" in character:
-            info.get("missing pods", []).extend(temp_dict.get("missing pods", []))
-
-
-def check_missing_pods(node_dict, scene):
-    all_master_pods = []
-    for ip, info in node_dict.items():
-        check_if_missing(info, require_by_all)
-        character = info.get("node type", "")
-        if "master" in character:
-            require_list = master_by_scene.get(scene, [])
-            check_if_missing(info, require_list)
-            all_master_pods.extend(info.get("ready pods", []))
-        if "worker" in character:
-            require_list = worker_by_scene.get(scene, [])
-            check_if_missing(info, require_list)
-    temp_dict = {"ready pods": all_master_pods}
-    check_if_missing(temp_dict, all_master_together_by_scene.get(scene, []))
-    missing_add_to_all_master(temp_dict, node_dict)
-    return node_dict
-
-
-def is_dl_success(node_dict):
-    for ip, info in node_dict.items():
-        if info.get("status", "") != "Ready":
-            return False
-        if len(info.get("missing pods", [])) > 0:
-            return False
-        if len(info.get("failed pods", [])) > 0:
-            return False
-    return True
-
-
-def append_result(node_dict, result):
-    for ip, info in node_dict.items():
-        info.setdefault("dl result", result)
-
-
-class K8sPod:
-    def __init__(self, status=None, metadata=None, **kwargs):
-        self.status = PodStatus(**status)
-        self.metadata = metadata
-
-    def get_ip(self):
-        return self.status.host_ip or ''
-
-    def get_name(self):
-        if isinstance(self.metadata, dict) and 'name' in self.metadata:
-            return self.metadata.get('name', '')
-        return ''
-
-    def get_status(self):
-        if self.status.container_statuses:
-            return self.status.container_statuses[0].get('ready', False)
-        return False
-
-
-class PodStatus:
-    def __init__(self, **kwargs):
-        self.host_ip = kwargs.get('hostIP')
-        self.container_statuses = kwargs.get('containerStatuses')
-
-
-class K8sNode:
-    def __init__(self, status=None, metadata=None, **kwargs):
-        self.status = NodeStatus(**status)
-        self.metadata = MetaData(**metadata)
-
-    def get_ip(self):
-        if self.status.addresses:
-            return self.status.addresses[0].get('address', 'NA')
-        return ''
-
-    def get_name(self):
-        if self.status.addresses:
-            return self.status.addresses[1].get('address', 'NA')
-        return ''
-
-    def get_type(self):
-        if self.metadata.labels.get("masterselector") and self.metadata.labels.get("workerselector"):
-            return "master,worker"
-        elif self.metadata.labels.get("masterselector"):
-            return "master"
-        elif self.metadata.labels.get("workerselector"):
-            return "worker"
-        else:
-            return ''
-
-    def get_status(self):
-        if isinstance(self.status.conditions, list) and len(self.status.conditions) >= 2:
-            return self.status.conditions[-1].get("type", "")
-        return ''
-
-    def get_npu(self):
-        devices = []
-        for key, value in self.status.capacity.items():
-            if "huawei" in key:
-                devices.append("%s:%s" % (key, value))
-        return devices
-
-
-class MetaData:
-    def __init__(self, labels=None, **kwargs):
-        self.labels = labels
-
-
-class NodeStatus:
-    def __init__(self, addresses=None, capacity=None, conditions=None, **kwargs):
-        if not isinstance(addresses, list) or len(addresses) < 2:
-            raise Exception('json format error, wrong address: %s' % str(addresses))
-        self.addresses = addresses
-        self.capacity = capacity
-        self.conditions = conditions
-
-
-def main(path_name, scene):
-    node_dict = get_nodes_info()
-    node_dict = get_pods_info(node_dict)
-    node_dict = check_missing_pods(node_dict, scene)
-    if is_dl_success(node_dict):
-        append_result(node_dict, "success")
-    else:
-        append_result(node_dict, "failed")
-    if os.path.isdir(path_name):
-        flags = os.O_WRONLY | os.O_CREAT
-        with os.fdopen(os.open(os.path.join(path_name, 'node_dict.json'), flags, 0o700), 'w', newline='') as f:
-            json.dump(node_dict, f)
-
-
-if __name__ == '__main__':
-    path = sys.argv[1]
-    scene_num = sys.argv[2]
-    main(path, scene_num)
+#!/usr/bin/env python3
+# coding: utf-8
+# Copyright 2023 Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ===========================================================================firmware_ver
+import os.path
+import subprocess
+import json
+import sys
+import time
+from collections import OrderedDict
+
+require_by_all = ["calico-node", "kube-proxy", ]
+master_by_scene = {'1': ["etcd", "kube-apiserver", "kube-controller-manager", "kube-scheduler"],
+                   '2': ["etcd", "kube-apiserver", "kube-scheduler"],
+                   '3': ["etcd", "kube-apiserver", "kube-scheduler"],
+                   '4': ["etcd", "kube-apiserver", "kube-controller-manager", "kube-scheduler", "ascend-cert",
+                         "ascend-edge", "ascend-ngnix"]
+                   }
+
+all_master_together_by_scene = {'1': ["calico-kube-controllers", "coredns", "hccl-controller", "ascend-operator",
+                                      "resilience-controller", "volcano-scheduler", "volcano-controllers"],
+                                '2': ["calico-kube-controllers", "coredns",
+                                      "volcano-scheduler", "volcano-controllers", ],
+                                '3': ["calico-kube-controllers", "coredns"],
+                                '4': ["calico-kube-controllers", "coredns"]
+                                }
+
+worker_by_scene = {
+    '1': ["ascend-device-plugin", "noded", "npu-exporter", ],
+    '2': ["ascend-device-plugin", ],
+    '3': ["ascend-device-plugin", ]
+}
+
+
+def get_nodes_info():
+    result = subprocess.check_output(['kubectl', 'get', 'nodes', '-o', 'json'])
+    nodes_info = json.loads(result)
+    k8s_node = {}
+    for node_json in nodes_info.get("items", {}):
+        node = K8sNode(**node_json)
+        ip_address = node.get_ip()
+        property_dict = OrderedDict()
+        property_dict['node name'] = node.get_name()
+        property_dict['node type'] = node.get_type()
+        property_dict['status'] = node.get_status()
+        k8s_node[ip_address] = property_dict
+    return k8s_node
+
+
+def get_pods_info(nodes_dict):
+    result = subprocess.check_output(['kubectl', 'get', 'pods', '-A', '-o', 'json'])
+    pods_info = json.loads(result)
+    for pod_json in pods_info.get("items", {}):
+        pod = K8sPod(**pod_json)
+        ip = pod.get_ip()
+        property_dict = nodes_dict.get(ip, {})
+        name = pod.get_name()
+        if pod.get_status():
+            property_dict.setdefault('ready pods', [])
+            property_dict.get('ready pods', []).append(name)
+        else:
+            property_dict.setdefault('failed pods', [])
+            property_dict.get('failed pods', []).append(name)
+
+    return nodes_dict
+
+
+def update_missing_pods(info, require_list):
+    already_pods = info.get("ready pods", [])
+    missing_pods = info.get("missing pods", [])
+    for require_pod in require_list:
+        flag = False
+        for ready_pod in already_pods:
+            if ready_pod.startswith(require_pod):
+                flag = True
+                break
+        if not flag:
+            missing_pods.append(require_pod)
+            info["missing pods"] = missing_pods
+    return info
+
+
+def missing_add_to_all_master(temp_dict, node_dict):
+    for _, info in node_dict.items():
+        character = info.get("node type", "")
+        if "master" in character:
+            info.get("missing pods", []).extend(temp_dict.get("missing pods", []))
+
+
+def check_missing_pods(node_dict, scene):
+    all_master_pods = []
+    for ip, info in node_dict.items():
+        info = update_missing_pods(info, require_by_all)
+        character = info.get("node type", "")
+        if "master" in character:
+            require_list = master_by_scene.get(scene, [])
+            node_dict[ip] = update_missing_pods(info, require_list)
+            all_master_pods.extend(info.get("ready pods", []))
+        if "worker" in character:
+            require_list = worker_by_scene.get(scene, [])
+            node_dict[ip] = update_missing_pods(info, require_list)
+    temp_dict = {"ready pods": all_master_pods}
+    temp_dict = update_missing_pods(temp_dict, all_master_together_by_scene.get(scene, []))
+    missing_add_to_all_master(temp_dict, node_dict)
+    return node_dict
+
+
+def is_dl_success(node_dict):
+    for _, info in node_dict.items():
+        if info.get("status", "") != "Ready":
+            return False
+        if len(info.get("missing pods", [])) > 0:
+            return False
+        if len(info.get("failed pods", [])) > 0:
+            return False
+    return True
+
+
+def append_result(node_dict, result):
+    for _, info in node_dict.items():
+        info.setdefault("dl result", result)
+
+
+def is_all_pods_ready():
+    try:
+        result = subprocess.check_output(['kubectl', 'get', 'pods', '-A', '-o', 'json'])
+    except Exception as err:
+        print(err)
+        return False
+    pods_info = json.loads(result)
+    for pod_json in pods_info.get("items", {}):
+        pod = K8sPod(**pod_json)
+        if not pod.get_status():
+            return False
+    return True
+
+
+class K8sPod:
+    def __init__(self, status=None, metadata=None, **kwargs):
+        self.status = PodStatus(**status)
+        self.metadata = metadata
+
+    def get_ip(self):
+        return self.status.host_ip or ''
+
+    def get_name(self):
+        if isinstance(self.metadata, dict) and 'name' in self.metadata:
+            return self.metadata.get('name', '')
+        return ''
+
+    def get_status(self):
+        if self.status.container_statuses:
+            return self.status.container_statuses[0].get('ready', False)
+        return False
+
+
+class PodStatus:
+    def __init__(self, **kwargs):
+        self.host_ip = kwargs.get('hostIP')
+        self.container_statuses = kwargs.get('containerStatuses')
+
+
+class K8sNode:
+    def __init__(self, status=None, metadata=None, **kwargs):
+        self.status = NodeStatus(**(status or {}))
+        self.metadata = MetaData(**(metadata or {}))
+
+    def get_ip(self):
+        if self.status.addresses:
+            return self.status.addresses[0].get('address', 'NA')
+        return ''
+
+    def get_name(self):
+        if self.status.addresses:
+            return self.status.addresses[1].get('address', 'NA')
+        return ''
+
+    def get_type(self):
+        if self.metadata.labels.get("masterselector") and self.metadata.labels.get("workerselector"):
+            return "master,worker"
+        elif self.metadata.labels.get("masterselector"):
+            return "master"
+        elif self.metadata.labels.get("workerselector"):
+            return "worker"
+        else:
+            return ''
+
+    def get_status(self):
+        if isinstance(self.status.conditions, list) and len(self.status.conditions) >= 2:
+            return self.status.conditions[-1].get("type", "")
+        return ''
+
+    def get_npu(self):
+        devices = []
+        for key, value in self.status.capacity.items():
+            if "huawei" in key:
+                devices.append("%s:%s" % (key, value))
+        return devices
+
+
+class MetaData:
+    def __init__(self, labels=None, **kwargs):
+        self.labels = labels
+
+
+class NodeStatus:
+    def __init__(self, addresses=None, capacity=None, conditions=None, **kwargs):
+        if not isinstance(addresses, list) or len(addresses) < 2:
+            raise Exception('json format error, wrong address: %s' % str(addresses))
+        self.addresses = addresses
+        self.capacity = capacity
+        self.conditions = conditions
+
+
+def main(path_name, scene):
+    path_name = os.path.realpath(os.path.expanduser(path_name))
+    if os.path.exists(os.path.join(path_name, 'node_dict.json')):
+        os.unlink(os.path.join(path_name, 'node_dict.json'))
+    node_dict = get_nodes_info()
+
+    try_times = 0
+    while try_times < 5:
+        if is_all_pods_ready():
+            break
+        try_times += 1
+        time.sleep(2)
+
+    node_dict = get_pods_info(node_dict)
+    node_dict = check_missing_pods(node_dict, scene)
+    if is_dl_success(node_dict):
+        append_result(node_dict, "success")
+    else:
+        append_result(node_dict, "failed")
+    if os.path.isdir(path_name):
+        flags = os.O_WRONLY | os.O_CREAT
+        with os.fdopen(os.open(os.path.join(path_name, 'node_dict.json'), flags, 0o700), 'w') as f:
+            json.dump(node_dict, f)
+
+
+if __name__ == '__main__':
+    path = sys.argv[1]
+    scene_num = sys.argv[2]
+    try:
+        main(path, scene_num)
+    except Exception as e:
+        print(e)
```

## Comparing `ascend_deployer-5.0.6.dist-info/LICENSE` & `ascend_deployer-6.0.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ascend_deployer-5.0.6.dist-info/METADATA` & `ascend_deployer-6.0.0b1.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,74 @@
-Metadata-Version: 2.1
-Name: ascend-deployer
-Version: 5.0.6
-Summary: ascend offline installer
-Home-page: https://gitee.com/ascend/ascend-deployer
-License: Apache
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >= 3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: NOTICE
-
-.. sectnum::
-
-简介
-=======
-
-离线安装工具提供系统组件、python第三方依赖自动下载以及一键式安装的功能，并支持驱动、固件、CANN软件包以及MindX DL和MindX Edge MEF Center的安装。
-
-快速指南
-===========
-
-本工具主要支持开局场景（环境仅安装了OS），如果遇到问题，请参考\ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\。
-
-安装内容
--------------
-
-工具支持安装的内容参考下图，其中红色部分是昇腾设备上必须安装的，橙色部分和绿色部分是可选安装的，如果需要直接运行AI框架或Toolbox，橙色部分也是必须安装的。
-
-.. image:: ./assets/1.png
-
-使用样例
--------------
-
-以下以Ubuntu_18.04_x86_64系统，服务器上插Atlas 300I Pro推理卡为例快速展示工具的使用方式。
-
-1. 以root用户登录待安装设备。
-   
-2. 执行 ``pip3 install ascend-deployer==<version>`` 安装ascend-deployer工具。<version>为ascend-deployer工具的版本号，
-   建议参考\ `官网 <https://pypi.org/project/ascend-deployer/#history>`__\下载最新发布版本的工具包。如果提示pip3命令不存在，请用户自行安装。
-
-3. 执行下载命令。
-   
-   ::
-
-      ascend-download --os-list=Ubuntu_18.04_x86_64 --download=CANN==6.3.RC1,MindSpore==2.0.0rc1
-
-   执行以上命令后，会自动下载好OS所需依赖，CANN软件包和配套的驱动和固件包，以及docker软件等，**并存放到$HOME/ascend-deployer/resources目录下**。
-
-4. 创建驱动的运行用户HwHiAiUser。
-
-   ::
-
-      groupadd HwHiAiUser
-      useradd -g HwHiAiUser -d /home/HwHiAiUser -m HwHiAiUser -s /bin/bash
-
-   创建完用户后，执行 ``passwd HwHiAiUser`` 命令设置用户密码。
-
-5. 安装驱动和固件时，如果不是归一包（包名以 **Ascend-hdk** 开头），需在inventory_file中提前配置cus_npu_info变量。
-   
-   ::
-
-      [ascend]
-      localhost ansible_connection='local'
-
-6. 执行以下安装命令，自动安装所有能找到的包（MindX DL和MEF Center除外，该两者请参考 \ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\）。
-   
-   ::
-
-      ascend-deployer --install-scene=auto
-
-7. 安装后配置。
-   使用python和CANN前，需要根据实际情况配置环境变量，以下内容以配置python和nnae的环境变量为例。
-
-   ::
-
-      source /usr/local/ascendrc                # 配置python环境变量
-      source /usr/local/Ascend/nnae/set_env.sh  # 配置nnae的环境变量
-
-8. 详细指南请参考\ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\
+Metadata-Version: 2.1
+Name: ascend-deployer
+Version: 6.0.0b1
+Summary: ascend offline installer
+Home-page: https://gitee.com/ascend/ascend-deployer
+License: Apache
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >= 3.6
+Description-Content-Type: text/x-rst
+
+.. sectnum::
+
+简介
+=======
+
+离线安装工具提供系统组件、python第三方依赖自动下载以及一键式安装的功能，并支持驱动、固件、CANN软件包以及MindX DL和MindX Edge MEF Center的安装。
+
+快速指南
+===========
+
+本工具主要支持开局场景（环境仅安装了OS），如果遇到问题，请参考\ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\。
+
+安装内容
+-------------
+
+工具支持安装的内容参考下图，其中红色部分是昇腾设备上必须安装的，橙色部分和绿色部分是可选安装的，如果需要直接运行AI框架或Toolbox，橙色部分也是必须安装的。
+
+.. image:: ./assets/1.png
+
+使用样例
+-------------
+
+以下以Ubuntu_18.04_x86_64系统，服务器上插Atlas 300I Pro推理卡为例快速展示工具的使用方式。
+
+1. 以root用户登录待安装设备。
+
+2. 执行 ``pip3 install ascend-deployer==<version>`` 安装ascend-deployer工具。<version>为ascend-deployer工具的版本号，
+   建议参考\ `官网 <https://pypi.org/project/ascend-deployer/#history>`__\下载最新发布版本的工具包。如果提示pip3命令不存在，请用户自行安装。
+
+3. 执行下载命令。
+
+   ::
+
+      ascend-download --os-list=Ubuntu_18.04_x86_64 --download=CANN==6.3.RC1,MindSpore==2.0.0rc1
+
+   执行以上命令后，会自动下载好OS所需依赖，CANN软件包和配套的驱动和固件包，以及docker软件等，**并存放到$HOME/ascend-deployer/resources目录下**。
+
+4. 安装驱动和固件时，如果不是归一包（包名以 **Ascend-hdk** 开头），需在inventory_file中提前配置cus_npu_info变量。
+
+   ::
+
+      [ascend]
+      localhost ansible_connection='local'
+
+5. 执行以下安装命令，自动安装所有能找到的包（MindX DL和MEF Center除外，该两者请参考 \ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\）。
+
+   ::
+
+      ascend-deployer --install-scene=auto
+
+6. 安装后配置。
+   使用python和CANN前，需要根据实际情况配置环境变量，以下内容以配置python和nnae的环境变量为例。
+
+   ::
+
+      source /usr/local/ascendrc                # 配置python环境变量
+      source /usr/local/Ascend/nnae/set_env.sh  # 配置nnae的环境变量
+
+7. 详细指南请参考\ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\
+
+
```

## Comparing `ascend_deployer-5.0.6.dist-info/RECORD` & `ascend_deployer-6.0.0b1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,388 +1,356 @@
 ascend_deployer/__init__.py,sha256=3geaeGzhrlHQWFzpr3TqJSebV4Xzi1goFBjRH-QgqpQ,769
-ascend_deployer/ansible.cfg,sha256=mtZjAEI3kxTB6drqwmI_R59MFLANHcTd7tl--LzIETo,444
-ascend_deployer/ascend_deployer.py,sha256=CImgAfH5GtSVJCEVqX-5-AMRERCrdTP1CUYqoN1W5PI,7854
+ascend_deployer/ansible.cfg,sha256=0KR5x1QrpdWtQUsNS8NErtukS4QEgksOIxq5x1FR_7o,516
+ascend_deployer/ascend_deployer.py,sha256=O1YDmvF41kEv-m3oHxrzjMXOAEfxM42FRVLpABrYJwI,8717
 ascend_deployer/ascend_download.py,sha256=gDa6rnZVCRkBzuNhHT195zwLp_OgwL7d7pLeee6gw0E,2174
 ascend_deployer/downloader_ui.py,sha256=5w4oMvEGz-Xe3nY_pvK3oaaYFI1LfkxOLWgTF4PAZyg,6179
-ascend_deployer/install.sh,sha256=YfTx0-bo5CInb8GSyHhWD7le4slg3uQEjSubsYC7pgA,835
-ascend_deployer/inventory_file,sha256=nOBLdlbqVGZvvaJj-05BsOsQo6543Xiy_enxEkm-LNk,493
-ascend_deployer/jobs.py,sha256=p6VtsEsdGl5hO0y-9EQTpA74lT01FDXWxc8hAN3TQUA,7090
+ascend_deployer/install.sh,sha256=jg1h1jkYa0xzHn9TTuLZPEMJKkcCksq4SuEhXh5xYmw,409
+ascend_deployer/inventory_file,sha256=ZdRW30Kru_tWelcFCLPt-3syvvdJLiwBpzS1aoYYbUw,530
+ascend_deployer/jobs.py,sha256=n0hvmqJDy9cde6KTV0I56SzO-cBqzXdHtnfQXmpP2V4,23290
 ascend_deployer/start_download.sh,sha256=xR8a9C34dzBRgLyNfjurvpA0OISpeF-rqG3guJO_fsQ,475
 ascend_deployer/start_download_ui.bat,sha256=5L5Hmzv6aw9I0qufUcBZ2gpFP1oshz1H5Da1ctQio8Y,69
-ascend_deployer/utils.py,sha256=3gkUhra_OGAZAUMKbLi9sujlfmrKrOogksWJ_OGXwYI,7852
+ascend_deployer/utils.py,sha256=1yVrDpR70I-K7x8sgiDJnvFJqM0eSh66fxEJYbuze1M,9686
 ascend_deployer/version.json,sha256=HA6x_geHEIgQPolmzJ-qv1Zmt6ESu2S6xXnvn-gxAPk,54
 ascend_deployer/ansible_plugin/ansible_log.py,sha256=HMh0u19kVPwY0vllTSVRNAf46-L0GVpVn74P-pgbplQ,14692
+ascend_deployer/ansible_plugin/deploy_info_output_plugin.py,sha256=TWRS91HnBgsq3Fwkil8dZgPr-MjDCmn8bC13xCXFLVg,23041
 ascend_deployer/ansible_plugin/install_info.yaml,sha256=sv6NOIG0Ii2IRXCefbq2oCyz3BqAOG9r61FPg8JZ1fo,1123
+ascend_deployer/ansible_plugin/progress_config.json,sha256=_9y0mw1-cexvZYWzzgI9gEkRJmpHsU5DrbtdXOXzTIE,4478
+ascend_deployer/ansible_plugin/standard.py,sha256=NDBEwJO6T09im_fXWIVzBU7clsl_RP1xncOtCcaAF9Y,2002
 ascend_deployer/downloader/__init__.py,sha256=sC8Dz2PJ66aLzUn_8-E4sRlZp1raDgKWrX_ZpznrE0s,706
+ascend_deployer/downloader/ansible_reqs.json,sha256=SAOH-D0tmmCV2n7EFf99sZY9EoJYzCvaP0W41bkuaNw,1493
 ascend_deployer/downloader/config.ini,sha256=aeLfwNjJSMZjo0MivMphHqSmrASJXrwOrXWHO7lF6tI,176
 ascend_deployer/downloader/deb_downloader.py,sha256=7cvls40yFVjUP0TdMfNmr4UcezZhLrLEMUXgnmHnUY8,11086
-ascend_deployer/downloader/dl_mef_dependency_downloader.py,sha256=b3DN1nF4VOqRO0l9O65DwACxWqimWivJvyUDBicok24,3855
-ascend_deployer/downloader/download_data.py,sha256=mc2eZAy6tO5bgfYovyUjEjS5Kfv99rSfUhMD4p5Wta4,2197
-ascend_deployer/downloader/download_util.py,sha256=CA7fAA_g8ZjhcNKMw-4RewBaO1Rrf22Ft-POmKrK8Tc,16684
-ascend_deployer/downloader/downloader.py,sha256=p61ftwIeZd3R5NOvkh7qW3IRCA9Xo_B8iS9YH4Kj2wg,11892
-ascend_deployer/downloader/logger_config.py,sha256=poczViEn7kdcbSU2FbmD4usux4VYJAjmZ2q6fBImWEs,4554
+ascend_deployer/downloader/dl_mef_dependency_downloader.py,sha256=RAMQXZYnXLXGV4qGAESxyIoJLOOiJcuMs88gGalvUxQ,5682
+ascend_deployer/downloader/download_data.py,sha256=YB7RHTHMK2ZheraR6GY-cvBu3V8-6LFgywG3_gCd60E,2225
+ascend_deployer/downloader/download_util.py,sha256=VQuDEMPIGxHlB4vcx1Knl5hZCanepzREZmnF97a2Rs0,16037
+ascend_deployer/downloader/downloader.py,sha256=G5DjS-db1c-64Rv_aWTItILZ6O1Rm2RxtEPY4CAJH0A,11656
+ascend_deployer/downloader/logger_config.py,sha256=_QlTKeGAsik0rFDjBM6Ks3_qarurrpGLuUvnYy08P_g,4536
 ascend_deployer/downloader/obs_downloader.py,sha256=FSA2WP91NqBgDNCZiCJAwzYomihA2-4jhCraZPHRHtI,2839
-ascend_deployer/downloader/obs_resources.json,sha256=klUXKEFwGS5-J7KzODKzwI9nFpyhx4Tczn1COJpgcHg,1630
-ascend_deployer/downloader/os_dep_downloader.py,sha256=AV1c54XNzlOLNjVWSKU5f8yz5pmunuBPf8PcFurtFs4,4685
-ascend_deployer/downloader/other_downloader.py,sha256=B_C8YH5gAirvVGf6Q0n2dy2e2snPs80gJN4M90_bn7Y,7197
-ascend_deployer/downloader/other_resources.json,sha256=aWdksKlWL8mnBOeScz_5GqosAhxbo69Lt4sh83mHXDY,3450
-ascend_deployer/downloader/parallel_file_downloader.py,sha256=mmj0xC6fVXhXocRhKHrG7lucEnzqb3u3iN-yiDEIs6U,14538
-ascend_deployer/downloader/pip_downloader.py,sha256=1dMjncIobVRw3gk0u_PpkH17jmSaAA_Q-4bgExqP6Ig,12446
-ascend_deployer/downloader/python_version.json,sha256=9pSqHUoRuHczku4tbP66Io8q519P8zCnDbPd49mgX38,8754
-ascend_deployer/downloader/requirements.txt,sha256=b18DLSv-yKH3qSy9mWvXL6tXu8OyuNlXlHuu5gXngaM,1738
+ascend_deployer/downloader/obs_resources.json,sha256=2mDuKKmhW78BYGKMQobJEmaG0yFl5WiiS6qeIMQPotk,2132
+ascend_deployer/downloader/os_dep_downloader.py,sha256=6skqs3gOt4aW_mFNK2UQGJgkPb23eBtG8rJdBsodjN8,5177
+ascend_deployer/downloader/other_downloader.py,sha256=YGlCXMhSB6nD24-Kt4CPvfAlKCtiuv3bKWfcjdf_QDE,7534
+ascend_deployer/downloader/other_resources.json,sha256=hly5GELxLI8E8qZdFIt8sU25oe1XcvOqvSpZixCPO4Y,1485
+ascend_deployer/downloader/parallel_file_downloader.py,sha256=ejcdofM71mkeive4YPYin9g7XqbIsQhpyjyafBKaGSQ,14990
+ascend_deployer/downloader/pip_downloader.py,sha256=63j25KqB_S4wceJfZBCztUsG2zXgDHGIpS9Hp9nTd2c,8153
+ascend_deployer/downloader/python_version.json,sha256=2NpXwPeA6IWqo_2mZbAe_1kJWIhDoZblaBalXqk91Yk,11880
+ascend_deployer/downloader/requirements.txt,sha256=3NSisyMYjx-IgW6zwO3VoGpJeM-GKnqkgFa_EO9VboU,1811
 ascend_deployer/downloader/rpm_downloader.py,sha256=FEfunjxBgJqGD6_3Wx3uybAbXN-f97HmjNVIPKkFMlg,20222
-ascend_deployer/downloader/software_mgr.py,sha256=TdBQJZOfqN_NKhyiv9IhiE7AgMJq628ve5D0EjBNgdM,13421
-ascend_deployer/downloader/version_match.json,sha256=jyXRVKttyeJpDUzMjDokAEtGYrzv-F-7bE7QT6JbDWw,935
+ascend_deployer/downloader/software_mgr.py,sha256=Jq-jGQr9HRJdERlz8EAodidlxJlbT6I0KoW7JVQDCTk,13898
+ascend_deployer/downloader/version_match.json,sha256=910nBM9N3JL_uTqxFd9CaYWSyE7OI6Kl7RKtgCyd7Fw,1135
 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/pkg_info.json,sha256=G0Bgg-n0LDdTEvU7J5iSBjDVeWSrFgyD9ND5CRbveZw,1106
 ascend_deployer/downloader/config/BCLinux_21.10_aarch64/source.repo,sha256=E95fOfRZwFK3AMg5eYg85T5LwjoJEt9Jrd_3IBVXuCI,157
 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/installed.txt,sha256=7zYwkXP8xHs9nFktIQzJkkzZJ8ntsht1alo5vffHDYs,65719
-ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json,sha256=VuIkFq5JJ7UerUtp6iVldfjtbVPUx3klThSos_ajlrw,3082
+ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/pkg_info.json,sha256=1e54vuXA8v1IYhiuWKrxvnVTLHnFjRn_0x6ybAC4Jfk,3627
 ascend_deployer/downloader/config/CTyunOS_22.06_aarch64/source.repo,sha256=LLkxKi3-fLBGqmF14zvDH8U2SljTH2Npg8RO9_G9HoI,262
-ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/installed.txt,sha256=Kfbn_pvj2gMy7GjrfJESAj8rWbe-GJca60ccnCjU8cg,66091
-ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/pkg_info.json,sha256=EYLIz0UbG8uSttN3dBUHcHuR3IwdAJlCYtZ1RGDd9lE,2844
-ascend_deployer/downloader/config/CTyunOS_22.06_x86_64/source.repo,sha256=1fIJU7VsvR1PEYd0aJIlcnwEI1oiifD9a1r-cKcb63E,251
-ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json,sha256=x9UkINP9ByEV5P4C0ix91X2wCh4lFjUNx5U5Vf83FsA,12476
+ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json,sha256=DUuFwlh1IxMkXCKkNpsu5Dsra0XGC-ur6EwQEpODMd0,8382
 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo,sha256=MXAKWne-AouqA4H0T3YO1gmRCsOKwY-TeG5MbBDqff8,234
-ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json,sha256=nKwyi3IEC2BrADH8uXm6OWH2f92SuV4ztkbJIdMpOWM,13906
-ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo,sha256=oOiLtW45sOuZZ_P_pugv7LhrEgs3uw_xrRY5-FOjNtM,371
+ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json,sha256=WSoTqOpqGd5Rvrsa8uxGB6Ln7OXJE5KWnIxwy3oLAeA,8533
+ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo,sha256=UAkL5U0cWgp_wO5O2Kw-_FSbnLFm_PZ98AmTyfDEH_0,223
 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt,sha256=nKuC_VfjU73aukPARJMi1U9a9ZdUItqZCcvz0W_edaQ,43257
-ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json,sha256=X3rIy4NooXv4HwSh1SjxBL9F6nfYcsOZs_t8mGC-Yv4,5919
+ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json,sha256=rGkNrfyktkTyzsGGR-9BBOPkNf_vMUK2HszFVPMllzs,6521
 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo,sha256=eysNjtYexsTQGiWpLqXoN9BYfCgLxfQN8cjcb8GDQtg,131
 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt,sha256=s_R0_DEUFrxq40paa3aDFxOeqFAiyq1G0K-kLOwAEMg,42707
-ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json,sha256=Yjs7twPlcfatHkCmILcqqwJkzRyRYagPB7FQj9n5NUI,5143
+ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json,sha256=7f96Ozm8A_MH8Kn70-3JCKLYeIAkdTRvaiVe27AXHyg,5741
 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo,sha256=4C0abYxsv25uVugAAdc4mPhbMxiaO-4vN8TnNgwqBXY,65
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt,sha256=RABC9Ydam7O91w4uymLiO04HCDgSG8RigE_2u1Sx6Iw,65900
-ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json,sha256=uYwIsedNZcn10XavsDoN3vwYMf4aSMg7v_MwzvcbIdQ,9517
+ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json,sha256=Rt2BKDClMOWIGdgIfjm0cvPZINdmdQu5oc6TrIQ0c6w,10119
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo,sha256=-4n539gqg17t4JRpUyqctcJ0eQK5-1KZuHqDFLvtKqM,130
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt,sha256=B1qfqvax5MY4ZBvzHa0z9cZNPgjymCcqOV9mDz-RdAE,42840
-ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json,sha256=q6r6r1Wm3rCbI6xXBbfsdu0YHh4sS7XUUGWGGzVLUvg,8566
+ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json,sha256=d5-1l1xfUI4jLrUioTU-DtMh16fNhpABUZ_GEk9CSY0,9168
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo,sha256=Cvl3U3MpU0IQc8gTvS6HdkDGIzRQzKsWChIMQhfTEyQ,130
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt,sha256=JAcDXwKy_6MSFPVc_5ntA_JTlP3VpfWE0P6NHLlRECw,42208
-ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json,sha256=s9zidqzIthW7VCXXCrpunVMp7NIUxDEcvdutDw423BA,8108
+ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json,sha256=Btsom3oqCvj2YE0xSE4iU3CEEnIAxYf4IIy4XKquSm4,8706
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo,sha256=44o98hE2tl4xd0ScyHk89RYwk58p7Eq92qysQZ_PmgY,65
 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/installed.txt,sha256=kZNU4UfOEOn1qR-ufWCl8zt_QkDc0QkK-OmuGiRErd0,55524
-ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/pkg_info.json,sha256=pA9C3suE_1Vlf0xTVHHnxXbb-kdiboI5jTarXZTJX74,3888
+ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/pkg_info.json,sha256=Ids1BzhzZkLPtGp-gzOHxWQgWKDMJYT50Ch6vQCwPXs,4071
 ascend_deployer/downloader/config/Kylin_V10Sword_aarch64/source.repo,sha256=Jxy4lKEo7jdw6jWhPVfN9I37yA-TA4fQDN8La7My-20,263
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt,sha256=sItZv2m9qFp8vdh6xsopvEQICxIsyKCWkrGMudbBmNI,60396
-ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json,sha256=vJFfEC0Kl2oWZ3ECObcqRhHkkommx15ed0SvlhC_-ew,3388
-ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo,sha256=qzbPi9gTz9pPFmXH_7Vbp7saSm_ivgRK6DkMOkUORIc,264
+ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json,sha256=bTCbynGf9N3F9HFztzuQgKEtyQlWOF40mAQZG8Dspt0,3368
+ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo,sha256=Ez5klJhEWuUYWPBLFrADq68XXOoxfglSjKQrIOxoKcc,259
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt,sha256=_wVdEw615qxHMyxH06QJPIuvBLapIG9r46oK6XY0pck,60964
-ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json,sha256=paIq645CQ2wCSYSRvcKINTxJnfl-jM2jZh8DAyHYSvc,3201
-ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo,sha256=ui74lUzSLFVRgr9NGZm0638JrJvflQNHtDbmvdbWDvQ,253
+ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json,sha256=-DkaZpre9sc3q6FLvynX05WSXmm9fX4bUV_8NKaN2m8,3181
+ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo,sha256=5jgtwOC7b0LAfHkuTBGx4T4kjoCqVbAze0bhTGZinaQ,248
 ascend_deployer/downloader/config/Kylin_V10_aarch64/installed.txt,sha256=sItZv2m9qFp8vdh6xsopvEQICxIsyKCWkrGMudbBmNI,60396
-ascend_deployer/downloader/config/Kylin_V10_aarch64/pkg_info.json,sha256=vJFfEC0Kl2oWZ3ECObcqRhHkkommx15ed0SvlhC_-ew,3388
+ascend_deployer/downloader/config/Kylin_V10_aarch64/pkg_info.json,sha256=LCd_hhJdsDhpSEPKNxkJ2EhB7q_kG357-RCuDiK6Koc,3565
 ascend_deployer/downloader/config/Kylin_V10_aarch64/source.repo,sha256=Ez5klJhEWuUYWPBLFrADq68XXOoxfglSjKQrIOxoKcc,259
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt,sha256=ItxvYYCtXV-E-9aVtk_YelIQ91MLQuA3byYuTrGz0Yg,51454
-ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json,sha256=2hq22MMdFgiomw6D_ww5lxYJ8cOYvtGp9AoTSGkfmkA,3369
+ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json,sha256=16ORX2-k9Ez8lf5hPbuEV_eFx1aY1XhRHYzbXzxRNw0,3546
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo,sha256=5Xkg_Au7cKVS2S-Wt02HnPX6QRs1mcEg75CNuIMRzck,365
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt,sha256=59jrLcg4b3IR3wjBavS0g040YW__-uC4EdEoW99bl8g,51932
-ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json,sha256=M9StadsdGG5Bd2PdrSYPvj6ygGrtmFlUPkBhGLh8Qo0,3651
+ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json,sha256=iu-lK8sdykG7uxW-nVe4lQMFz5f8bf2gPjjwyG4rIMQ,3828
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo,sha256=0BvlH8TblZbbYBRHdx8YgqMt9vr6E8tG4i9H3P7DBU4,353
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt,sha256=kNV9sbRHNGfDPh44gJRfKeT_1ixx1G5AVsk2lF-rziQ,51351
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json,sha256=7w8QiW99KBuSANC613IVPImWsiNUAAySucQBdh_TbNA,5439
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json,sha256=GWts9KXcPGslYG7F5czQ405rzj7N9IoPTJ64niiREN0,5809
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo,sha256=koyb7uyQaYLNckSFx2dipEQME7k29Qz9YJYRo-UslvU,458
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt,sha256=dTh1kpyfwd7wD2-6YypziUtVmDMBiLSOMQPaAuo10K0,43010
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json,sha256=zWvYiYFtRgB0w6TRznJ1bmPK13E-fsKP52-gyo3m0Ic,3220
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json,sha256=EiHXVeJNcA-pXtzd4WpOQZHaiAtmk_oxIocHcaKic74,3442
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo,sha256=dckwsHk8V5ZZYeJBG5Y-_KE9lztKhBEn4Fi7rLAN6_g,445
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt,sha256=WfZIn1u2qhzTR2tJhECdiX1d6sCPgwWepEVBn5HBx-c,56970
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json,sha256=nxi3gwHX2cjC4Gdeh1L7WicmHGzL10F9eNI-n1Mag9I,3134
-ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo,sha256=6HDMnrFt-aUP60MEN6Tv5nJCokJcBvyS_jHmq8QT6dY,268
-ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json,sha256=nb6YVYUCV95bzm1-5tRIxukfb9ZT38vHdJ106cRpu8k,4234
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json,sha256=P7vUxtdhMDmbDHnN9BdYZpIkqR4Ft7IWlT8Mlyh1CGU,4
+ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/config/UOS_20-1050e_aarch64/installed.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/config/UOS_20-1050e_aarch64/pkg_info.json,sha256=P7vUxtdhMDmbDHnN9BdYZpIkqR4Ft7IWlT8Mlyh1CGU,4
+ascend_deployer/downloader/config/UOS_20-1050e_aarch64/source.repo,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json,sha256=qRnEvmgM0qwuI_W4rq4tK63QDbaHGzOk8vExSXdoHeE,5790
 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list,sha256=hDXHX8w0fwit1D2njIhhBTOjCzwehVkd5INGTmmwSFU,370
-ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json,sha256=790r9-4P_iofm_J8KI6ZoKm8gpyCGM-BhTdeEehYCm0,5748
+ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json,sha256=EI_XA7QppvBGSRErbkLQa22ZPMo-e1MfhZiK_uFCpHo,7004
 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list,sha256=-ZN1Y__CqGtpqogO3QHVnOVl04MBxQvu9CQn3wNJt_I,352
-ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json,sha256=nWRGsqu4NbUq36Td-irZbGABxC5_fKGALBIBPkuypNw,5202
+ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json,sha256=WyG6Cl7UZAulkQBAyIpeYiHxtL--X6tqVIV5d3NVE74,5391
 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list,sha256=8QbZP5aNc9uYxYVTe7WmeGYZljWPZ_Av6bvkgb4hwqE,366
-ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json,sha256=wRqLDQwfqp8CmRdx5O61OYEcwaUnR6CT4Vb8V3itOLQ,6286
+ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json,sha256=x5fF_Y-irgfAkjysOPopk46hZ9HpW5sbbbfYKpfQzl8,6021
 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list,sha256=Fpa9xHLXJBSoHonzvop98ucN4yOE2q9FAuu06UKHFL4,348
-ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json,sha256=Jl5S-XhdQmGq_ChQ8GN5WUiVNDVzuC0d7_DlUzQQURo,5921
+ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json,sha256=LrTYRhJxOEYLKnvK2Oeizs8eXigxTXinlFs92hRvH5E,6325
 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list,sha256=dVuItkYL-4PTn0tTbcBbObkaXOYD7JlBOid9LHoAlWk,366
-ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json,sha256=m0veft0BDzPqeEnUA7gc3gVaNTXFnSFuRmUXVKt6pcU,6674
+ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json,sha256=Rm4HPFe4EcGUTmS4RcNI2jcDKAMQLUgy6Np6nMrTr0A,6764
 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list,sha256=CZWl_Rw_Qdy_qpekt40YqzeDtmS3GEjmsF-6HIntiGM,348
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json,sha256=3f-_TEgN_kgZ6HWMWzXxpbBNc56-4vnEV7Y8_K4CXbI,3938
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json,sha256=XfvMDCi7WwvCK0EkciI3RvmPg6W6DWMB8-DqiZQlbf8,3922
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json,sha256=LGJUAYv86eT__6LkHK4eheBdczoDD60vgh_tqY289OQ,3930
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json,sha256=TzMCa7bIDBL080Bs-OhA6VSSnRAYurBQc0DVjzs8dlg,3914
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=WxOY6ksoJRBZdSnzJqHtrGA2Ly1cvamD6o9TEYyTzs0,4010
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=23vxrVveSvbV0c39ej2j1T5gHnx418NfXWOu-eA07to,3994
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=jflvDFh6kYca6MdZA7BXA5o1zSjsCfUbNG1rJ-LfGHI,4010
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=zUs0wwufXRyiDI8vlggRnaxxSReqbliZKmBLgZSgmO0,3994
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=HVxUV_lWxqcqB6jOEMyrzkfGXS5SniFiHNPlrn65SVo,3954
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=Ow8yySozaxaL2hJn_K-zE3CoovzBE84qOULBkzin0CY,3938
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=bGiD2H3kz0cwgBg7c2h33NvZBcMTYjoZS5BdWDDIer8,3954
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json,sha256=pXMDeW01zcR_mn8gKMaHoCAemCu208GRGmbelal4Vpc,3938
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=WpIGaJSREvRxoJl9YH3LM32kZhF56mcD3OCpfjhTseQ,3954
-ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=WgonedBeDKqan8S5y0its_d_bUMXFfDiTGLx2zib1s0,3938
-ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json,sha256=jaXDi7dHh8QEHfvhs5saz8CZJsaVrM1ASp-WWicCUiQ,3715
-ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json,sha256=2oTyycsGfpuap8bZZ2EbpMOlkXrF6dFpTO1NAG1u6wg,3681
-ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json,sha256=Q0_uj5ywM9b67YFlqPvXcX6q9kP0eK2WqPekvLIIhAw,1185
-ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json,sha256=ktAZupLZ9kSOWJFRQ9DuiUpALjd81f4SlUmIvEkVCrM,1177
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_aarch64/resource.json,sha256=TXjV8mL8UGoC4oyDrCRU_w9ZrB8Zbiu4odTRHJbnjs8,3116
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CTyunOS_22.06_x86_64/resource.json,sha256=RpZdpTZYKOOHX5A02EFp5JcSRKteh3aKRSsBbJ3qvaI,3106
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_aarch64/resource.json,sha256=VXlbf5N9S2eCnO_aaHTyfuVNLrtv-ElWMoHmT_aI9HE,3938
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/CentOS_7.6_x86_64/resource.json,sha256=qZzUI9MT0A-R68NNODFGdIoNHgJuQqlsqu4vaEzh9Lo,3922
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json,sha256=OFz6GX-a5DZQFfX9f2UnBJzDhdt5qEft_jX2klPYtH4,3930
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json,sha256=9tyzezJt_4--2A9mqs82isUYNVd2jNbzl7wTkeGFnxk,3914
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=RckF2n1Rgb8BFizeSlidtRHl_faL2d0jFzQ6oqPbVHg,4013
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=CGxCs87Sl5vgKuYnA7KTXdzbtlz4gKB_4lJYGMq84Fg,3997
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=CyIqfUYWHDAb9pDpoLdaW70lUVXCz1nAN_R7qvmFRb0,4010
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=Il-EaukWR8ZuZrGAUiC6AyLyuKfkz3Zzn4vkd6YP1bQ,3994
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=zwhswZEFbCvqZL2z0VU2utH9YLGVLNogJj9gs-c7JB0,3954
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=PmPyBVbqOzTHcYQvhp0uoeeaxD7J0o-kb46vxGAGfPY,3938
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=gkYLu9DTbXnysNM7Z6hGSutlNdRD1L_3S5uB1wtOAk0,3954
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_20.04_x86_64/resource.json,sha256=f0UsJXOMunyqTyzMCE_wM6RrmuJFm_TuihD5yojhrjo,3938
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=OMKaoo1QS7JQWaUcrQPZ3gTlwXF0gWn_fPAlYLB2aSI,3954
-ascend_deployer/downloader/dependency/5.0.RC2/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=5TBia8YgG4PCiXONJWNrOlemIWUdyM-klBMbZsNPJgc,3938
-ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json,sha256=xuXkyEs5pypGLQGwPcHadY2wy-iVe8Cb6nsIiXNiaXo,3939
-ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json,sha256=8NiyRqCGNo5BA94TyKtc5aHwOb2OaB4ByBWCMuNC7mg,3911
-ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json,sha256=Qvbp4Gj9dGemK5UtNnYv88FphUDfWkLx0oaWLQ039bI,894
-ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json,sha256=_dFtvuRP9gEh8ZajMw0iaSUHLM3BRZ4_IQgKa20qPFE,888
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_aarch64/resource.json,sha256=TXjV8mL8UGoC4oyDrCRU_w9ZrB8Zbiu4odTRHJbnjs8,3116
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CTyunOS_22.06_x86_64/resource.json,sha256=RpZdpTZYKOOHX5A02EFp5JcSRKteh3aKRSsBbJ3qvaI,3106
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_aarch64/resource.json,sha256=VXlbf5N9S2eCnO_aaHTyfuVNLrtv-ElWMoHmT_aI9HE,3938
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/CentOS_7.6_x86_64/resource.json,sha256=qZzUI9MT0A-R68NNODFGdIoNHgJuQqlsqu4vaEzh9Lo,3922
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_aarch64_pre/resource.json,sha256=OFz6GX-a5DZQFfX9f2UnBJzDhdt5qEft_jX2klPYtH4,3930
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Kylin_V10Tercel_x86_64_pre/resource.json,sha256=9tyzezJt_4--2A9mqs82isUYNVd2jNbzl7wTkeGFnxk,3914
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=RckF2n1Rgb8BFizeSlidtRHl_faL2d0jFzQ6oqPbVHg,4013
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=CGxCs87Sl5vgKuYnA7KTXdzbtlz4gKB_4lJYGMq84Fg,3997
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=CyIqfUYWHDAb9pDpoLdaW70lUVXCz1nAN_R7qvmFRb0,4010
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=Il-EaukWR8ZuZrGAUiC6AyLyuKfkz3Zzn4vkd6YP1bQ,3994
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=zwhswZEFbCvqZL2z0VU2utH9YLGVLNogJj9gs-c7JB0,3954
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=PmPyBVbqOzTHcYQvhp0uoeeaxD7J0o-kb46vxGAGfPY,3938
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=gkYLu9DTbXnysNM7Z6hGSutlNdRD1L_3S5uB1wtOAk0,3954
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_20.04_x86_64/resource.json,sha256=f0UsJXOMunyqTyzMCE_wM6RrmuJFm_TuihD5yojhrjo,3938
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=OMKaoo1QS7JQWaUcrQPZ3gTlwXF0gWn_fPAlYLB2aSI,3954
-ascend_deployer/downloader/dependency/5.0.RC3/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=5TBia8YgG4PCiXONJWNrOlemIWUdyM-klBMbZsNPJgc,3938
-ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json,sha256=d7Hwt_nsxR2rTghGf5DwS-ei0xEuWSDyG9HE31V6Qlw,3975
-ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json,sha256=6zTZF5JYY_W0F-E_wadPK6kxiRCLSSKpTClD7RqApkc,3947
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_aarch64.json,sha256=TXjV8mL8UGoC4oyDrCRU_w9ZrB8Zbiu4odTRHJbnjs8,3116
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CTyunOS_22.06_x86_64.json,sha256=RpZdpTZYKOOHX5A02EFp5JcSRKteh3aKRSsBbJ3qvaI,3106
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/CentOS_7.6_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json,sha256=WsX0LaBKD9TeW22b-wZ5vK2J9x2-zlRyRX6P4j9nwHs,338
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json,sha256=lG6GHYIPfONNff73lfqARFt-dDBt1B5xiKc2vm-0Zw4,336
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/UOS_20-1050e_aarch64.json,sha256=M5zJ8APKTsolPqrbzkVJiaZkGr2MCj4bw7IrsIQWKiU,1429
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_18.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_20.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/COMMON_UPDATE/Ubuntu_22.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.0/DL/aarch64/resource.json,sha256=2AgH2qUrQeDbLax0QoEs11ciaR_nQ_qrxH2n6lq2jCQ,4761
+ascend_deployer/downloader/dependency/5.0.0/DL/x86_64/resource.json,sha256=ntyOPqR64xvYa5yQIT9r8MAXht_hyr40CfEZkpeTU90,4727
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/CentOS_7.6_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_18.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_20.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON_UPDATE/Ubuntu_22.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json,sha256=afZGVEB-OemgzuOUnacviy8W1eqdGLGSJcWj-RoHSYg,4225
+ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json,sha256=3tH1jo3kPNtv6SNheXmz-eOUiB07otRkaiujbLTvGUs,4191
+ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json,sha256=TR00YgKxrBMwZMHfuBjLVmBlbJf0KlnhyPw7YkOS1oI,1695
+ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json,sha256=JLMHPz2mALOQAVIs6ccAoHPbSCoPQQA8n8L-ErmjsVo,1687
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_aarch64.json,sha256=TXjV8mL8UGoC4oyDrCRU_w9ZrB8Zbiu4odTRHJbnjs8,3116
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CTyunOS_22.06_x86_64.json,sha256=RpZdpTZYKOOHX5A02EFp5JcSRKteh3aKRSsBbJ3qvaI,3106
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/CentOS_7.6_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json,sha256=WsX0LaBKD9TeW22b-wZ5vK2J9x2-zlRyRX6P4j9nwHs,338
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json,sha256=lG6GHYIPfONNff73lfqARFt-dDBt1B5xiKc2vm-0Zw4,336
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_18.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_20.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/COMMON_UPDATE/Ubuntu_22.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC2/DL/aarch64/resource.json,sha256=iLePtwWv9zeHZtOLPgivGfAVeiZfYQL3MHv-AQw_deg,4449
+ascend_deployer/downloader/dependency/5.0.RC2/DL/x86_64/resource.json,sha256=kkkKOgb31OOTxy9FmIkDdmpqmIiU-kGYcPngJycQvH8,4421
+ascend_deployer/downloader/dependency/5.0.RC2/MEF/aarch64/resource.json,sha256=hz4Ye05-vmJK8ofFrAwXLc-M26zyEkpa-gef8pRmC78,1404
+ascend_deployer/downloader/dependency/5.0.RC2/MEF/x86_64/resource.json,sha256=dLkhlou3OLRilcRyhH908sG0P16uu75l74rfsBxhOwU,1395
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_aarch64.json,sha256=TXjV8mL8UGoC4oyDrCRU_w9ZrB8Zbiu4odTRHJbnjs8,3116
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CTyunOS_22.06_x86_64.json,sha256=RpZdpTZYKOOHX5A02EFp5JcSRKteh3aKRSsBbJ3qvaI,3106
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/CentOS_7.6_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_aarch64.json,sha256=WsX0LaBKD9TeW22b-wZ5vK2J9x2-zlRyRX6P4j9nwHs,338
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_20.03LTS_x86_64.json,sha256=lG6GHYIPfONNff73lfqARFt-dDBt1B5xiKc2vm-0Zw4,336
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/OpenEuler_22.03LTS_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_18.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_20.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_aarch64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/COMMON_UPDATE/Ubuntu_22.04_x86_64.json,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/downloader/dependency/5.0.RC3/DL/aarch64/resource.json,sha256=kVqrHaxACTdfo6bB3XPN9ZImlnRzFWtmG5vNb1GNw9Y,4485
+ascend_deployer/downloader/dependency/5.0.RC3/DL/x86_64/resource.json,sha256=Xw0IosgSR_SpdqpscVcw4FDJmMZMYOn1c5nHspDAH1A,4454
+ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_aarch64.json,sha256=gjUKGw4EUwMXm3q2RfDID_5OV3pLEutRj2KLclAWAHI,3428
+ascend_deployer/downloader/dependency/COMMON/CentOS_7.6_x86_64.json,sha256=0kBrzzIUx2qzmLuN19mlJ0hteJadk__72DDs2u-i5vw,3412
+ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_aarch64.json,sha256=EDJ2MMOyrLq1uT-NXLcxJtPp8Svl7m3XquENt_WZKJs,3500
+ascend_deployer/downloader/dependency/COMMON/OpenEuler_20.03LTS_x86_64.json,sha256=Jdfiz-ceI4tX4YEzKmG9836EdjiiGIen4OlLwMS9w_k,3484
+ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_aarch64.json,sha256=5sVLxtA7gS7s9SZQal8FN-o3PhOKiV5H5yPyRAhVLqc,3500
+ascend_deployer/downloader/dependency/COMMON/OpenEuler_22.03LTS_x86_64.json,sha256=0JmKukNg0xqScuTTcZQSl7jifH2aszt1GpvQvcqW0wA,3484
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_aarch64.json,sha256=zDYFSo-j0vsoc_1fWfHbnDAzouxVwqb0TrM-sfVVBWA,3444
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_18.04_x86_64.json,sha256=Xqcc5a23OcvKtrBS50bIEGMHU13xpQ2MxkWU136vew8,3428
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_aarch64.json,sha256=KIh19U-S_zlerQjygZMaM0Y2yIAAeQJed1wA8C_Ca9M,3444
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_20.04_x86_64.json,sha256=Q3v4sDzJBWXZG-bpzJ7ktOawMbdiu3Q6vprv9U8zbvg,3428
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_aarch64.json,sha256=hpH0Z3lTYH2BjnqpRE0GV7hXdp_syC4Jgt96XzShyZM,3444
+ascend_deployer/downloader/dependency/COMMON/Ubuntu_22.04_x86_64.json,sha256=BdHFJDz2Lo87XEptD8xl8udGeIzx2y-0SaThPQ8ilTk,3429
 ascend_deployer/downloader/software/CANN_6.0.1.json,sha256=58Gbgm8925nBRZf7OCJnoRKe0F5QudT1BMXhsPpX3cE,3619
 ascend_deployer/downloader/software/CANN_6.0.RC1.json,sha256=vTT_E8mRFNbCnXZitYX-5gL7GH1cT1s0vjROl9YAvy8,3116
 ascend_deployer/downloader/software/CANN_6.3.RC1.json,sha256=sS3smHNhrAmycd0kor4dZh7xwwsXPSECEsNgYcJgBbU,3696
 ascend_deployer/downloader/software/CANN_6.3.RC2.json,sha256=a37JTNnjRxEnM3TGtoHmnKordBw8qM3MZphG1AE4M90,3987
-ascend_deployer/downloader/software/CANN_7.0.RC1.json,sha256=xZbpwHbCMPIcspns6bdlYKyF_3MLW8A08fzcZ5OoPo4,3986
+ascend_deployer/downloader/software/CANN_7.0.0.json,sha256=pZJAjD_jjuFr199VXp5s2lWRDuoCbWmuDWN03STQpUU,3904
+ascend_deployer/downloader/software/CANN_7.0.RC1.json,sha256=GhOsKXm_bExHUxnATIL5-FPXQXLa2hL07WrNpvav8BA,3987
+ascend_deployer/downloader/software/DL_5.0.0.json,sha256=fQ8GygLY_lMOrYFwpNCASLIcx0FmNk3bjH01D3x-jl0,191
 ascend_deployer/downloader/software/DL_5.0.RC1.json,sha256=xNynEjkmERJjQC_tGoEnQD_jb53SuRfJYbQvRaj8GaA,196
 ascend_deployer/downloader/software/DL_5.0.RC2.json,sha256=8P4QjRDOk2TIkUn9hqjugJ5OeoBzABJUqkJznrKWEak,196
-ascend_deployer/downloader/software/DL_5.0.RC3.json,sha256=n4-ShMn51Q-dvF-q-qWzgoaO-uo_U-WCF-8FAURhIDE,195
+ascend_deployer/downloader/software/DL_5.0.RC3.json,sha256=OYd33vJDI6uPM_6yju34TutHsEA_WYg-LAEoe7WUHAQ,196
 ascend_deployer/downloader/software/MEF_5.0.RC1.json,sha256=pEQR7FFBCFXipXT-Eljv_9mKcsStgeUT8T7H0i47MfQ,86
 ascend_deployer/downloader/software/MEF_5.0.RC2.json,sha256=r5QarN5ACGqHlQdvI0VuRDi9RJPjjvCKSV7o7Y7J68g,85
 ascend_deployer/downloader/software/MindSpore_1.10.0.json,sha256=vJlObRHpH1BQusd9efMF3lBZLtSb3z8-nsV-xWKu994,2847
 ascend_deployer/downloader/software/MindSpore_1.9.0.json,sha256=VSdfHxQIPhaHyIYF4_7-jurRHKWRVFgnKaO7H161DQo,2828
 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json,sha256=RwenhQYyp9VWWhdk20gPmFPUVr-hSAtjjSgNnLO6dLQ,2807
 ascend_deployer/downloader/software/MindSpore_2.1.0.json,sha256=khw3c7D9_dq3NdUZ_TXu_7ITWc94TJzlTDZPGXSrpR0,2750
-ascend_deployer/downloader/software/MindSpore_2.2.0.json,sha256=5InUUxqil0j4QA0wtEzXqdZylXQJKjzUd5QlVh8b9fs,2749
+ascend_deployer/downloader/software/MindSpore_2.2.0.json,sha256=kuNycHM-41INiSvabhAjNF3hoemcCNCzron5L8e87bU,2750
+ascend_deployer/downloader/software/MindSpore_2.2.10.json,sha256=UC2voVgp9bZtXh7lfLQr6L-0KDLanwML09cmHq8HqTo,2768
 ascend_deployer/downloader/software/MindStudio_5.0.0.json,sha256=Eo_mjiStaqYrAhlTBXzBzOV8pW7eILYwCZAWnZHQJck,48361
 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json,sha256=BgaX-Ndr24DOFZx8ZvtSw0ynu8XRXqDSLHj0MViAWT4,25492
 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json,sha256=N9eOjDPb0uIj2nzuWNqVNptKsxyI_AOWYj-xFlXUfVU,48369
 ascend_deployer/downloader/software/MindStudio_6.0.RC2.json,sha256=_0FtcCUbU91JQ63xSTK4XVdEmiB0I4x005H_t7rYRHc,48675
+ascend_deployer/downloader/software/NPU_23.0.0.json,sha256=GskiOelNkYoiw6kSLs26nXroRok-6ltyEpNY4hhNA4w,2114
 ascend_deployer/downloader/software/NPU_23.0.RC1.json,sha256=w50m35V7TQa9TDWmDtySLvyG1AdGaz3zZjSVIPVTd68,1461
 ascend_deployer/downloader/software/NPU_23.0.RC2.json,sha256=xTa405A_huH0rvINo4xIuJiuzqalbNyoOHAnpEk4c8c,1814
-ascend_deployer/downloader/software/NPU_23.0.RC3.json,sha256=NJFvBRBSNSM464ESQYjW8LPMYaREPjtiWbPk0tPVuts,2152
+ascend_deployer/downloader/software/NPU_23.0.RC3.json,sha256=DrZvKZvH1i7yg2CEyZGFgkGjLSuDdSboOnPBBWepjQs,2153
 ascend_deployer/downloader/software/NPU_6.0.0.json,sha256=nYubm4ipg7wK0R8HQ6TJIT18iFTgxK4s2ZzyTsoPqKg,2078
 ascend_deployer/downloader/software/NPU_6.0.RC1.json,sha256=rYWASlYo-sb7pK-R38UPVX45wEk4UvXDLHhF-6ANZ3A,3408
 ascend_deployer/downloader/software/TensorFlow_1.15.0.json,sha256=FJww1bm8Gx8ThNY9fcNqtCPT16fEik4EUot4dgWHP5c,1103
-ascend_deployer/downloader/software/TensorFlow_2.6.5.json,sha256=-ElZLiDrJTgvUNNZjszkwgFZ7uknVsQOsaayB1rAKdA,1097
+ascend_deployer/downloader/software/TensorFlow_2.6.5.json,sha256=N0VJg7Swndc9KaZdrGDhua9-b97OXRqv7jd2ASq__N4,2856
 ascend_deployer/downloader/software/Torch-npu_1.11.0.json,sha256=ybYLXVe9poCVIvQGcmDXsjOcT5vGWuoxbrUpKxD7Gic,2931
 ascend_deployer/downloader/software/Torch-npu_1.11.0.post1.json,sha256=mmpRuxo8NJW76nU2YHEFFgqufLlHynHz7s81jK3Si8A,5649
-ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json,sha256=BVDKCXKsFob4XEuxjNqp-bLtWLmZitDkTtfGhud98DU,5654
+ascend_deployer/downloader/software/Torch-npu_1.11.0.post4.json,sha256=xP0pXisPd0yHBw6v8PO_3f6FIMuvRHyZNGYQEyM2j8Q,5655
+ascend_deployer/downloader/software/Torch-npu_1.11.0.post8.json,sha256=MoJDTf0jpbxCPbUuyYaZS9voL_0fTGxNbDDktaQhzs8,7559
 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json,sha256=bHVi-oALMKxBmfkMaqe7ftb6gTUwUF9SyWR67rXjJkI,2946
 ascend_deployer/downloader/software/Torch-npu_1.8.1.json,sha256=rZ9FoxdT6Y7UKDqYfF6m8V1Rqia1CAj4PpgCcqboZ5M,2935
 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json,sha256=je5tcl2h6v9U7z8QSqaUkKQ60woifqd_UyOlyWWYXuI,2960
 ascend_deployer/downloader/software/Torch-npu_1.8.1.post2.json,sha256=seKXi0TMmIi6FNSvtGIsWmMd31RO3EGilASpDop5ANg,5624
+ascend_deployer/downloader/software/Torch-npu_2.0.1.post1.json,sha256=cb-tqvceyLGLdDCP3EjsJvYTMMY3A9k3gC1FNBVMpdU,5756
+ascend_deployer/downloader/software/Torch-npu_2.1.0.json,sha256=E9HVL_Rmy6bUiFPwYoTO5NNTqAmd-RZ6gU5zk-IQr2Y,6181
 ascend_deployer/downloader/yum_metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql,sha256=4TE3bYIpTQ0uFUhEHO94OBpU81WN3YygtrkUjd38DQw,1772
 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py,sha256=fi1rzqdF16qGLRKrLV6dK-DyLP_zi_vm8IvRWmE7Bco,11352
-ascend_deployer/group_vars/all.yaml,sha256=dD4P_Hhbg2Z10FBD3cO8IOhNzyOGZxBXAP6JGbyZ7Uo,1897
-ascend_deployer/patch/selenium_firefox.patch,sha256=MD5-UZ717Hca32fdmKa21g_JnbxKRM4BlVx-U-EPALA,807
-ascend_deployer/patch/selenium_firefox_profile.patch,sha256=K89iaIG9x0RX9qO0_LXISXSGDsG9QdzgvflrQWsrqYk,1127
-ascend_deployer/playbooks/basic.yaml,sha256=Ou1DidGhODBKq82i31KLe1HpOjMqo320AJndcSL3yMQ,236
-ascend_deployer/playbooks/check.yaml,sha256=xxq0cKw-bq_lQV4ZMz8HJjyaiTWp66Si7vyNyV-uepE,539
-ascend_deployer/playbooks/check_mef.yaml,sha256=FGf3L5QqmSTxpS7C_Ofe0S13_0NroU10CAjlXXkB5dg,479
-ascend_deployer/playbooks/check_pkgs.yml,sha256=vFej41gd3l3fq8khqR6jtsLPw0NU9JM1POQpbx4qmzE,94
-ascend_deployer/playbooks/clean_nexus.yml,sha256=xh54lcmYV49mPahbCpJolvF6qTlYCKZSq00aCPMBLa8,451
-ascend_deployer/playbooks/create_nexus.yml,sha256=0UjBWCHO5Mgxa8k4wxrzVu7Ox5WUXiZiXTwzhVlWIJM,611
-ascend_deployer/playbooks/create_user.yml,sha256=aKv6wRSemxWzG2m2y_tU356D9nRXiafRsGuMrW6NaRE,540
-ascend_deployer/playbooks/distribution.yml,sha256=javypj3rHcn6Rxx4kBqDx8MAkdbnqTJyZNE-w2fXz3A,663
-ascend_deployer/playbooks/docker.yaml,sha256=43GPdsfSWdOmFGNICVNCzPmC703dNZ3Uq-GxAnYK5uc,1003
-ascend_deployer/playbooks/gather_app_info.yml,sha256=Bmhjybkgks8NKxwwyTJtGHXeJqbOW66hn9uByAt2xJE,1021
-ascend_deployer/playbooks/gather_facts.yaml,sha256=UtX8qT8HT0RIThtEFEPmMHUu8dVUYZTvfI-4pACA2O0,3487
-ascend_deployer/playbooks/gather_npu_fact.yml,sha256=A5nkepo2PcFjeGiZxDkn8wAaZxVXbSke_X_uUuCYcBM,1254
-ascend_deployer/playbooks/harbor.yaml,sha256=_MLo4qg26_e9Nu1lVxK8zduhieyd1gY9oq7AfmJAuuY,121
+ascend_deployer/group_vars/all.yaml,sha256=EafmbuBOuAVEhA-ovNApPALec4arS_UGt_Oi6ZrbW20,2036
+ascend_deployer/library/check_compatibility.py,sha256=8HGFOEZ_1RUv2kdKtN4gMQAXTxKXGbDxrwHseiw81P0,5293
+ascend_deployer/library/check_nexus_status.py,sha256=D8tsXWIYyGV907QFKbiqzNQR7d5PfRUu3zq7oOC7lJ0,2521
+ascend_deployer/library/check_status.py,sha256=3pgj_C9YQpFosnrgLyw9muHYgcXD16qiMDAD0DDTQi4,9223
+ascend_deployer/library/collect_info.py,sha256=JKz9I8fSoTjk62cIPDMGQsTqqU0EbchHfBJq1jWCFFA,2847
+ascend_deployer/library/create_user.py,sha256=SKK2EZUzFPXfFrcdoLd2qZn2TG0pbMaHE2mj4Lraf2c,1637
+ascend_deployer/library/install_ascend_operator.py,sha256=XoIjw6PAHkGtltXiOl6Gq4I0KpTKfNmKG9JFRArlcQc,1499
+ascend_deployer/library/install_cann.py,sha256=WbfTApDX2-lKGvLgEH7--uOrXS2iKAzLVMV3NeKvmSc,11358
+ascend_deployer/library/install_device_plugin.py,sha256=O21SrwYrKcA2UboWXoLISV2QGY3UXUYuuG0n2aYH4Ow,6689
+ascend_deployer/library/install_docker_runtime.py,sha256=TKMkdLxT0_J3MyOvfIaOKUJyWB69h-MJNGkRr9E-78c,3506
+ascend_deployer/library/install_hccl_controller.py,sha256=YYtVVLNbH1C4yCWh9WZTTFX8bhlD9wXAUoHYIs9R_9s,1543
+ascend_deployer/library/install_mindio.py,sha256=DocW3dxTkBmf1Q2D7LlD-9CjezQ9zur7ChqWMHd_MGo,2636
+ascend_deployer/library/install_noded.py,sha256=xdujAZgVb6UXSFkfJL5S7zu__IgPEf_FpS4I6VBKuzw,1497
+ascend_deployer/library/install_npu_exporter.py,sha256=U-iB1G3gSQKsO4FRS527ujYPvA50KYtmR5OlfZLgv4I,1737
+ascend_deployer/library/install_python.py,sha256=VT8ObAgOXXFDQbQs48ZmsXpivgOyL0rTOeNO1PB_FcU,4748
+ascend_deployer/library/install_resilience_controller.py,sha256=LhnnI3mGgOK1AvxMVVEI1tq_AGFhwz4Vk1gnCifZoqY,1589
+ascend_deployer/library/install_sys_pkg.py,sha256=UWJZJiimxhy4gIMDoTMpPSbRl0nORPh_V0hmt5qnA-o,9563
+ascend_deployer/library/install_volcano.py,sha256=cg19ZbksAsQT1QkC-AJt6NWBusODKJVEq2onDd2Lsf8,3554
+ascend_deployer/library/login_harbor.py,sha256=Hzc7RzZ53hISc6LhGGLWcHZqkE954qGkxnH5vrcqC9I,4642
+ascend_deployer/library/process_framework.py,sha256=JweRmPCiRjm9x-Hh8x3ODKJZMNk02Ut3gj_5kMCgWgI,13435
+ascend_deployer/library/process_npu.py,sha256=m7yWiCTqU8CI5EedeO1XWkPGsNx0bBd_jLDSSz2qC9I,11726
+ascend_deployer/library/process_test.py,sha256=Da6k1M4DA66zR_dgggdYmtIq6Bb8WsvIIpKwW_-t984,11157
+ascend_deployer/library/push_image.py,sha256=__SAAxozi3I65VbE3CEXuty7tcKu9rk3WdlWMcB5lN4,6341
+ascend_deployer/library/scp.py,sha256=CbbzUEep1pVx9K8X2fC5cDlHTg4tazUFlFJWEh1Y4aw,3976
+ascend_deployer/library/system_report.py,sha256=kJcb8ejnky_Rljrp-jH636g7I7iDBbC7RW1_8xuWlwo,7956
+ascend_deployer/library/uncompress_resources.py,sha256=5hHnR0yMAEaJBmdMCPHfkXa9EtZen0K9x_Vu_teGbXk,4230
+ascend_deployer/module_utils/__init__.py,sha256=_W8CwG1G1xj8kCFRhvfGBMWMGKWObxY_Zguyz6Qrc1Q,39
+ascend_deployer/module_utils/check_output_manager.py,sha256=wDGKh0-zIv7OqOvv3R8MzThyqOOTyQ7LJiFIXta7Kys,5499
+ascend_deployer/module_utils/common_info.py,sha256=CfTrJ6b-JOYB0ZtLteNmLbHb_Iji-6faTMz8KMiLLUA,13373
+ascend_deployer/module_utils/common_utils.py,sha256=nHERyK_tKMDmM-6B92WIPm2a3ZSgwOuN0REWlA1He-U,4184
+ascend_deployer/module_utils/compatibility_config.py,sha256=X7aXy_8CKSoFT0vnn_5DRuuUQZFEfqAuomG2BmWYqbo,21172
+ascend_deployer/module_utils/dl.py,sha256=doWM-PBt1uYSAyH2GyAjddbd4ckJWNpwHVb5qjY_6dU,15802
+ascend_deployer/playbooks/check.yaml,sha256=PqVrzZKRO2IaMD-2WQGGxNy0I1f4QZbrjVYLSLF0bJc,607
+ascend_deployer/playbooks/distribution.yml,sha256=hVtyq1GW9wYwU66Mr-DP9kDpkUqHdWDkXDB561pIjZY,665
+ascend_deployer/playbooks/docker.yaml,sha256=oW10Zx2BJZjuXjuA8g38D_4nYtzhSS-MIOiglEMHuXQ,1095
+ascend_deployer/playbooks/gather_installation_facts.yml,sha256=YRxUCMcSnduvSdeOVakoNfPqOHIJ1KzEb3tOsWbWpCA,591
+ascend_deployer/playbooks/gather_npu_fact.yml,sha256=3sq9HJI4_elrHMCQ5yK0B_o69567P7EhR9ILC1QrapU,506
+ascend_deployer/playbooks/harbor.yaml,sha256=KPlfqpPk_xQuvYhsDjjjXIJdPNZk2LeNvLV1Ag0u5L8,398
 ascend_deployer/playbooks/hccn.yaml,sha256=VtkSnfHyq7wL9WRZ1FAhK6mpBjSFPRle8LCqTy8TE-4,193
 ascend_deployer/playbooks/image_load.yaml,sha256=G7-tr6B1ZUuRJYMkmYyBVbS2TBmkEEaRliIaLsvuc6g,133
-ascend_deployer/playbooks/k8s.yaml,sha256=K34Odp9uGc4nLt5H0VDtD5ezRJfLRwrK0Xi1ua-4R8w,2144
+ascend_deployer/playbooks/k8s.yaml,sha256=dvbRO8eQxyVy5Wy3N9qj_kCSUF4CYmfy-EuR63Shw7M,2284
 ascend_deployer/playbooks/kubeedge.yaml,sha256=bcF_WC6RqCBTA38P-hNWeCvBP38yIS-MdB333e08Lok,85
-ascend_deployer/playbooks/mindxdl.yaml,sha256=pTa-tC_t667ZAE58kj266EnMLu91vRhY4Yzt6IHAA84,2742
-ascend_deployer/playbooks/modify_user_group.yml,sha256=nFrPwxyL9wzrslWPcjz-w2mOZmqMrui4_-sPJmWpx3U,491
-ascend_deployer/playbooks/os_map.yaml,sha256=5VbMUe3e7Zgv-hewRKOmzn2mrP5Lho3o9fLtmkXZpKU,264
-ascend_deployer/playbooks/os_map.yml,sha256=PxFo37lietKCz6YCS2z9tqJk9e6m3ows4L9G5zEGqTc,2267
-ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml,sha256=nXMok4k-2PZBhv0JKbsP6yRiesABOdB_uEHqmH72d5E,1056
-ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml,sha256=nXMok4k-2PZBhv0JKbsP6yRiesABOdB_uEHqmH72d5E,1056
-ascend_deployer/playbooks/prepare_Kylin_V10Sword_aarch64.yml,sha256=eXZ-OCGV9uR8NUuJssaXCDBsRgk-Ja3As7RNbCMotFI,1652
-ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_aarch64.yml,sha256=FGUOd26iZV-tzjYlY09vDDvN0HXXHC2T2pVbd0eHUD0,1653
-ascend_deployer/playbooks/prepare_OpenEuler_20.03LTS_x86_64.yml,sha256=FGUOd26iZV-tzjYlY09vDDvN0HXXHC2T2pVbd0eHUD0,1653
-ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml,sha256=eXZ-OCGV9uR8NUuJssaXCDBsRgk-Ja3As7RNbCMotFI,1652
-ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml,sha256=eXZ-OCGV9uR8NUuJssaXCDBsRgk-Ja3As7RNbCMotFI,1652
-ascend_deployer/playbooks/report.yaml,sha256=YDQ6talRtZ3jmeTzM3mO8P7kX7_wFJ0lU7L71QdJtUc,575
-ascend_deployer/playbooks/set_facts_cache_permission.yml,sha256=vMTb7wIDN5utqsrGd8myI2l8U-hQVloe-AJZIrJTAC8,139
+ascend_deployer/playbooks/report.yaml,sha256=IftVJI-9VNDhTuJMox2BwLVcgtBF9vedZIR2UQOhJh0,1785
 ascend_deployer/playbooks/sync_time.yml,sha256=jiN-5XLWhK8YCkP8A4_h9ay4pDgDrWtvgxqpIgsSW-o,349
-ascend_deployer/playbooks/task_set_custom_fact.yml,sha256=IWk8YF2wuFS1Gku1k05QCMOIN64cywnEfLbM8mpzwx4,6776
 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml,sha256=n3PyVh4k72KzXuJEbBvtWGRcSGV_iDloiDp5TpJHFBI,155
 ascend_deployer/playbooks/uninstall_mef_releate.yaml,sha256=TZraFst-Ykc0wHKAoswYe3tW2a_yUGIS4CjFt631UHc,246
-ascend_deployer/playbooks/callback_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ascend_deployer/playbooks/callback_plugins/crop_columns.py,sha256=E745CmlBHbFkxLeOdsONQqf4eJ6Nv9f-CH-IqCstPTg,464
-ascend_deployer/playbooks/facts/app_info.fact.j2,sha256=KdVRCDzhLtGMqpKo1USq4YXrS3rxi-aSoKeV02YZT1A,5199
-ascend_deployer/playbooks/facts/npu_info.fact.j2,sha256=Qe8dTCyq4Tuu9I3B_jfP-JtKbKti4md1ILDG4hBM6DQ,7171
-ascend_deployer/playbooks/install/install_ascend-device-plugin.yml,sha256=OU6hUOy34hxms5tmSdeWZ4YOixXgxdvCpJ3KacL4vV0,107
-ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml,sha256=sIK2tC3pr9zkw1Vl2IeZ8unbYXMNbr0pZ6hldsmluqg,109
-ascend_deployer/playbooks/install/install_ascend-operator.yml,sha256=I5v148ZJAtrn1enEi0aVSUaQ4XRAjYOxIDfx8FDkLrk,110
-ascend_deployer/playbooks/install/install_atlasedge.yml,sha256=VJfBGHYkYJGKHzzpnbHhaHMz5-8yZzxg7Iuwknqyq58,584
-ascend_deployer/playbooks/install/install_docker_images.yml,sha256=J5EuB15vTrzB9QRVFx5A0ahAIX8B6iuPqOJYKgVI94Y,502
-ascend_deployer/playbooks/install/install_driver.yml,sha256=FbRqQuaa3Bd-hqQn32EiymelTFYeDwZmGrZvaGmN9OU,1299
-ascend_deployer/playbooks/install/install_firmware.yml,sha256=vegU_9N650CdW_ZNU4WHLArI-kHric_YDsiEeTfa6u4,1332
-ascend_deployer/playbooks/install/install_gcc.yml,sha256=wzsJ1usrYuSG1tvFe829VWRbAsqmyVKDa41F9bfWd54,896
-ascend_deployer/playbooks/install/install_ha.yml,sha256=Qhe1gyKv_UB6Q29VAEKmo-fzasELPXyT2Tm6ymI2DcU,557
-ascend_deployer/playbooks/install/install_hccl-controller.yml,sha256=cwnYSmZ16cbjUQIOIYkFwRIGPOKYuqsAE1P31QlphN0,99
-ascend_deployer/playbooks/install/install_ief.yml,sha256=9uyGdPMqwixrRGgNnmg3XOg-GtUdu-8CzcOvquT7uuI,462
-ascend_deployer/playbooks/install/install_kernels.yml,sha256=bF9aENohNv_FCVrH-W3BgB3e7954HQqpOCoeiQwc1nk,102
-ascend_deployer/playbooks/install/install_mindio.yml,sha256=vVa7VBXcez8tSdn2SZ043kzzWCNeTDHNi_fVFv-ZMAo,101
-ascend_deployer/playbooks/install/install_mindspore.yml,sha256=ES_cvT_lIMsxdW0NVsQMgoxUdu1a-JZ5X91npdEGGuA,927
-ascend_deployer/playbooks/install/install_mindstudio.yml,sha256=Oj1jshvM3OuXMTRZYoIq_g2wi_G4eD9KQPmo53Qm5gA,6464
-ascend_deployer/playbooks/install/install_nnae.yml,sha256=Uxp-GvbbdcBe7c7vHRnuS10u804G0z2WA867bfMSYwk,96
-ascend_deployer/playbooks/install/install_nnrt.yml,sha256=ZCDbGvDDro7kHE5toYoY2uwPLSHbniv8LV81nzyDves,96
-ascend_deployer/playbooks/install/install_noded.yml,sha256=kBFswQNjODf6ULxhFPBwKzoKyzjM-TN89tFKAuwUlvs,100
-ascend_deployer/playbooks/install/install_npu-exporter.yml,sha256=Ky0j_AypNX-YgBr480eUtZy3sR-EnT9pmKPf5P3G6Wk,107
-ascend_deployer/playbooks/install/install_npu.yml,sha256=WP7-_H0GRGoM2ei9Lb05exf_LWIBiEZ65533Ia5PTIc,1398
-ascend_deployer/playbooks/install/install_python.yml,sha256=62I2D8DdE178Mum9k32gTFCNPXsMeGB5bA0RbSIe5iM,105
-ascend_deployer/playbooks/install/install_pytorch.yml,sha256=eD5gHLXUKK5ZcQzou0CPyDGcx2uoShhjs5keYbGg2oc,2728
-ascend_deployer/playbooks/install/install_resilience-controller.yml,sha256=WOkqOqkm_YHJcdlj5Ri5byFUFVOo9IcorNFpx1XTqqE,116
-ascend_deployer/playbooks/install/install_sys_pkg.yml,sha256=3DfUzjDrnSC_qsE2gZ7Y2oq7Xohy69TeCJuKok_Fjos,487
-ascend_deployer/playbooks/install/install_tensorflow.yml,sha256=9OEUs9N5gQ20F79pTpqQ08mtx5C3uioOOV9T5YjnCsc,3278
-ascend_deployer/playbooks/install/install_tfplugin.yml,sha256=gVqt5EkpXApkLxeG8KBx87oGraCpkF3hfgoJenXSsAM,104
-ascend_deployer/playbooks/install/install_toolbox.yml,sha256=V5aXG6MHAyNbh1N6HQF1h5E69yBEwz8MsZMT7LBuwxU,102
-ascend_deployer/playbooks/install/install_toolkit.yml,sha256=RDgRmGKLBjHKfx0D8Caq1U22QxcBoSPXZfVHqTjOzHk,102
-ascend_deployer/playbooks/install/install_volcano.yml,sha256=rA-OvYCbwbF_vkW3LfAppew5skvWa6GX6DyTLqopTAM,115
-ascend_deployer/playbooks/install/task_atlasedge.yml,sha256=LX8UDMiPLO4vQatAJzBxd1dgeqZPadVhvDc31icPDJg,1490
-ascend_deployer/playbooks/install/task_cmake.yml,sha256=ue2t4_13xOEt9nRbEt6iCRHemHDH8_FaNz4doUAfhq0,663
-ascend_deployer/playbooks/install/task_dl.yml,sha256=uJWV5PKylc7tC3QKZ7QIEPFqRI_B29o0s8ezRX0bKNk,995
-ascend_deployer/playbooks/install/task_docker_images.yml,sha256=16iwil91p9Xo0l3dBZruEo-RotRpBEJsAWxjyCJLrPg,818
-ascend_deployer/playbooks/install/task_driver.yml,sha256=lhdY26x4-h2z6czLYYbwDbXYMTcGd94b2QYCX_se83E,81
-ascend_deployer/playbooks/install/task_driver_common.yml,sha256=rF4AG89228oQquHBOPYbrE7T5lmvyAnFmBrqsWUM8PM,6900
-ascend_deployer/playbooks/install/task_firmware.yml,sha256=Wc-d8DzsZNEo5xxd10kDXYqtv0x4bjBN7FxNkr1VBUk,6419
-ascend_deployer/playbooks/install/task_gcc.yml,sha256=nPcCmo6N30E00uV9-8vpokgLA06uetpbc81Whfl_yas,2210
-ascend_deployer/playbooks/install/task_get_npu_scene.yml,sha256=aa6P4mAcn9ExFxEwCOyg8leM7dssZbQC3FWMo-c_OdQ,3055
-ascend_deployer/playbooks/install/task_ha.yml,sha256=8VXkImxzfc08Wbobj_eAOE8Pos64-ifN_HqKrmF759o,1253
+ascend_deployer/playbooks/install/install_ascend-device-plugin.yml,sha256=A0Zwz4G5mwHQs3Ob-IcK5FKtSYynRuQpgjQxoEh5_6w,2262
+ascend_deployer/playbooks/install/install_ascend-docker-runtime.yml,sha256=f6ovxqqyXpgVmy7TTWgoSWQFHD0SH0ISEDZemSrRl4w,172
+ascend_deployer/playbooks/install/install_ascend-operator.yml,sha256=ocg8voR100giWZJ3z4CRxS4HVQ3upe7DkFYntgwEol4,2273
+ascend_deployer/playbooks/install/install_atlasedge.yml,sha256=CVHIVRCQcevv5Z8e7ET7OFhpuYOpewRn2u9yjhOwM70,646
+ascend_deployer/playbooks/install/install_docker_images.yml,sha256=P_ZwdQ3X4CgsKkGGgQwVf6VRWb0WTXE0drIR0prZS4Q,532
+ascend_deployer/playbooks/install/install_driver.yml,sha256=g6zOjP8FPssd1fNr8vrXvFHuRyDh0XsMQ6-hsCkmTsM,11
+ascend_deployer/playbooks/install/install_firmware.yml,sha256=oGKk0eGVsvh5jRAIwtSLsRijERVvGd8SmBCh5OUVRFQ,12
+ascend_deployer/playbooks/install/install_ha.yml,sha256=4W8jyPLZApW1Q0xrXNmUZZWNaUSJAIOqXBIX8iwgzZc,612
+ascend_deployer/playbooks/install/install_hccl-controller.yml,sha256=kvASuLNkA4S47yZ0xwlXg-A1fPMZvCsOnHDkGsLpRKA,2273
+ascend_deployer/playbooks/install/install_ief.yml,sha256=4II1u1ngMvCdkUTpQM8cmC2nLuaPXb82V79o5wMLOuY,482
+ascend_deployer/playbooks/install/install_kernels.yml,sha256=Qx5AuUxoVDgeMGsfn93UOvUXeVrjEl6_UI2ZGXF0ZmA,476
+ascend_deployer/playbooks/install/install_mindio.yml,sha256=hWiFPMfeeONVsK50-W5kqN-UjV2QMbPksvnJCSe1vyU,649
+ascend_deployer/playbooks/install/install_mindspore.yml,sha256=BnEM2vpmjD-gzZqj_363eOn6Ce9t-jkrQHen-YEOpeI,284
+ascend_deployer/playbooks/install/install_mindstudio.yml,sha256=plMYzDq5ePTmzTgUnyZ13SXyQUUnBaUJR2ERA8g7CgA,6672
+ascend_deployer/playbooks/install/install_nnae.yml,sha256=gKwwNE03Lg3QwCUCZrFU9J7BbuFkpcLnUl8oXTEtsiU,441
+ascend_deployer/playbooks/install/install_nnrt.yml,sha256=C9e4sQSMPKFIS4ZnD-PIkPotmNlKgBmgbn3esNR-ydc,441
+ascend_deployer/playbooks/install/install_noded.yml,sha256=6umLsmf9_ur4GmaTa0DeAvPITPYFDAXXIVs4LbfLlBc,2113
+ascend_deployer/playbooks/install/install_npu-exporter.yml,sha256=_QphQGiTn2mFe64tUOAxMBJfS2A_HGtoIDSp4m3nJvk,2225
+ascend_deployer/playbooks/install/install_npu.yml,sha256=D4nSEInizN-FvoxihTIdVFt8Fnu1Eli218oEXoJz1mw,430
+ascend_deployer/playbooks/install/install_python.yml,sha256=U5DhUMi_P92WXLaQIvVrZ3teI29p0HWpGyWkZQh4MRI,238
+ascend_deployer/playbooks/install/install_pytorch.yml,sha256=OlViGzU1ZrooJuH6MNCQ912mfVh8ErNXBCFiC1D9A3c,279
+ascend_deployer/playbooks/install/install_resilience-controller.yml,sha256=DXRz-fYXCQZSKmQksEYNUVzUr7_a-ivSPPamhHfIUjQ,2369
+ascend_deployer/playbooks/install/install_sys_pkg.yml,sha256=nFTGpS0GPe-nkO2aBskebwrkz3C1LWZNVt37URKK6Bw,1225
+ascend_deployer/playbooks/install/install_tensorflow.yml,sha256=iPBbxgi0xZEq1HB6z1d9OAURbNRe2D_flRHqc908Txc,287
+ascend_deployer/playbooks/install/install_tfplugin.yml,sha256=GME6ObkZxvoptrmeppexCQkuG4iB99ES8SVe1g6zpsw,465
+ascend_deployer/playbooks/install/install_toolbox.yml,sha256=5zyb19PJrx3KEdBiK62NMJyDpxiMAEYZDq3znioU60c,459
+ascend_deployer/playbooks/install/install_toolkit.yml,sha256=1bcH3b1nmeBZRxvM5GmRwHGtv5Zrh-LfpfryDMKdbv4,498
+ascend_deployer/playbooks/install/install_volcano.yml,sha256=Ete6FkLbo8XgnesXZiQQF3WscE6VnFQnGIOlTYqhNiU,2158
+ascend_deployer/playbooks/install/task_atlasedge.yml,sha256=hoAbL8H6inWv3lVvJiCMQ2TwjtfF5jy3WlJjEyU1uC0,1527
+ascend_deployer/playbooks/install/task_dl.yml,sha256=Dzo1hwYzIdnWLqxVZX-nkXjC3XcYEM7Oq-3kcQ6sgqM,140
+ascend_deployer/playbooks/install/task_docker_images.yml,sha256=LhWEPYIRqdbHJHZvTJWnFdWJvj6LqdYocKO5Z7vaDos,733
+ascend_deployer/playbooks/install/task_ha.yml,sha256=zXu8k6z_VO6LlOnSkteQIxAI2dMcjxvIlN9MFffp80U,1343
 ascend_deployer/playbooks/install/task_ief.yml,sha256=M-BG1Imq-9jfQ0JR4Scy7l9xlld1J5YWYp3sKQNFvEA,670
 ascend_deployer/playbooks/install/task_ief_a500.yml,sha256=yguTfoZxiVjeeCNjdoB8bZNRrPimzjGuaM3fUo4nET4,2777
 ascend_deployer/playbooks/install/task_ief_a500pro.yml,sha256=Ow70QwooJge5P8NeFE17UuWx2S2Y2sWVZ6ZWbXuYBJg,1665
-ascend_deployer/playbooks/install/task_kernel.yml,sha256=CLs5wxnsJtdWb7LjWnrpsj8KqzVH8Ynn9H-H5gNnTdc,1337
-ascend_deployer/playbooks/install/task_kernel_euleros.yml,sha256=OYbrDSOwzkOCc1N3Qw-oh1ESO3V1NMNM9hN1tj8KVWw,1242
-ascend_deployer/playbooks/install/task_kernels.yml,sha256=-ZkWu_1PJDuLNCsk75jZcPO2Admn5m79iE1Wl4lmy_0,8921
-ascend_deployer/playbooks/install/task_mindspore.yml,sha256=X9lNO5rRjlVCYFpBz8j8Hjd-xYLLAa80Jn-5VQmLAGk,1273
-ascend_deployer/playbooks/install/task_mpi.yml,sha256=gscEYAQt1Why_n2xvC5kiu8OF3j-BK0IIJoYKLaVkXY,2155
-ascend_deployer/playbooks/install/task_nnae.yml,sha256=_wND24s9r44t1nIfHR1OzNa4SVj1jotp9OU9BkgwRmw,3226
-ascend_deployer/playbooks/install/task_nnrt.yml,sha256=5Hcxyxm9YTjCaNqGro2Z7IOP19OpadHVP9R4z693KaA,3232
-ascend_deployer/playbooks/install/task_protobuf.yml,sha256=wisHWXln-3KJNKNAEujdEyG4R34xd8tPie9C1JpoEPU,709
-ascend_deployer/playbooks/install/task_python.yml,sha256=8757_kb8MqLYikXQGtuTVYt6dtQGqidk9hutOUIJkUk,3209
-ascend_deployer/playbooks/install/task_pytorch.yml,sha256=g8TQRT1xDIOyKdc6CnA9AQ-yxwSjuX1-czu2TL8JzkI,1286
-ascend_deployer/playbooks/install/task_sys_apt.yml,sha256=jYzG3GbYszcfKXpaStIt-dQyN21847c4RKfXddJGseM,1812
-ascend_deployer/playbooks/install/task_sys_dnf.yml,sha256=puH6Ig-5rFtt1UO4tyrffJ9sJ_2sfdzc5yK__qzSf48,2467
-ascend_deployer/playbooks/install/task_sys_pkg.yml,sha256=Zmd3Rur7yinlJlAw_KQxzPPrSkWy74I3h7a6ixRLDGU,3557
-ascend_deployer/playbooks/install/task_sys_yum.yml,sha256=DPq_QvIXmN461TSGj66B2E4sz6sDnrHs0xgxfyVjdak,3113
-ascend_deployer/playbooks/install/task_tensorflow.yml,sha256=-JHHIg7YlvxPHe7zzDn3pXY2hbRH9in_21SmuWOHuIA,1073
-ascend_deployer/playbooks/install/task_tfplugin.yml,sha256=WasY4j1HGRUiaX45aEaHFmJRyslr58LE60GQFDKKMtA,3436
-ascend_deployer/playbooks/install/task_toolbox.yml,sha256=OtwHakCgztM_fQHcDJgYVn0ILEaxFCKE7XxLRSsNvc8,3329
-ascend_deployer/playbooks/install/task_toolkit.yml,sha256=drixSiySlgoamLy2tRgGlFsYagbEHEEdnfbDmrYCZQk,6600
-ascend_deployer/playbooks/install/patch/install_nnae.yml,sha256=Bjt_L7j-afhIo4wNzHYz-x8tGdk4JJZDzEjI_bTEgU0,102
-ascend_deployer/playbooks/install/patch/install_nnrt.yml,sha256=ltW42VyV6193wq1IYHMEV_Jv-rZPAXlyMVOaZ9MyNSQ,102
-ascend_deployer/playbooks/install/patch/install_tfplugin.yml,sha256=aly9mNlv0lFBjLNpyS_IhiFJiRs3l4Ob3ImtAJcsavI,110
-ascend_deployer/playbooks/install/patch/install_toolkit.yml,sha256=mS-UW0JeNbxLTBvadmAkZsVKFGk4q-Pfb5V9b9Lc0do,108
-ascend_deployer/playbooks/install/patch/rollback_nnae.yml,sha256=8ZcPKniMaYMUS5LvCRrMf2kuAHPJnnnI6p-XzryA4IU,106
-ascend_deployer/playbooks/install/patch/rollback_nnrt.yml,sha256=YzUDHNq4aINfO3T4Fy6jQYiM1R4D9kE3r9xTipia9qM,106
-ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml,sha256=w7KvXXOjckJpCdxRinjdNLM9QslTwsm7kddO-2a8CT0,114
-ascend_deployer/playbooks/install/patch/rollback_toolkit.yml,sha256=IzqjJTqQg3FMTbQB1ZZ3GNk4-nLb_bifyWLyjKgGvoY,112
-ascend_deployer/playbooks/install/patch/task_nnae.yml,sha256=yVzJo6n_GKl-Z8QMK8c84VbMjws06qVYZb8286XJC6M,1378
-ascend_deployer/playbooks/install/patch/task_nnrt.yml,sha256=KnlWAaXty8QLg3Gc3dmulatDXJQRXOA1fnL6nt6947Q,1378
-ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml,sha256=BAzxKjDnjsDnRljiyirXNqUPkjZj3JycoUYpSCR5c6o,663
-ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml,sha256=OnDd3YMSyaeby6qGP6CBxTZBF1E85UV0GqxU64erwZg,1680
-ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml,sha256=ji58LL9mv5It7C-_dagH7XvPvmmOCOfLEawLjCaliNY,726
-ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml,sha256=J3qsAC8Qh8IM9IFvbh00Ky49g1_wyyLzb6tzeOY9npc,1693
-ascend_deployer/playbooks/install/patch/task_tfplugin.yml,sha256=HPAombQW9Zw59HWRx5ZMdvgtR1ZXH2RGaaPfhscd6Qw,1445
-ascend_deployer/playbooks/install/patch/task_toolkit.yml,sha256=5O74rEJRPESnXOg1haaMmCPLIukwTDVT1ii-BBQ33Io,1285
-ascend_deployer/playbooks/process/process_check.yml,sha256=iDv0yzMTVaBYtMEZpditZr5Pf2xECbxhTMl7TXgPijg,369
-ascend_deployer/playbooks/process/process_install.yml,sha256=R_cElyt26268N8qOqMHnaM38tHDsnYFlXbDDSqu0U3A,3765
-ascend_deployer/playbooks/process/process_patch.yml,sha256=V6zDjtcRbkwew51LTUvbd-HmvgD7ojnCjSyMNTv-1V0,783
-ascend_deployer/playbooks/process/process_patch_rollback.yml,sha256=do01GGNQJRQXMbWdBpktQreDfI4GIIIJtOLuVlsIg88,787
-ascend_deployer/playbooks/process/process_scene.yml,sha256=tJsnA2JKzd5_W2JJ57TqdljcPjy_S5AvJGSTqhUJV48,2144
-ascend_deployer/playbooks/process/process_test.yml,sha256=ZwAZx62Tr85jRZU3jOjg23hReUQlqgPk5taZ0xIFpNM,1049
-ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml,sha256=IzTusCwr2j72btMbBnQGyhTowU5qiExBAfefor3W_AY,312
-ascend_deployer/playbooks/roles/mindx.basic/files/space.sh,sha256=sweRsZwzkCcoCWy5iWd2msj4oJdop3OraLOde-vytG0,1258
-ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml,sha256=oZhZG9mIeYOjRuh52eWhgGcgMkGUUfln5-DJxjMSFP0,2771
-ascend_deployer/playbooks/roles/mindx.basic/tasks/check_driver.yml,sha256=1-SsuhY_ajfzKKv2Ri9uVnrbwrRo1Nrgmor7Rkxwbdw,1378
-ascend_deployer/playbooks/roles/mindx.basic/tasks/get_k8s_version.yml,sha256=Uw9P55wHMM7ModlT2UguDEX_q1SJAXsoNU51Hs7o94o,1392
-ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml,sha256=oV_W7AZh006F2NWqMpg4OOME-1rDYtbQaJ4XskEzMkQ,2256
-ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml,sha256=wej99jUbO2gDAp7BNbw34jQgMJy8G5itmoAQJJMnykQ,4784
-ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml,sha256=NYYrJKbJwsDC_mqbDhOKZrbQxYj73gwpYnDVPfxfDXo,4892
-ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml,sha256=Ox7iYNp85o3s2Pbe40e6tjEFK6BMXF6eALarhq74LGQ,13754
-ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml,sha256=ZSUXe5ifcgEI_kVGuatvm-VPRJxpkxAMA0kPAFqpG1o,335
-ascend_deployer/playbooks/roles/mindx.dl/README.md,sha256=zVYAP3TfVYfVeqkuiCUs0hnhSID2Vx7xLc4ObZvIMnw,76
-ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml,sha256=0pa35fkGsNXf0_aHusnywN7hof4CRMKRoNr5wsp5BIk,1379
-ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml,sha256=e4vPgX79HlfSjygJhGVEQT_g3qIMPWhV5P2j3D3t1rM,181
-ascend_deployer/playbooks/roles/mindx.dl/tasks/ascend-operator.yaml,sha256=_su0UYaIhMApQS18n3mob59AR2b6QXJaANUw-WNrkk0,5474
-ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml,sha256=E6dIhOulsphnNpOuvQ_x6SMtGp5ATl23IWvkdUnuDJU,11032
-ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml,sha256=PfNpGclq1umyPnX0mc_nvi9tj6DZpVEEJBx6pbz-Nrk,675
-ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml,sha256=RhZgxqWY5-xJyObFOQdLxeylS2VPNeE2l3raHVslJXM,9970
-ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml,sha256=lY6FKiV1pDzwehqQeQhbCzN1XXnDoRT6rYd8SEUC6R0,7728
-ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml,sha256=Zp8jlSKUxoItXkSdHyA186EpcEYvqdFRG5WF1Xud45U,510
-ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml,sha256=8YZa5JohfX-D0wK9qT_KxyYYyGIYHu5nt7iR-z5xYSc,1673
-ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml,sha256=dshbxDHaz_0QW8VRGZ3LZnYeD_5S_KkC8LPiKi5f9Fw,5087
-ascend_deployer/playbooks/roles/mindx.dl/tasks/label_master.yaml,sha256=Q1H0lgP2UoOAm4X7FCLb7W-bk1UwD88zkhFkaLEfzQU,324
-ascend_deployer/playbooks/roles/mindx.dl/tasks/label_worker.yaml,sha256=RpTE3pw9_DC-OF3kClb6ngGvXDZO0fJi29yYmf0wD_s,5357
-ascend_deployer/playbooks/roles/mindx.dl/tasks/mindio.yaml,sha256=sSrFjbxGFuRzlYw1EJZeyR89M6VmWpa7AurR9xOJIGA,3083
-ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml,sha256=BROy3CKkXmax450cCRTVgArjMj1MpL7Hexuij1OkR_w,5118
-ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml,sha256=6t3b93FrJepVmD2JGoxnBCGHQ01_cTV0Cxy0GGqXlyg,4808
-ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml,sha256=zVRNFUE_7GUMTi5Vo93ff0hqf54qg5VWRAExOLDUbcY,3874
-ascend_deployer/playbooks/roles/mindx.dl/tasks/resilience-controller.yaml,sha256=aDvwp_NEVaa_hPfxdAmLYOY89DvkFIVRll9Iv0HI4Qc,5747
-ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml,sha256=uDJVpxNItNlp9hgmdWdXfy5S95ir4ATWLSRJ7Sdr9GI,5981
-ascend_deployer/playbooks/roles/mindx.dl/templates/drc.conf,sha256=DU6n_X5-CMgdlrUEhBd3-Mk-MjlYbQTOoFssgA0tnws,1259
-ascend_deployer/playbooks/roles/mindx.dl/templates/memfs.conf,sha256=upaag7G-TWs3fpAn2ZOQ283qgGMkiN4goZS3Ffh_CuI,1038
-ascend_deployer/playbooks/roles/mindx.dl/templates/ockiod.conf,sha256=MagWbgcVnFuug2HqurpbooFuWV3BnC8ZWGVzK2_FxMY,110
+ascend_deployer/playbooks/install/patch/install_nnae.yml,sha256=8TaVSG79WiEZ_0AnlBjMAeOSnWLsEQs30HJOxufi_pQ,477
+ascend_deployer/playbooks/install/patch/install_nnrt.yml,sha256=x1ShbtQ-oJUS9OyDkRQp4z3TRNXxbOWV0tqTkVXCDps,477
+ascend_deployer/playbooks/install/patch/install_tfplugin.yml,sha256=m6JNthkp5_1N42zA6fLXIfX0TdbkKBLMjRVzUfISkfM,501
+ascend_deployer/playbooks/install/patch/install_toolkit.yml,sha256=SgmkxJ9jjKGKMXD3_CGbHvFtG53armv7M6T3k5jHVDk,495
+ascend_deployer/playbooks/install/patch/rollback_nnae.yml,sha256=ko5xTN0jgcNfzb9KphFf3NJUKb-Xucze3b9UQq6mEQg,470
+ascend_deployer/playbooks/install/patch/rollback_nnrt.yml,sha256=zihfZslOxz8Ta_D_2MAbFl4MS4vFm1QWP_ob-P8nlSA,470
+ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml,sha256=AKpSOguy_37asvxhKa87fI8jfEA8s8mb3TTdWxwrvNU,494
+ascend_deployer/playbooks/install/patch/rollback_toolkit.yml,sha256=EMoc3BUbmBsKpyq5HGHu14T1lY2d7dn8vol4jynABfg,488
+ascend_deployer/playbooks/process/process_check.yml,sha256=8xwDGMIcl-trusxo5RU8o2CABBri2m2IA1gZ2FNzaIo,135
+ascend_deployer/playbooks/process/process_install.yml,sha256=VU_JPB0dwkYCjKo9yhEgKly7566FZHLVPZbxagEMcsQ,3004
+ascend_deployer/playbooks/process/process_patch.yml,sha256=DTibIv5nhyioWlkYH3F_fxzOChrSbtff1U_0qXffEP4,647
+ascend_deployer/playbooks/process/process_patch_rollback.yml,sha256=iEgIckbSmlLwp6D-ve5UjN1mviXxlNnZlr1BTu8Dv98,651
+ascend_deployer/playbooks/process/process_scene.yml,sha256=wC7mIxc7eh1daKBebZ-rufmy8-M8XYHr1eU2IOsSQ_I,1401
+ascend_deployer/playbooks/process/process_test.yml,sha256=5qqcQYOajTV3sIxoSAJpludR_jdXl2KRAbvqcD_47Wc,265
 ascend_deployer/playbooks/roles/mindx.docker/README.md,sha256=_rk-uEyhUIyM1X9hFmBoR0cVNsCPjaFutgnLGY7Jnk8,67
 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml,sha256=HIK4udfQ5FIDSBZCHGmRI2fXksD_gpJZaYmTy6_s6ZQ,171
 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml,sha256=RzHpMKtHxNdDl0aEsvOIl96NXzOXKtQRCxFkKuuxdwc,347
-ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml,sha256=j8wMPI5_9498O-jVrvSbpONp96Jr-ODqYVdtF8Qya0A,418
-ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml,sha256=W3_xcU4vILSvjiAfLp15c-xU8v2iyIgj_W1TzLHXqY0,474
+ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml,sha256=jHxGiU73jvxFK2ikseSTQgmwKVjvcp6zm8TF9Dewxo0,422
+ascend_deployer/playbooks/roles/mindx.docker/tasks/install_containerd.yml,sha256=RuBmdNk-6jxNgWWXLsAGf_qi_k7z_42ogOubfKLsUyU,1217
 ascend_deployer/playbooks/roles/mindx.docker/tasks/install_nerdctl.yml,sha256=C3mBkCIWDFmN8owVYXhdp8_oOQd6irMZe9WoFeCE4V0,1085
-ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml,sha256=Aoz2pzP4XWsVn_84DRxCPIwngwPOrpEzD5RJ7BxXZUE,1135
+ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml,sha256=1-3yeNbC72D9qt_BzIXc-MbhVKam8HZaLR3audO0LY0,1382
 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml,sha256=bXsWWUxC9WmfBUZCmT6eMS8daSSVkjCEl-5lpUAuZ5w,1160
 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml,sha256=viaIim_7LKiJwaTyFnu7AxKsHI9D-LB8H6k83Xj3U1o,272
-ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml,sha256=O-OHocr3VY8qFwybYKvzCrj5c5kRZyUujncLhBxllBg,1314
-ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml,sha256=wDiwJIfN95dQ0PXvQv_UDxw6Kzr6bZghpxwZAhnUKqg,1158
-ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml,sha256=t5N9tSuXR8MEo45hOr-6v-iTobl68LxBDXmxDHtqJwE,346
-ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml,sha256=UWzlh9VhrttEXCzhl6NBTgna5ZqoO3_mfU50iLIXh5U,1382
-ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml,sha256=hb6M4EeVx8416XPO-nIwpyHRW7V2iZsnMeVrLig_JgA,42
-ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml,sha256=gcYRvJyZwKRPhwYtvI8tXAayaSRrOWzJNWXgJVzk10E,1723
+ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml,sha256=w7gAaboDMeK00EyHCe-MFqqO-rCM9fOsRiDWFnx3cZw,979
 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml,sha256=WNOEhlXVDW5t0KAdO392ljVs_ne93Q1Tm-YmMbzGHxY,660
 ascend_deployer/playbooks/roles/mindx.k8s/README.md,sha256=yEssYhqELC5UiHFN7ooAN3vB48OZIc4EHaMucUfvQSE,536
 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml,sha256=k3F1-Ebg2zDZ5s7WrEWksEsRYxa28HdnC_oyp7Bg_mY,400
 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf,sha256=ICh5R0gs5GbvEdItYXv4XzgVOOsPKjdNjqQmBxzYyTI,929
 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service,sha256=SMj1pqE9QXn-FW9IExZ6WQF3z92nPBuWgf7H49FZtwk,283
 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml,sha256=BRFTshnlZZPPYEvfccG4xZD4bvRLfA5JoWfEl2UZcIE,179
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml,sha256=1PCjhnosJZnTMAQwbRckw9pujMCWyNfGzgt4DXnDtRs,691
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml,sha256=QLPzPtv6SqVhbsuqXmBoTkyQLFeOS1frr-zlIiXXSog,1008
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml,sha256=vEN389NHfkegFNqf1621Dorujrf8-9SCJB_kmMmvaM8,774
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml,sha256=8JBmDVbJGqoEoZfXUseU84E7qTZE25ioKqp4zep68AY,1251
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml,sha256=JDuIEAbirW-tCUHtuIYUhX5O3Lleq1sdTYdtZocrFfQ,1237
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml,sha256=K2_3bRFykJ1Z1uIm4RF6LawdmCe67FLGXpATp3ZAOcU,1119
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml,sha256=vCmEAJBwbRfAmDRw1UeovfdV63ij6huI-Smb77u2m1M,882
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml,sha256=BUI9SMBBPqqxU-Z0XhAXVOVHbOGH9DdHEoyQtOZ1FJ4,1309
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml,sha256=3_rqb7KJUHJjw92a0fgWOnEX8pD_ZJUdZ8sdnDC58zY,1119
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml,sha256=BnfZwRtLBw95V7bnsM-Zz3hou_JG5Nx_9StCNBlEVqI,1032
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml,sha256=iKLtbuX9miYSPEgn2FMX8YAlDA3ojwd_Ky1T4J44dTo,4329
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml,sha256=YyGudJgJwUASMteByci0M-6xP8p93vSe1Eh874skyY8,2000
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml,sha256=5mByGipzZebiV_N39zAQXTTOOMzBQB3ZgBugiOw9My0,3854
-ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml,sha256=FRQF-koBAF1Ymq-s3zktISetW6k9S5H10zerc4qBzGQ,1852
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml,sha256=H3fgP2_Wa5nk4hhT0nf1Tm1i12GsvL_8NtoTGyv8qPc,4329
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml,sha256=fk2Ci7DklC4HhmH8YAL2hZokm5ejBfFJl52DzHmkjHw,2002
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml,sha256=pvgMcurrwYO7kiWdQhgepX58jGwFicZwZoeYtCjypak,4102
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml,sha256=mdrvL_ncTtiy4_4HE1r5-h-xs3Rg_jmerB8jy7YZxEc,1856
 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml,sha256=9c5hE8eJWjhGSqT60_Z-2ikOaobRI0C5_AQ926Xyipw,860
 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml,sha256=0IuV_4dsttpiTK0gmRZrINL22Gj6-pW1nW553aT1naw,202740
 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.25.0.ipv6.yaml,sha256=X4XSqjEOEnpjJ1HVVzKm1YD7f90Iv_g3mRT17nKK60g,237804
 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml,sha256=IONjdNOyHi_HRTQ3OCRmkH0YKP5Dife6RKk6UXYQKps,539
@@ -392,107 +360,60 @@
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml,sha256=vCVJRNNwuleGKWaoYz77DEYDst8Uv_Sw3lDfgV1EwAw,1896
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml,sha256=ImwcEivucISHilWW2Qcf2YJcHF6O7XICmwzNq6MNcZw,8715
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml,sha256=XXm1lB_aU1KOshj1Fi9if2jA98pMFdu1ISNbg-vvyy4,10576
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml,sha256=h6btWq1S2NXWFLJUyIdaSSjpo699-ovF-nI_oWWqWxY,1877
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml,sha256=nry_fOwbj5epjvzi9ItjdwwCHudYz3NcGt84KHrlk5g,2443
 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml,sha256=K2QGKpuGUgDuK5EbsWI5UTXaGwu_-TS8sOfcLslXvYo,1355
 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml,sha256=EfM1TxOjLrD1JvVMnJI0hOrGGGXW8ukPeFU-i4CvVg4,176
-ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml,sha256=ZiqXi72yhiis53M7x4jUcCSPMFpN_YChdpEf7-8cGtw,4514
-ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml,sha256=a5xqx4dWRzMmrNs99mpt875vWZVqixR1y6wYz-0CE8E,144
-ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py,sha256=5EibqtBrQ7PwjhCAfPC_yh5NNnf-5TWOAx5ebT8pX-Q,591
-ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml,sha256=OH8Z5RkTLftQg0gH3F63_RZJ7e99QRjXCtCVbxBc4qc,2537
-ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py,sha256=iO4SIXdJYGqHfv9RlQ1gevZ6fPyaCxf25nOxAzWkwso,2640
-ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py,sha256=1tnSrB6JbZnadNBoThabIaIh9Eal_nakWqIzzQrT9o4,8253
-ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml,sha256=qBqt1GnH0oh1LqkigfvAEmigqQjQilqasLRzqqfh_vw,1368
-ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py,sha256=OvrgopyALQuaxYVSG--Qytc1m2QDPtjggaj4bVpGqek,1012
-ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py,sha256=W0gdfG9JksCkYJQIS-XZyBdvCTXQbqRNyXX0oV-UUSs,786
-ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml,sha256=RB3g8mZOd5PBxZcGyk0E0OvNXefrYpG0XCdxdd5gpN8,2037
+ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml,sha256=1hgPjH7aq4pV0obpcfRIdcPqkVksAM2eKBEzNFJDtFI,4530
 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml,sha256=JDDiO0oedEzlSRz1uNeBPMrhWw86vhNtI2fN4PgKT7Q,389
 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml,sha256=z55v95_ueyFs3zQmUnkRt9ixoZcCZI0PsjD-w3ULxHM,390
 ascend_deployer/playbooks/scene/scene_auto.yml,sha256=tEPEu4K10RQZS3yw41r_Xjmt2vatlecQeIqPytSc6Bo,960
-ascend_deployer/playbooks/scene/scene_dl.yml,sha256=C5drgWAcympg1E478-1vde4HTZyCQFzhuCtpis89Q7w,613
+ascend_deployer/playbooks/scene/scene_dl.yml,sha256=vi3RImiKf0r_MBUfX1tuINRm_k3Xj4-wxWxh0lnJrlE,1303
 ascend_deployer/playbooks/scene/scene_edge.yml,sha256=w3idz1HuKo6qKcJr-m44iTDOP4wOiBYdQlXvCDSsUYw,259
-ascend_deployer/playbooks/scene/scene_mef.yml,sha256=NKt6EfP6KzfiDG8fI96TIRrsQnGDohLKcRVIZlt3qko,361
+ascend_deployer/playbooks/scene/scene_mef.yml,sha256=sqebgYTJAeIGH0rHKth6ixeAtRTsk4EesFD7u97biLQ,306
 ascend_deployer/playbooks/scene/scene_mindspore.yml,sha256=N8jl61OrdJ3Petl0irWUEXiDX4brIScPLa5il-UDNAw,514
 ascend_deployer/playbooks/scene/scene_offline_dev.yml,sha256=SEO7UmhRiBtoN_n9HJJyXaJs7bGe2BRR6pyYHI0OBkc,435
 ascend_deployer/playbooks/scene/scene_offline_run.yml,sha256=6aD5f1mua65hL8tB4osBmElFkW88PYosFsmR4OFYN1s,354
 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml,sha256=jC69LyU98npgE1GIHMwaAvBKj5hnWQkeqNou5jdXr0I,510
 ascend_deployer/playbooks/scene/scene_pytorch_run.yml,sha256=em4k3qeeh_-qN8n-QJ2Oh1DQMUU9slsOTdg29eoUBkw,504
 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml,sha256=D4_mrI4NKLMD_4fsC7Njb2op103Ym9TzLVwaBlT65Xg,593
 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml,sha256=usd-zORtPFqmsHEz3I1EMsCsvhm383eo2-EY2v8_BJg,587
 ascend_deployer/playbooks/scene/scene_vmhost.yml,sha256=g9ffCyxfOnsgTkUW3lwmYaps9ndwpTOqsy_MQtQA6Y4,273
-ascend_deployer/playbooks/test/case_driver.yml,sha256=98ujuNmsUjN7dRNtOK8DgHiROulrrQ-BwaGqjZZdeRE,2673
-ascend_deployer/playbooks/test/case_firmware.yml,sha256=c7QHUM6jcxSC6okYMneNKimOPz6uw4YmGV65SW3T-so,1169
-ascend_deployer/playbooks/test/case_mindspore.yml,sha256=0iIbZctMK3pyc8iN3EPUj5hIQ32BguP6rFtnRTsKO4M,3166
-ascend_deployer/playbooks/test/case_nnae.yml,sha256=c1hMdLz61GNqYLrmHSbXlg0nqGZCgjFxLU5LUbgAyJA,1049
-ascend_deployer/playbooks/test/case_nnrt.yml,sha256=2yVhpeY4tkTNdDMTVfgvZqXBsrqFl8x1sKR1reXZLG8,1047
-ascend_deployer/playbooks/test/case_pytorch.yml,sha256=V5DfpiUFDQs0xgJko3Zuq7MTsEyi_C3iddQ0vh01PGk,3619
-ascend_deployer/playbooks/test/case_tensorflow.yml,sha256=TuIGTXBauMPCwof67YYTxPajEVVgdMvPGoit1wkbaWc,7799
-ascend_deployer/playbooks/test/case_tfplugin.yml,sha256=jRIbvUbWXDlePFtj_rwsTEMHqEMI0Oi05BcAkLnZ69M,545
-ascend_deployer/playbooks/test/case_toolbox.yml,sha256=wjoHGWj2I1MjXBC01m4sjVJ3C_XYw9RRTYghQPkyNCk,1473
-ascend_deployer/playbooks/test/case_toolkit.yml,sha256=CjXtT2tmyA_8rgNMZ06PEUFEyYo5CSr8hpo6gDldLH4,1110
-ascend_deployer/playbooks/test/test_all.yml,sha256=Iiuze5fGq9axRaPFv-fdRyFRLaCJHk4zH3FqiAyct5E,608
-ascend_deployer/playbooks/test/test_driver.yml,sha256=b5pGl8GVfIWtqKrHbXmmtcqr-mskZ0Hm5fy1_1YCHy8,284
-ascend_deployer/playbooks/test/test_exhibit.yml,sha256=W3XeZjzNcv5dRA_M6VZKYtMjkZunjWgLs0iu-YMReI0,114
-ascend_deployer/playbooks/test/test_firmware.yml,sha256=q3FlDhQiPi3VKIkQHjiPwy-bxfmAfL75hf9CzyxBL4M,284
-ascend_deployer/playbooks/test/test_mindspore.yml,sha256=mOTaFGiOm8pOmjGUwdZQl9kyU_MsdGhA_vIJyzM-vz0,99
-ascend_deployer/playbooks/test/test_nnae.yml,sha256=XoQXcfFppRtu29ntX96xbP_EmjwkplqUvGRB2HITM4A,90
-ascend_deployer/playbooks/test/test_nnrt.yml,sha256=K1VWj2uRXfKqcjuMyU2PuOqLbzstgm-S5hwz5P8t2Rc,89
-ascend_deployer/playbooks/test/test_pytorch.yml,sha256=2hZXx8jklP6bmApcRNYelFwx7i9oGEak5-_Ag0pmH0c,96
-ascend_deployer/playbooks/test/test_tensorflow.yml,sha256=xVVNWd_c0DByGfi_jnwpe6vJgDrnBdYUDwGtcPkK6Wg,101
-ascend_deployer/playbooks/test/test_tfplugin.yml,sha256=fm-IvOolhycuY45svRn-cXt3cYcnwLKYzxtObWNR7Gg,97
-ascend_deployer/playbooks/test/test_toolbox.yml,sha256=5ifAcGk0GLj1GfZD1bljSObTy0_z-ehvqKQe6CPHqJQ,104
-ascend_deployer/playbooks/test/test_toolkit.yml,sha256=YfwXJlVmRewWXuSzeUK5Mi28LfXU9ytNvWbWbXEErBo,95
+ascend_deployer/scripts/Huawei_Integrity_Root_CA_G2.pem,sha256=0hyQSjSgvM3rqbYYAnWk0L_gSpXfrAuOcOGrxFt-ZY8,2231
+ascend_deployer/scripts/Huawei_Software_Integriry_Protection_Root_CA.pem,sha256=aJRKqY3t4v6agln9x06mzCAxqQvLtP3uUob6leUO4Ns,1902
 ascend_deployer/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ascend_deployer/scripts/check_pkgs.sh,sha256=_dlp1aVtaDdLeQ3_eUGLn9OF3Y7jt8wvDtyeB6j24NE,21173
+ascend_deployer/scripts/create_report.py,sha256=gyZ6s7SfggGUQg4OlpM9k2ncP0s23hrdOqhWmqi3WyM,4096
 ascend_deployer/scripts/eula_cn.txt,sha256=515-QYXMXyjWZqidh_MTInwiHfTakBHHBE6Tdwe92Lo,11154
 ascend_deployer/scripts/eula_en.txt,sha256=8_K9VaKUgq83YjFr0CMB5cyd22djCrE0M6o57IeQkeA,12908
-ascend_deployer/scripts/hccn_set.sh,sha256=j8oTcJmKe9fa6_Gm4lsIMBFQIeSUCXJJFNoTFOdOo-0,1116
 ascend_deployer/scripts/image_load.sh,sha256=HGNiBn8EXoVrqyxPBit7NlHLwwbWN6sd_BBhXyV09SI,1104
-ascend_deployer/scripts/install.sh,sha256=u-mtTLGfx_0FOuqrF0qV2QZD_oFwDeDf6_XMlNFiZ4g,969
-ascend_deployer/scripts/install_ansible.sh,sha256=DEXh1Acvs3gheDoVN8tuIKV8h_Tg9oHJpppnvxQ1Dhs,3587
-ascend_deployer/scripts/nexus.py,sha256=wRI3bHanscKVb4FtyhMuwltmKSfuV1QZi_Mif_HWZS0,16509
-ascend_deployer/scripts/nexus_config.json,sha256=7JA9kdW_SmIAy_x8k5F6ce__mv0LHlg9oxIp9bf2OVE,1380
-ascend_deployer/scripts/prepare.sh,sha256=U7WcT8f6z0Ek7P-goBIlrFPl8Wu3r3J1b0-hsWrnNiY,15205
+ascend_deployer/scripts/k8s_rep.py,sha256=RymaPfqyPQtyAcqLIo5H0LMV8iiQDzC1KkeiVHNGVCM,8938
+ascend_deployer/scripts/nexus.py,sha256=ta2xarlSNhlV2Sf4nDIkbjfgj44L-bKGS4JT5tABxBo,15500
+ascend_deployer/scripts/nexus_config.json,sha256=KpYIimaRMKuKq9RsXrr1a2Qycn3svSXkBzNHB_gh3yU,1350
+ascend_deployer/scripts/pkg_utils.py,sha256=xeV4uk19CcPbXxgJwT2rop9NMqxYu-l--vD8ibH_fWM,8712
 ascend_deployer/scripts/uninstall_k8s_docker.sh,sha256=nSY6GniAuiaDI3Emj-BCRY38IRPHklYZ2OIMDgDVf90,535
 ascend_deployer/scripts/uninstall_mef_kubeedge.sh,sha256=8g3Yni8tl1Rgy5slpNIqdJozZcmp5O9x0b7TBAjX2j4,643
 ascend_deployer/scripts/uninstall_mef_related.sh,sha256=7tu9AcnPMxpbsjBMicW3udsKn8_aIcA9Za9h75xp11c,679
-ascend_deployer/scripts/utils.sh,sha256=sHVwhZydgv2vF1GQ9QBPjWwCtWccb_Q5IGSeIbjWaOA,5723
-ascend_deployer/tools/DeviceIP-conf.sh,sha256=R74aTgi2D2TqggSvXLj6tViTC7FwTODvA5rSx26eCW8,10900
-ascend_deployer/tools/check.py,sha256=cu3uzA14apAt1DqK273XWkfABwxTUafDmRLN35tiI14,4049
-ascend_deployer/tools/hccn.py,sha256=LIxGwCd_Rpmc2FctlSVH0Y5ql6LCzDjZgZC6wBegamg,9718
-ascend_deployer/tools/update_crl.sh,sha256=VwBHBTughh1qOxqqurddYS37blB96iH2eTkBSHpcgaE,9930
-ascend_deployer/tools/hccn/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
-ascend_deployer/tools/hccn/main/hccn.go,sha256=robmOcfv1cHeM__UTnU2-sP6wDRBcId4UwSP8hkbGVc,6863
+ascend_deployer/templates/mindio/drc.conf,sha256=DU6n_X5-CMgdlrUEhBd3-Mk-MjlYbQTOoFssgA0tnws,1259
+ascend_deployer/templates/mindio/memfs.conf,sha256=upaag7G-TWs3fpAn2ZOQ283qgGMkiN4goZS3Ffh_CuI,1038
+ascend_deployer/templates/mindio/ockiod.conf,sha256=MagWbgcVnFuug2HqurpbooFuWV3BnC8ZWGVzK2_FxMY,110
+ascend_deployer/tools/hccn.py,sha256=qYW3xq43fEBZdz0AG3pL-XAGg5jlm3iJwoua-ER4y2w,9719
 ascend_deployer/tools/kubernetes/driver_installer/README.rst,sha256=6g3f9HHvomay5Spx1d1HFV7mDxeu2sjKdptL7f5ff7A,2373
 ascend_deployer/tools/kubernetes/driver_installer/image/dockerfile,sha256=oypbtVoYLefN2bH7NJDQOr8WmG0lPLK9vlIhVyPjSuM,314
 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/driver-install.sh,sha256=XLg214eQs1bJ6WoUz1B4JdX2dYt6lujwySNLSUEq0aA,665
 ascend_deployer/tools/kubernetes/driver_installer/install_scripts/exec.sh,sha256=w4GdyktiCES6EcQutyEuy_XAozyX5NvaBrVw0GBXV7U,1658
 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-arm-installer.yaml,sha256=15NhJ76YmmDFXDr0C3wuX0LYtE4j1TTfWfwZ7M9QntE,697
 ascend_deployer/tools/kubernetes/driver_installer/yaml/310-x86-installer.yaml,sha256=jkfclgKdP2sD3b5OExp17VixuLRgqxb0TJ4KrAw-dP4,697
 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-arm-installer.yaml,sha256=EB0hzwM7oaRY0OWQvYeqLuvGIgXIZoRRLSmNGSeWGnI,703
 ascend_deployer/tools/kubernetes/driver_installer/yaml/310P-x86-installer.yaml,sha256=vPy2C55RZ4a6EM7qaUuUcthnXf7R0hXCcyrWRjt_jvM,703
 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-arm-installer.yaml,sha256=A16A2DhirZer5GQWGJErh2KjQv1N1FQil1L9LHat20I,697
 ascend_deployer/tools/kubernetes/driver_installer/yaml/910-x86-installer.yaml,sha256=KgicmOBXdAJ_wp-6dvvG4JvBS1Y3GUvsVZ2BAT4MC7E,697
 ascend_deployer/tools/nexus/Dockerfile,sha256=r9sloQ5C5HMVo7TWnuttIcTEssUKGuG51m1BNc3hSKU,4260
-ascend_deployer/tools/report/main/go.mod,sha256=T_4E5SwIfDiUuU3LukbU4QKLaPEFaZ1lgb-GQcsNRuA,142
-ascend_deployer/tools/report/main/main.go,sha256=MnVc5U17AAEu150DdFrziPgRtfgqxLsav2PbOiagr80,18729
-ascend_deployer/tools/unzip/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
-ascend_deployer/tools/unzip/main/unzip.go,sha256=-Z0ihIicC_3GihItvhc1it3PQoyFLSz0ycGuKj82wlk,1587
-ascend_deployer/yamls/basic.yaml,sha256=LMbvOfJ78T5dXk0YEhATGNGiMe4_sSnzt6MoT_bu4I0,46
-ascend_deployer/yamls/check.yaml,sha256=74W_bQT1to6tJGK2FPrggJuFbogaAzXK7oDDLaR3xrk,46
-ascend_deployer/yamls/docker.yaml,sha256=4OEYn9_0xxyMCpl1qdJhiTZ3MctxhUdz3uXYRxzYwwY,132
-ascend_deployer/yamls/gather_facts.yaml,sha256=-LQEyu7YPjZ_BKJ9o606nkIIzWZXy4-AXjijkdTV63k,53
-ascend_deployer/yamls/harbor.yaml,sha256=4YmjA4UTdAhNLB4pH2d8G2jTnIiNELbMYY-VCqxO2y0,72
-ascend_deployer/yamls/hccn.yaml,sha256=5VuwXcGseHty7iA7s4z8YKlupyu0HRe9j_WvjLTCRKk,45
 ascend_deployer/yamls/image_load.yaml,sha256=8P1n5bl4dZo-F5Q_7-F2JIMngGnWESzEr3qzIC4JaPw,51
-ascend_deployer/yamls/k8s.yaml,sha256=OwWlFC9IPOYT-2GT4LJUYMZCC2qKSI1o9X1dw8vvEpo,126
 ascend_deployer/yamls/k8s_reset.yaml,sha256=PlvKZ3qM5U-SAyT9g-mmzWecz7fX4Q_y4_k1zbyfOTU,351
-ascend_deployer/yamls/mindxdl.yaml,sha256=xvHRj2q-tMw8G0x6CcXZ8gbdKuyEvsxEDj02u_1es4A,74
-ascend_deployer/yamls/report.yaml,sha256=OABhE8u336Y0ILTBln4mSw3s8llyDRnA1B5ZdVzmExY,47
-ascend_deployer-5.0.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ascend_deployer-5.0.6.dist-info/METADATA,sha256=iDM2tmtNlIPlDY38T4kLpXUzKFgwGRkZRP-WxKlzjjE,3227
-ascend_deployer-5.0.6.dist-info/NOTICE,sha256=nXRyXoFFIIiaatp7itl1iDhbY_0aeRJDwwoAXVWxs8Y,62
-ascend_deployer-5.0.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ascend_deployer-5.0.6.dist-info/entry_points.txt,sha256=qR3K0vWpfPNTOHJQ81nC58KRoczDpK8MiFOMOuUzL2o,128
-ascend_deployer-5.0.6.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
-ascend_deployer-5.0.6.dist-info/RECORD,,
+ascend_deployer-6.0.0b1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+ascend_deployer-6.0.0b1.dist-info/METADATA,sha256=N_GL4oob8A95IPRsJ-tNSWDzx0r8iXm1JHioYmUbaDg,2876
+ascend_deployer-6.0.0b1.dist-info/NOTICE,sha256=nXRyXoFFIIiaatp7itl1iDhbY_0aeRJDwwoAXVWxs8Y,62
+ascend_deployer-6.0.0b1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+ascend_deployer-6.0.0b1.dist-info/entry_points.txt,sha256=1tHjoPfLxJ7hy-nS1hfEQ-vBHs_80V-qiR7W1fU3YuM,129
+ascend_deployer-6.0.0b1.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
+ascend_deployer-6.0.0b1.dist-info/RECORD,,
```

