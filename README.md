
# 1 OLDX-MocoMoco四足机器人开发平台项目  
<div align=center><img width="600" height="130" src="https://github.com/golaced/OLDX_DRONE_SIM/blob/rmd/support_file/img_file/logo.JPG"/></div>
<div align=center><img width="400" height="300" src="https://github.com/golaced/OLDX-FC_QUADRUPED_QUADROTOR/blob/rmd/support_file/img_file1/fc2.jpg"/></div>

  ____该项目是OLDX-MocoMoco四足机器人（OLDX-MocoMoco Quadruped）各版本固件和开源程序的统一管理地址。<br><br>

机器人校准视频教程：https://www.bilibili.com/video/av51043941 <br>
机器人测试视频更新地址：https://www.bilibili.com/video/av46405055  <br>
官方机架taobao链接：https://item.taobao.com/item.htm?spm=a1z10.1-c.w4004-15110596499.22.6b86242c3mvjW9&id=589551490320<br>

**-搭建该项目的方式-**

方式|说明|发货周期
-------------|-------------|-------------
整机购买(**推荐**)|从官方淘宝店购买碳素机架+已经加工好的控制器(不包含舵机)|最长半个月
机架打印+控制器购买|自行加工项目文件免费提供的3D打印机架 +从官方购买控制器+自己购买舵机|最长1周
机架打印+控制器制版加工|自行加工3D打印机架+自行制作、焊接控制器+自己购买舵机|控制器(4层板)+IMU+下载器转接+供电模块

**-开源程序与VMC机器人库-**

方式|说明|开源模式
-------------|-------------|-------------
(**VMC机器人库**)|支持多种着地反馈、动态步态调节和更稳定的姿态控制能力，需要向官方购买授权码|闭源(目前支持STM32F4系列，且库与芯片ID绑定)
开源程序|支持基础对角步态和姿态控制|开源

代码版本|开源代码说明|闭源VMC库说明
-------------|--------------|-------------
**Publish Ver1.0**|(1)虚拟力基础步态<br>  (2)梯度下降姿态解算<br>  (3)NRF射频通讯遥控<br>  (4)UCOS操作系统|(1)虚拟力+IMU自稳<br>  (2)动态步态+姿态调节
Publish Ver1.1|(1)SDK开发    |(1)SDK开发<br>	(2)自适应步频<br>	(3)平稳速度S函数切换
**Publish Ver1.2**|(1)梯度下降融合磁场+磁场干扰判断<br> (2)KF气压计高度融合<br>    (3)KF里程计位姿融合<br>    |(1)位置闭环控制+Jerk轨迹规划<br>   (2)跳跃API<br>   (3)SLIP模式<br> 	(4)梯度下降融合磁场+磁场干扰判断<br> (5)KF气压计高度融合<br>  (6)KF里程计位姿融合<br>   
**Publish Ver1.3**|   |(1)双闭环姿态控制<br>   (2)全局控制器<br>   (3)修复姿态前馈 BUG<br>   (4)修复SDK BUG<br>   
Publish Ver1.3.1|   |(1)增加模型观测器提高角速度估计可靠性，步态更加稳定<br>  (2)修复SDK BUG<br>   			
Publish Ver1.3.2|(1)增加GPS和外部罗盘驱动<br>  (2)增加SBUS遥控器控制<br>  (3)增加GPS导航<br> (4)航点写入和QG地面站Mavlink链路|	(1)增加极坐标误差修正 <br>	 (2)增加大机架参数缩放 <br>
Publish Ver1.3.3|(1)ROS下控制Node和树莓派键盘控制<br> (2)修复气压计融合引起的遥控器通讯终端|	(1)增加着地传感器提高步态稳定性 <br>
Publish Ver1.3.4|(1)增加足底传感器STL打印文件|	(1)增加自触地机制 <br> (2)增加遥控软启动<br> (3)修复BUG
Publish Ver1.3.5|(1)增加巡线SDK  <br>(2)增加无刷电机通讯控制接口 |	(1)修复BUG <br> (2)增加12Dof腿正逆解预留接口
Publish Ver1.3.6|(1)增加了使用遥控器写入参数和授权码|	(1)修复跳跃模式BUG <br> (2)修复启动站立时前后移动的BUG<br> 
Publish Ver1.3.7|(1)增加了两轴云台控制和相应的SDK (2)增大了航向控制的限制|	(1)使用了包含机体高度的倒立摆确定落足点 <br> (2)使用ESO估计角角速度进行扰动控制<br> 

百度盘地址：<br>
Ver1.3:  提取码： 17lp  链接：https://pan.baidu.com/s/12YHw7mHr14SStXLzhOFCYA  <br>
Ver1.3.1:  提取码： twvq   链接：https://pan.baidu.com/s/14chFpgKWZHjGc4xXIKb-Fw <br>
Ver1.3.2:  提取码： h0nr    链接：https://pan.baidu.com/s/1A7bbyGE4d823Yo5dpqCAoA <br>
Ver1.3.3:  提取码： f5sg    链接：https://pan.baidu.com/s/1g2UxnaU7_X75BwBaifMejw <br>
Ver1.3.4:  提取码： gkui    链接：https://pan.baidu.com/s/1IOWj-bF9VqdqwAu24S5L3Q <br>
Ver1.3.5:  提取码： rfam    链接：https://pan.baidu.com/s/1EUbEgOLhX_r8qBonZ2Ts_Q <br>
Ver1.3.6:  提取码： vq4o    链接：https://pan.baidu.com/s/12HEpyOe_MXspkF34WgIHWg <br>
Ver1.3.7:  提取码： scs1    链接：https://pan.baidu.com/s/1bRbwOFXClFw-7eHWtSQezQ <br>

<br>
Keil5环境软件下载：<br>
提取码：dxeu  链接：https://pan.baidu.com/s/1_3mZ_9vYUIQjBLj3DI84Ig <br>


**-如果该项目对您有帮助请 Star 我们的项目-**<br>
**-如果您愿意分享对该项目的优化和改进请联系golaced@163.com或加入我们的QQ群567423074，加速开源项目的进度-**<br>

<br>
**-由于本人非专业研究四足机器人，该项目只是基于个人学术水平开发并不代表目前足式机器人算法就是这样，请不要过分依赖项目内容或与正规产品对比-**<br>


# 2 捐赠与项目后续开发计划
____团队计划后期推出5kg~10kg级的足式机器人开发底盘，支持RPlidar激光雷达导航进行SLAM算法验证，能以相同的价格替代目前市面上同类的四轮小车平台如Autolabor等。
 <div align=center><img width="800" height="300" src="https://github.com/golaced/OLDX-FC_QUADRUPED_QUADROTOR/blob/rmd/support_file/img_file1/r1.jpg"/></div>
____如果您觉得该项目对您有帮助，也为了更好的项目推进和软硬件更新，如果愿意请通过微信捐赠该项目！
<div align=center><img width="440" height="300" src="https://github.com/golaced/OLDX_DRONE_SIM/blob/master/support_file/img_file/pay.png"/></div>



