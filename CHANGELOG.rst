^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package geneus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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

