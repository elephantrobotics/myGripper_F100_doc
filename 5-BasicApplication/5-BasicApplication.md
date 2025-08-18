# 屏幕控制

myCobot Pro 力控夹爪带有屏幕显示功能，并且屏幕下带有按键方便对屏幕的操
控，通过对界面的选择，可以更加便捷的操控夹爪与了解夹爪信息。屏幕信息和
整体功能描述

|界面|功能|
|:--|:--|
|主界面|查看夹爪信息，如：位置（Position）<br>设置速度（Speed）<br>电流 （Current）<br>输入 IO（Input）<br>输出 IO（Output）|
|设置界面（Setting）|查看，设置夹爪数据|
|设置波特率界面（Modbus Config）|查看和更改设备波特率|
|IO 使能界面（IO Config）|查看和使能 IO，默认 IO 是使能状态|
|夹爪控制界面（Manual Config）|Open-控制夹爪张开<br>Close-控制夹爪闭合<br>Release-夹爪不使能（这时候夹爪就不会有扭力，可以自由摆动爪）<br>Hold - 夹爪使能（给夹爪使能，这时候夹爪存在扭力）|
|版本信息界面（Information）|Firmware - 夹爪版本号与夹爪ID<br>Servomotor - 舵机版本号与舵机ID|

**主界面**

进入夹爪主界面，我们可以看到屏幕上实时获取夹爪的一些信息，这能更方
便的知道夹爪的信息。主界面主要有以下信息 如图所示

<img src="../img/pm1.png" width="50%" >

主界面上实时显示夹爪角度，速度，电流，输入输出 IO 电平

**设置界面**

主界面下长按确认键 2s 即可进入主界面

<img src="../img/pm2.png" width="50%" >

设置界面，通过按键可以上下移动和选择

<img src="../img/pm3.png" width="50%" >

**波特率设置**

在设置界面点击 Modbus 进入 Modbud Config 界面点击 Baudrate 进入界面，选择你想设置的波特率点击确认，当波特率傍边的原点颜色改变证明设置成功

<img src="../img/pm4.png" width="50%" >

设置完后找到 Exit 点击即可退出当前界面

**IO 使能设置**

设置界面选择 I/O Ctrl，进入 I/O Config 界面，默认下 IO 是使能状态，如果不行，使用 IO 控制，可以选择 Disable 来关闭 IO 控制

<img src="../img/pm5.png" width="50%" >

**Manual 界面**

设置界面选择 Manual 进入 Manual Control 界面实现快速便捷的操控夹爪

<img src="../img/pm6.png" width="50%" >

选择 Quick Move 即可进入控制夹爪界面，如图 4.7，选择 Gripper Init 可进入
夹爪配置界面

<img src="../img/pm7.png" width="50%" >

Open-设置夹爪张开，Close-设置夹爪闭合，Pelease-设置夹爪不使能，Hold-设置夹爪使能，Exit-退出当前界面

<img src="../img/pm8.png" width="50%" >

选择 Auto Init 可设置夹爪零位

**Information 界面**

通过选择 Information 进入界面，我们可以看到 Firmware 和 Servomotor 两个选
项，前者是固件版本号，点击进去，可以查看当前固件主版本与次版本号。后者
是查看点击信息，点击进去可以看到 ID 与电机的主版本和次版本

<img src="../img/pm9.png" width="50%" >

点击 Firmware 查看固件版本与设备 ID 指令中的 ID

<img src="../img/pm10.png" width="50%" >

点击 Servomotor 查看电机版本与 ID，ID 无法修改

<img src="../img/pm11.png" width="50%" >

#### IO 控制

根据上述的引脚线序说明，找到 OUT1 OUT2 对应的线，输入 24V，当输入一高一低电平
时夹爪就会运动，相反给出一高一低电平时夹爪就会反向运动。屏幕主界面上可以观察到 IO 输入情况，当没有 IO 输入是 Input 就显现白色，当 IO 输入时就会显现黑点

<img src="../img/IO3.png" width="50%" >