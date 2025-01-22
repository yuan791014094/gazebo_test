# gazebo_test
gazebo_test
使用到了前人的teb局部路径规划

运行时报错，错误如下
[move_base-9] process has died [pid 7115, exit code -11, cmd /opt/ros/noetic/lib/move_base/move_base __name:=move_base __log:=/home/rosnoetic/.ros/log/efc2520e-d891-11ef-9797-89ec0c40a1f9/move_base-9.log].
log file: /home/rosnoetic/.ros/log/efc2520e-d891-11ef-9797-89ec0c40a1f9/move_base-9*.log
在给定目标点时，小车会比较优秀地前往。但是在小车启动过后，一定时间内movebase节点崩溃，小车延续做崩溃时刻的动作

注意到随机生成目标版的样本很少，后续应该会添加。并且stop模型没有图片。

注意到可能存在的漏洞：目标版有小概率会生成到障碍物后面，贴的很近，导致无法被观测。
