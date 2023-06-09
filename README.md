# EZBOX
这是一个以HITBOX为参考进行优化的布局，比MIXBOX更适合键盘玩家进阶，适合连续玩游戏时长超过2小时的玩家；

![image](https://github.com/89g-dyy/EZBOX/blob/main/rev1/Screenshots/rev1.png)

控制板采用树莓派PICO，芯片为RP2040；
PCB的线路布局参考https://github.com/OpenStickCommunity/GP2040-CE，建议直接用该项目的固件；
PCB的TYPEC下需要飞两根导线到树莓派pico底部，D+ -> TP2,D- -> TP3；
PCB绘制软件为嘉立创easyEDA，嘉立创工程https://oshwhub.com/89_g/89gbox

制作方法：
1、按照rev?文件夹里的bom&tools备齐物料与工具
2、将rev?\dwg内的顶板与底板制作出来(面板对切割的精密度要求比较高，不建议制作)
3、将rev?\GerBer_XXX交给PCB生产厂商生产出来（推荐嘉立创），选择好自己喜欢的颜色，嘉立创生产可以选择指定位置客编，这样PCB更整洁
  或者也可以在https://lceda.cn/editor#id=f018a354f8e147a6b28c85ed92779d2d这个网址里直接下单
  步骤：
    1)找到：制造=>一键PCB/SMT下单
    2)继续下单后数据生成完毕点确定
    3)进入下单页面后登录，选择类型、
    4)材质选择FR-4;
      阻焊颜色选择白色;
      外观包装要求里的板上不加客编选择：指定位置加客编，选择不确定生产稿;
      SMT不需要；钢网不需要；
      发票建议电子个人发票；
      其他的默认即可；

4、按照RP2040文件夹里的readme刷好固件
5、制作过程中需要仔细阅读每一个文件夹下的readme.txt
