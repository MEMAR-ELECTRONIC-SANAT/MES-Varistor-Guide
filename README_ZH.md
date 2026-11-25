# 压敏电阻选型与应用指南

<p align="center">
  <img src="Images/GitHub-Assets/MES-Hero-Banner.svg" width="100%" alt="MEMAR ELECTRONIC SANAT — MES">
</p>

<p align="center">
  <strong>语言 / Language:</strong><br>
  <a href="README.md">🇮🇷 فارسی</a> |
  <a href="README_EN.md">🇬🇧 English</a> |
  <a href="README_ZH.md">🇨🇳 简体中文</a>
</p>

## 指南简介

**从数据手册参数到实际过电压保护设计**

本仓库介绍压敏电阻，重点是**金属氧化物压敏电阻（MOV）**的内部结构、工作原理，以及它在瞬态过电压保护电路中的应用。内容面向电子工程师、电路设计人员、学生及电子爱好者，帮助读者理解如何根据实际电路要求评估和选择压敏电阻。

<p align="center">
  <img src="Images/GitHub-Assets/MES-Section-Header.svg" width="90%" alt="压敏电阻指南内容">
</p>

## 指南内容

1. 什么是压敏电阻，以及它如何保护电路
2. MOV 的结构，以及氧化锌（ZnO）晶粒和晶界的物理机制
3. 电压–电流（V–I）特性曲线及工作区域
4. 重要的数据手册参数及其解读方法
5. 压敏电阻技术，以及 MOV、TVS 和 GDT 的比较
6. 典型应用与保护电路设计
7. 四项关键选型指标：最大连续工作电压、箝位电压、浪涌电流和能量承受能力
8. 市电应用中的实际选型示例
9. 常见直流电压及 380 V 三相系统的型号参考
10. 总结、术语表与安全注意事项

## 文档下载

- 📘 [下载波斯语版压敏电阻指南 — PDF，版本 1.4](./MES-Varistor-Guide-FA%20v1_4.pdf)
- 🖼️ [浏览教学图片与信息图](./Images/README.md)
- 🎨 [浏览 MES GitHub 品牌图形资源](./Images/GitHub-Assets/README.md)

> **文件状态：** 当前 main 分支中已提供波斯语 PDF。英文版 PDF 尚未存入此仓库，因此这里暂不提供英文 PDF 下载链接。

## 压敏电阻选型的四项关键参数

| 参数 | 含义与选型要点 |
|---|---|
| **MCOV — 最大连续工作电压** | 应高于电路可能出现的最高正常工作电压，并考虑电源公差及工作条件。 |
| **箝位电压（V₍C₎）** | 浪涌电流流过 MOV 时器件两端的残余电压。该电压必须低于被保护设备可承受的电压。 |
| **最大浪涌电流（Iₚₑₐₖ）** | 在相应测试波形下，器件的额定浪涌电流应高于安装位置可能承受的浪涌电流。 |
| **能量额定值（J）** | 应满足预期瞬态能量、脉冲波形及重复次数的要求。 |

此外，还应检查规定测试电流下的压敏电压（例如 V₁mA）、电容、圆片尺寸、环境温度、爬电距离与电气间隙，以及与保险丝或热脱扣装置的配合。

## 设计与安全注意事项

- 压敏电阻通常应**并联连接在被保护的输入端或负载两端**。
- 箝位电压并非与电流无关的固定值；它取决于浪涌电流和测试波形。
- 对于连接市电的设备，必须考虑 MOV 与保险丝或热脱扣装置之间的配合。MOV 在过应力后可能短路并产生过热。
- 选型时应查阅对应制造商、准确料号的最新数据手册。不同测试波形或测试条件下的参数不能直接比较。
- 对于雷击或高能量瞬态环境，可能需要采用 MOV、TVS 和 GDT 协调配合的多级保护方案。
- 本指南中的示例和推荐型号仅供学习参考，不能替代产品安全评估、适用标准检查及最终器件数据手册验证。

## 教学图片与示意图

当前仓库中的教学信息图为波斯语版本。请访问 [Images 文件夹说明](./Images/README.md)，查看图片预览并获取原始文件。

<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-00.jpg" width="30%" alt="压敏电阻简介"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-01.jpg" width="30%" alt="MOV 结构与工作原理"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-02.jpg" width="30%" alt="数据手册参数"></a>
</p>
<p align="center">
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-03.jpg" width="30%" alt="工作电压与箝位电压"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-04.jpg" width="30%" alt="浪涌电流与能量"></a>
  <a href="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg"><img src="Images/Varistor%20Protection_%20MES%20Persian%20Infographic-05.jpg" width="30%" alt="压敏电阻尺寸"></a>
</p>

<p align="center">
  <img src="Images/GitHub-Assets/MES-Divider.svg" width="100%" alt="MES 分隔图">
</p>

## 编制与发布

**معمار الکترونیک صنعت**  
**MEMAR ELECTRONIC SANAT (MES)**

*与您携手设计和制造可靠的电子电路*

- Telegram: [Memar Electronic](https://t.me/Memar_Electronic)
- Instagram: [Memar Electronic](https://www.instagram.com/Memar.Electronic)
- GitHub: [MEMAR-ELECTRONIC-SANAT](https://github.com/MEMAR-ELECTRONIC-SANAT)

<p align="center">
  <img src="Images/GitHub-Assets/MES_Animated_Logo_640x480.svg" width="120" alt="MES 动态标志">
</p>
