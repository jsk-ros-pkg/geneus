^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package geneus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.2.1 (2015-04-24)
------------------
* [geneus_main.py] fix when pkg_map does not have geneus
* [geneus_main.py] Fix unexpected function resposes caused by python gabage collection algorightm
* [geneus_main.py] fix typo for warning
* [geneus_main.py] Yellow color for warnings
* Contributors: Kei Okada, Kentaro Wada

2.2.0 (2015-04-21)
------------------

* [generate.py] load roseus-add-msgs for srv too
* [geneus_main.py] add timestamp message to manifest.l

* [geneus_main.py] message loding problem https://github.com/start-jsk/2014-semi/issues/196, https://github.com/jsk-ros-pkg/jsk_roseus/issues/257

  * [geneus_main.py] gen msg/srv does not need get_pkg_map
  * [geneus_main.py] fix comment and messages
  * [geneus_main.py] use topological_order instaed of rearrange_depends
  * [geneus_main.py] use catkin as a substitute for rospkg
  * [geneus_main.py] see only run_depend in package.xml
  * [geneus_main.py] Resolve package dependencies with attention to the order

* [geneus] treat uint8[] as string like rospy https://github.com/jsk-ros-pkg/geneus/issues/14
  * [generate.py] fixed version of `#15 <https://github.com/jsk-ros-pkg/geneus/issues/15>`_ which did not pass test at  https://github.com/jsk-ros-pkg/jsk_roseus/pull/276
* [geneus_main.py] fix pakcage_dpeneds, to solve https://github.com/start-jsk/2014-semi/issues/196 issue
* [.travis.yml] use latest version of travis test
* [.travis.yml] use latest catkin for --no-jobserver option
* [.travis.yml] Add after failure
* [.gitignore] initial commit

* Contributors: Yuki Furuta Kei Okada, Kentaro Wada

2.1.2 (2015-02-25)
------------------
* [.travis.yml] remove hot-fix code
* fix not to use get_depends, which cause eerror when the package is not installed
* [package.xml] forget to add python-rospkg
* Contributors: Kei Okada

2.1.1 (2015-02-21)
------------------
* [geneus_main.py] use rospack to find build(only package have msg/src) dependency
* [.travis.yml] add test code to check work with roseus
* [src/geneus/geneus_main.py] add comments
* fix ros::load-ros-package order by dependencies
* Contributors: Kei Okada, Yuki Furuta

2.1.0 (2015-02-12)
------------------
* fix message generation for uint8(char)/int8(byte) (#4,#6)
* Contributors: Kei Okada

2.0.1 (2015-02-10)
------------------
* [scripts/gen_eus.py] set executable
* Contributors: Kei Okada

1.0.0 (2015-01-06)
------------------

0.1.0 (2014-10-02)
------------------
* rewrite everything only depends on genmsg
* Contributors: Kei Okada

