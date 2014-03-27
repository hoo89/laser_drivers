laser_drivers
=============

このパッケージは以下のURLのリポジトリのフォークです.
https://github.com/rhuitl/laser_drivers

LMS511とROS hydroで動作するようMakefile等の改変を行いました。

# How to build
$ export CC=gcc-4.4 && export CXX=g++-4.4
(gcc-4.4がインストールされていることを確認してください)
$ rosmake sicktoolbox_wrapper2

# How to use with LMS511
roscoreが動いている状態で
$ rosrun sicktoolbox_wrapper2 sicklms_5xx
と打てば、あとはトピック/scanにレーザースキャナからのスキャンデータが入ります。

スキャナのIPアドレスはドライバ中で決め打ちされているため、
変更するにはドライバを修正し再ビルドする必要があります。
 - TODO:オプションでこれを指定できるよう laser_drivers/sicktoolbox_wrapper2/ros/sicklms/*.cpp の修正
