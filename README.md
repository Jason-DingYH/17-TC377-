# 17-SAK-TC377TP-
17届智能车四轮摄像头组英飞凌TC377硬件开源。
外设包括MT9V034,ICM20602,基于IR2104的双路BDC驱动，四运放低端电机电流检测,板载双18650插座并含有硬件电池保护电路。(PCB孔位适用于C车模)。
![Mark2正面](https://user-images.githubusercontent.com/78647422/184537604-23308db6-9239-42e7-a9b5-bf2c518040e7.jpg)
此开源项目中一共有三个版本的PCB，1.第一版使用3节18650供电采用上下插板结构(电源板在下方，未上传到项目中)，母线电压使用LM5116降至7.4V，由于带载能力较弱，后弃用(若需要使用母线降压方案，项目中上传了一个BUCK_DEMO板，已验证通过，带载能力10A以上，需要做好散热。输入12.6v输出7.4v时负载10A输出纹波为80mv，可根据个人设计经验修改以提高纹波表现)。2.第二版采用2节18650电池直接供电，摄像头稳压电路漏连，如上图使用了飞线。3.第三版与第二版无大的改动，修正了摄像头稳压电路，并且引出更多io用于连接副板满足UI界面的设计需求
