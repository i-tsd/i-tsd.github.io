---
title: 整合有化学裂解功能的微流控液滴中的单细胞RT-PCR
tags: 学习
---

《定量分析化学》课程的论文是写一篇文章的综述。本人写了微流控液滴中的单细胞RT-PCR。内容如下所示。

![](/pic/singlecell-1.jpg)

<!--more-->

## 摘要

通过液滴微流控技术，可用单细胞逆转录聚合酶链式反应 (RT-PCR) 辅助细胞的鉴别与分离。然而现有操作流程需要多种微型设备，以分别供酶催化细胞裂解、PCR试剂添加等步骤使用，使该过程繁琐而易失败。本文将描述一种将以上各步骤整合于单一设备中的新方法。此法令分离所得的单个细胞受控暴露于一碱性缓冲液中，裂解细胞，并使能够抑制 RT-PCR 反应的因子失活。含有裂解产物的液滴随后可被RT-PCR缓冲液所中和。利用此化学裂解法，可以区分出不同细胞个体的基因表达，且所得数据的质量不亚于较复杂的两步方法。该系统接收细胞并产生适于进行扩增的液滴，使在单细胞液滴中进行的 RT-PCR 更加快捷可靠。

## 背景与简介

生物体系往往由大量不同表型的细胞组成，因此对样品总体的分析可能掩盖会一些重要细胞亚群的特性。传统的分析单个细胞的方法通常只适用于分析样品的一小部分。因此，为完全表征大量细胞，尤其是含量较低但重要性高的细胞，必须开发超高通量分析方法。

基于转录组测序技术 (RNA-seq) 的转录分析由于能在全基因组水平上表征RNA表达而十分重要。然而，对数百万个细胞进行单细胞转录组测序在经济上不可行。

许多情况下，单一转录标志物便足以确定具有研究价值的细胞(例如，寻找表达具有癌细胞特性或病毒特性的转录子的细胞)。利用原位杂交技术的成像技术可根据特定 mRNA 区分不同细胞，并兼容高通量，故十分有价值。然而这些方法对表达程度较低的基因不敏感；而且，由于核酸的不稳定性，对已被分类的细胞进行下游的测序也有困难。

在微流控技术辅助下，可在经逆转录聚合酶链式反应 (RT-PCR) 扩增后探测到单个细胞中的特定RNA序列。这为单细胞基因表达分析提供了替代路径，并满足高通量的要求。另外，微流控液滴可以顺次被分析、分类，从而提供一种基于核酸组成的、类似于流式细胞术的检测分析手段。由于核酸的生物学意义，基于核酸组成对细胞进行可靠分类意义重大。

由于细胞必须被裂解才能释放RNA，在微流控液滴中进行单细胞 RT-PCR 存在诸多困难。裂解使用的试剂和裂解产物可抑制 RT-PCR 反应，而由于细胞在液滴中占据的相对体积很大（即浓度高），这一效应在微流控液滴中尤为明显。现有策略利用酶降解裂解产物消除这种影响，而酶必须在 PCR 之前加热灭活。因此,细胞裂解和试剂添加都需要单独的微流控设备。裂解产生的液滴被收集、加热、转移的过程费时费力且容易出错。为解决以上问题，本文将描述一种将以上各功能整合于单一设备中的新方法。

## 工作原理与方法

### 微流控设备的制造

微流控设备利用多层软光刻技术制造。用于刻蚀不同高度通道的光罩使用 AutoCAD 绘制，并印刷在透明胶片上。第一层 (6.5μm) 由用于从装置中提取油的细通道组成；第二层 (35μm) 包含用于将细胞封装于液滴中(微囊化)的通道与协流通道。第三层 (80μm) 包含控制液滴流速的延迟线、RT-PCR液滴生成装置、融合器与盐水电极。主模是利用旋涂法在一个 3 英寸硅晶圆上制造的。掩膜对准和紫外照射在每次旋涂后进行。最终，晶圆在 PGMEA 中成型。PDMS 基底与固化剂以 10:1 混合，经真空脱气后倾倒在置于培养皿上的主模上。混合物在 65℃ 下固化 4 小时后被切割。凿出一直径 750 μm 的余隙孔与聚乙烯管连接，以将液体注入通道。

### 细胞与试剂

Jurkat 和 MCF7 细胞在 37℃、5% CO2 存在下于含有 5% 胎牛血清 (FBS) 与抗生素的 RPMI-1640 培养液中培养。收集 80-100 万个 Jurkat/MCF7 细胞，然后在含 2% FBS 的冷 PBS(PBS-F) 中洗涤。离心，分别于 100μL, 10μM 钙黄绿素紫与钙黄绿素红中重悬，再于冰上放置 30min。着色后，细胞于100μL PBS-F中重悬，然后于40μL Optiprep混合以调整密度。洗涤对移除细胞外 mRNA 是必要的。碱解缓冲液 (ALB) 含有 20 mM NaOH, 60% (v/v) PEG-200 和 2% (v/v)Triton X-100。PEG-200 的碱性减少了 NaOH 的用量，使 RT-PCR 缓冲液能有效中和ALB。液滴在一种含 2% (w/w) 008-FluoroSurfactant 的氟化油 (3M, HFE Novec 7500) 中形成。含有液滴的油在 RT-PCR 前被含5%  (w/w) 008-FluoroSurfactant的 FC-40 油交换。RT-PCR 混合物含有 1:1 的反应混合物与酶混合物、2.5% (v/v) 的 Tween 20 与 2.5% (v/v) 的 PEG 6000。RT-PCR 混合物中加入了对 CD45 蛋白特异的荧光标记的 TaqMan 探针。

### 设备与RT-PCR操作

计算机控制注射泵将液体注入设备。将油从装置中提取出来的器件连接有一处于吸取状态的注射泵。倒置显微镜用于监测液滴生成。当细胞裂解产物液滴与 RT-PCR 混合物液滴达到 1：1 结合时，向盐水电极加压，使液滴发生融合。液滴被收集入多个 PCR 管，油相与 5% (w/w) 表面活性剂油发生交换，然后进行 PCR 热循环。

### 荧光成像与分析

RT-PCR 后，液滴被置于载玻片上，以倒转落射荧光显微镜成像；曝光时间由软件控制。液滴参数和荧光信号由Fiji粒子分析流程确定。对所得的荧光信号进行分析并作图。

## 结果与讨论

液滴中细胞的等效浓度很大(含1个细胞的 100pL 液滴中的细胞浓度相当于 1000 万个细胞每毫升)，所以细胞裂解所释放的分子能有效抑制许多生化反应。通常策略是纯化感兴趣的分子 (如 DNA、RNA) 再分析。然而，由于液滴本身就是功能齐全的反应器，难以耐受如萃取柱、毛细管电泳和化学沉淀等纯化手段，故纯化它们较困难。

因此，通过用蛋白酶分解包含阻碍生化反应的各种酶的裂解产物后，才能操作 RT-PCR 。由于蛋白酶亦可分解 RT-PCR 所须的酶，故在加入 RT-PCR 试剂前必须加热使之失活。因此，操作需分两步：其一是细胞被封装、裂解，其二是裂解后的液滴在热致失活后与 RT-PCR 液滴融合。这一流程复杂且容易出错。若能在单一装置中完成这一系列步骤则能使过程快捷可靠。

本研究中，研究人员选用化学手段——碱裂解法使抑制蛋白失活。室温下碱裂解只需数秒即可完成。裂解完成后，液滴可以直接被 RT-PCR 缓冲液所中和。这使在无热控制的单一装置中完成全部流程成为可能，从而大大降低了复杂度。

如封面图所示，装置将活细胞注入碱性缓冲液中，形成液滴。液滴通过混合器 b，在通道 d 中停留 30 秒。此后，碱性裂解液在与PCR试剂反应的流程中被中和，得到可用于PCR扩增的液滴 (e,f) 。这一方法使通量由先前方法的 168 滴/秒提升到 411 滴/秒。同时，液滴体积的缩小减小了试剂用量：在 10% 细胞负载率下，分析 10 万细胞所需的PCR试剂体积由 660μL 降至 270μL 。同时，先前报道中准备 47078 个液滴用时 120 分钟，而本方法只需 19 分钟。

高 pH 除裂解细胞外也会水解 RNA，故需要将液滴紧密堆积、使之在通道中匀速运动，以控制碱裂解的时长。通过从乳剂中移除油可以实现紧密堆积。管道长度经设计，使裂解时长为适宜的 30 s。                               

通过这一流程，可以根据特定基因表达来鉴别细胞。为展示这一点，研究人员将一些 Jurkat 细胞用钙黄绿素红 (红色荧光) 染色，以分辨存在细胞的液滴。而 RT-PCR TaqMan 探针 (绿色荧光) 用于鉴别该细胞的一种特定转录物。用显微镜观察所得液滴。由于液滴的细胞负载率为5.8%，故只能观察到少数含有裂解产物的红色荧光液滴。荧光的强度取决于细胞内酯酶的活性（这种酯酶将染料转化为具有荧光活性的形态）。观察发现，绝大部分含有裂解产物的液滴也具有绿色荧光活性。由于 Jurkat 细胞表达 CD45，这一结果是预料之中的。然而许多显示绿色荧光的液滴并不显示红色荧光。这种现象在液滴中进行的单细胞 RT-PCR 中十分常见，推测是 mRNA 在细胞在封装进液滴前释放所致。为了解决这种“背景”信号所带来的问题，可用活细胞染料对细胞进行预染色，以在分析过程中排除假阳性结果。另外，也需要合理选取荧光强度的临界值，以明确区分阳性和阴性细胞。

![](/pic/singlecell-2.jpg)

为展示本流程利用特定基因表达鉴别不同细胞的能力，研究人员分析了一组同时含有 MCF7 与 Jurkat 的细胞。MCF7 与 Jurkat 分别用钙黄绿素红与钙黄绿素紫染色。Jurkat 细胞表达 CD45，而 MCF7 不表达。如图所示，在不同通道下观察，得到了不同颜色的荧光图像。将不同图像叠加，便得到 (d)。为确定这种图像与已知的基因表达规律是否一致，将液滴对不同颜色荧光的强度作图如 (e) 所示。72%具有红色荧光的液滴也具有绿色荧光活性；而 86% 具有紫罗兰荧光的液滴则显示 MCF7 阴性。共计有 6% 的 MCF7 细胞显示 CD45 阳性，推测是因为液滴与细胞外的 CD45 转录产物的共微囊化，或非专一性的扩增。这一结果更容易在相关的二维散点图 (g)~(h) 中得到说明。正如前文所展示的，通过将探测与液滴分类相结合，可以分离得到特定的一类细胞裂解产物，以供进一步分析。

## 工作意义与个人思考

流式细胞术是生物学中重要的技术，但目前其适用范围基本上仅限于利用特异性抗体探测蛋白质组学标记；而核酸所承载的信息是细胞中最重要的信息之一。液滴微流控技术将两者结合，使基于核酸成分区分细胞成为可能，无疑是一重大进步。而本文所述的装置不再使用与 RT-PCR 不兼容的蛋白酶而改用碱裂解法，从而省略了繁琐的加热失活等步骤，使这一流程更加快速可靠。

快速地利用 RT-PCR 对单个细胞进行分析的能力在生物学方面具有较高的应用前景，如鉴别组织或血液中的特定细胞类型，以实现对癌细胞中紊乱基因表达的解卷积。

原文指出，钙黄绿素荧光的强度与细胞中酶的活性有关；由此联想到，倘若所有液滴均经过一定、相同次 RT-PCR热循环，则 CD45 荧光的强度是否能够与基因表达的程度相联系？除“基因是否表达”外，“基因表达程度”也是反映细胞特性的一个指标。倘若能建立荧光强度与基因表达的程度之间的明确关系，则可区分基因表达程度不同的细胞，从而提供更多有价值的生物学信息。我查阅资料了解到，实时荧光定量PCR技术可以对对待测样品中的特定 DNA 序列进行定量分析。因而，对微流控液滴应当也能应用类似技术。

另外，我也注意到，基于单细胞 RT-PCR 鉴别细胞的方法仅适合单一转录标志物便足以确定研究对象细胞的场合，因而其应用范围必然受限。是否可以考虑通过某些方法，如加入多种荧光探针，以确定多种转录标志物？

此外，文中所提到的单细胞测序技术近期也有所进展。传统测序技术一次处理大量细胞，从而得到的变异水平只能是平均后水平。而单细胞测序可以揭示细胞的微妙变化乃至发现全新的细胞类型。近期，我校谢晓亮教授团队正运用高细胞单通量测序技术寻找新冠病毒中和抗体，使效率大幅度提升。倘若能实现高通量单细胞转录组测序，则能解决目前单细胞RT-PCR所不能解决的上述问题。

## 参考文献

[Kim, S. C.; Clark, I. C.; Shahi, P.; Abate, A. R., Single-Cell RT-PCR in Microfluidic Droplets with Integrated Chemical Lysis. *Anal Chem* **2018**, *90* (2), 1273-1279.](https://pubs.acs.org/doi/abs/10.1021/acs.analchem.7b04050)