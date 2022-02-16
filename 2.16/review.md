# Cell types of origin of the cell-free transcriptome

## 1

* Cell-free RNA from liquid biopsies can be analyzed to determine disease tissue of origin.
  来自液体活检的无细胞RNA可以被分析来==确定疾病组织的起源==。
* We extend this concept to identify cell types of origin using the Tabula Sapiens transcriptomic cell atlas as well as individual tissue transcriptomic cell atlases in combination with the Human Protein Atlas RNA consensus dataset.
  我们将这一概念扩展到使用==<u>Tabula Sapiens</u>转录细胞图谱==和==单个组织转录细胞图谱==，并结合人类蛋白质图谱RNA共识数据集来识别起源的细胞类型。

![image-20220216022237347](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfquyesiwj20lk0aqgn3.jpg)

> Tabula Sapiens is a benchmark, first-draft human cell atlas of nearly 500,000 cells from 24 organs of 15 normal human subjects.
> Tabula Sapiens是一份基准的初稿人体细胞图谱，包含来自15名正常人24个器官的近50万个细胞。
> This work is the product of the Tabula Sapiens Consortium.
> 这项工作是Tabula Sapiens联盟的产品。
> Special thanks to the Chan Zuckerberg Initiative for funding this project and to the CZI Science Technology team for creating cellxgene, the tool that makes the visualization of this research possible.
> 特别感谢陈·扎克伯格倡议为该项目提供资金，并感谢CZI科学技术团队创造了cellxgene，这一工具使这项研究成为可能。

* We define cell type signature scores, which allow the inference of cell types that contribute to cell-free RNA for a variety of diseases.
  我们定义了==细胞类型签名分数==，它允许推断==对各种疾病的无细胞RNA有贡献的细胞类型==。

## 2

* Cell-free RNA (cfRNA) represents a mixture of transcripts reflecting the health status of multiple tissues1 , thereby affording broad clinical utility.
  无细胞RNA(CfRNA)是反映==多种组织健康状况的多种转录本的混合物==，因此具有广泛的临床应用价值。
* However, several aspects about the physiologic origins of cfRNA, including the contributing cell types of origin, remain unknown, and current assays focus on tissue-level contributions at best1,3,4,5–7 .
  然而，关于cfRNA的生理起源的几个方面，包括==起源的贡献细胞类型==，仍然是==未知==的，目前的分析主要集中在==组织水平==的贡献上，最好的是1，3，4，5-7。

### fig.1a

![image-20220213141228081](https://tva1.sinaimg.cn/large/008i3skNly1gzbuu7nlv8j316a0hkn10.jpg)

> a, Integration of tissue of origin and single-cell transcriptomics to identify cell types of origin in cfRNA.
> A，整合起源组织和单细胞转录组学，以==确定cfRNA中起源的细胞类型==。

* We first characterized the landscape of cell-type-specific signal from healthy donor plasma using published exome-enriched cell-free transcriptome data 6 (Fig. 1a).
  我们首先利用已发表的富含外显子组的无细胞转录组数据6(图1A)描述了来自健康供体血浆的细胞类型特异性信号的图景。
  After removing low-quality samples (Extended Data Fig. 1 and Methods), we intersected the set of genes detected in healthy individuals (n = 75) with a database of cell-type-specific markers defined in context of the whole body9 .
  去除低质量样本(扩展数据图1和方法)后，我们将==在健康个体(n=75)中检测到的一组基因与在整个身体环境中定义的细胞类型特异性标记数据库9交叉==。

### exfig.1

![image-20220216010234725](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfqv2h6dcj20u00w8gpe.jpg)

> Extended Data Fig. 1 | Cell-free RNa Sample Quality Control.
> 扩展数据图1：无细胞RNA样品质量控制。
> Quality control metrics (3′ bias fraction, ribosomal fraction, and DNA contamination) were determined for each cfRNA sample downloaded from a given SRA accession number.
> 为从给定SRA登录号下载的每个cfRNA样本确定质量控制指标(==3‘偏倚分数、核糖体分数和DNA污染==)。
> Samples with outlier values are highlighted in red and were not considered in subsequent analyses (see Methods section ‘Sample quality filtering’).
> 带离群值的样本以红色突出显示，在后续分析中不考虑(参见方法部分“样本质量过滤”)。
> (a) Ibarra et al (n = 285) (b) Toden et al (n = 339) (c) Chalasani et al (n = 500).
> (A)Ibarra等人(n=285)(B)Toden等人(n=339)(C)Chalasani等人(n=500)。
> Box plot: horizonal line, median; lower hinge, 25 th percentile; upper hinge, 75 th percentile; whiskers span the 1.5 interquartile range; points outside the whiskers indicate outliers.
> 方框图：水平线，中位数；下铰链，第25百分位数；上铰链，第75百分位数；胡须跨越1.5个四分位数范围；胡须外的点表示异常值。
> Each point corresponds to a downloaded cfRNA sample from the corresponding SRA accession number.
> 每个点对应于从相应的SRA登录号下载的cfRNA样本。

* Marker genes for blood, brain, and liver cell types were readily detected, as previously observed at tissue level1,3,4,6,7 , as well as the kidney, gastrointestinal tract, and pancreas (Fig. 1b).
  血液、脑和肝细胞类型的标记基因很容易被检测到，正如之前在组织水平1、3、4、6、7以及肾脏、胃肠道和胰腺观察到的那样(图1B)。

### fig.1b

![image-20220213141934957](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq07wunlj20x60l6q5h.jpg)

> b, Cell-type-specific markers defined in context of the human body identified in plasma cfRNA.
> B，在血浆cfRNA中确定的==人体环境中定义的细胞类型特异性标记物==。
> Error bars denote the s.d. of number of cell-type-specific markers (n = 75 patients); the measure of center is the mean.
> 误差条表示细胞类型特异性标记物数量(n=75名患者)的标准差；中心的测量为平均值。
> CPM-TMM counts for a given gene across technical replicates were averaged before intersection.
> 在交集前，对特定基因跨技术重复的CPM-TMM计数进行平均。

* We then sought to deconvolve the fractions of cell-type-specific RNA using support vector regression, a deconvolution method previously applied to decompose bulk tissue transcriptomes into fractional cell type contributions10,11 .
  然后，我们试图使用==支持向量回归==来==去卷积特定细胞类型RNA==的部分，这是一种以前应用于将大量组织转录本分解为部分细胞类型贡献的去卷积方法10，11。
* To reduce multicollinearity, transcriptionally similar cell types were grouped (Extended Data Fig. 2).
  为了减少多重共线性，转录上相似的细胞类型被分组(扩展数据图2)。

### exfig.2

![image-20220216005248897](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq06thsgj20u00x80wt.jpg)

> Extended Data Fig. 2 | hierarchical clustering on non-immune Tabula Sapiens organ compartments.
> 扩展数据图2：非免疫性Tabula Sapiens器官隔室的层次聚类。
> Dashed line indicates the height at which tree was cut.
> ==虚线表示砍树的高度==。
> Dendrograms correspond with the cell type annotations belonging to (a) the epithelial compartment, (b) the endothelial compartment (c) the stromal compartment.
> 树状图与属于(A)上皮室、(B)内皮室(C)间质室的细胞类型注释相对应。



* We observed that the basis matrix defined by this gene set appropriately described cell types as most similar to others from the same organ compartment and corresponded to the highest off-diagonal similarity (Fig. 1c).
  我们观察到，由该基因集定义的基本矩阵恰当地描述了==细胞类型与来自同一器官隔室的其他细胞类型==最相似，并对应于最高的非对角相似性(图1C)。

### fig.1c

![image-20220216005541233](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq050qcgj20wm0padkq.jpg)

> c, Cluster heat map of Spearman correlations of the cell type basis matrix column space derived from Tabula Sapiens.
> 从Tabula Sapiens导出的单元类型基矩阵列空间的Spearman关联的群集热图。
> Color bar denotes correlation value.
> 颜色条表示相关值。

* We also confirmed that the basis matrix accurately deconvolved cell-type-specific RNA fractional contributions from several bulk tissue samples 13 (Extended Data Fig. 3 and Supplementary Information).
  我们还证实，基础矩阵准确地==去卷积==了来自几个==批量组织样本==13的==特定细胞类型的RNA分数贡献==(扩展数据图3和补充信息)。

### exfig.3

![image-20220216010747840](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq03kspqj21ew0u041n.jpg)

> Extended Data Fig. 3 | Tabula Sapiens basis matrix performance on <u>GTEx</u> bulk RNA samples using <u>nu-SVR</u>.
> 扩展数据图3：使用nu-SVR的Tabula Sapiens基矩阵在GTEx批量RNA样本上的性能。
>
> > GTEx:
> > The GTEx (Genotype-Tissue Expression) Project identified genetic variants that influence how genes are turned on and off in human tissues and organs.
> > GTEx(基因类型-组织表达)项目确定了影响基因在人体组织和器官中的开启和关闭方式的遗传变异。
> > Genetic variants that influence how genes behave are called expression quantitative trait loci (eQTLs).
> > 影响基因行为的遗传变异被称为表达数量性状位点(EQTL)。
> >
> > nu-SVR:
> > Based on support vector machines method, Nu Support Vector Regression (NuSVR) is an algorithm to solve the regression problems.
> > 基于支持向量机方法的神经网络支持向量机(NuSVR)是解决回归问题的一种算法。
> > The NuSVR algorithm applies nu parameter by replacing the the epsilon parameter of SVR method.
> > NuSVR算法通过替换SVR方法的epsilon参数来应用nu参数。
>
> GTEx tissue samples possessing cell types wholly present and absent from the basis matrix column space were selected.
> 选择具有完全存在和不存在于基本矩阵列空间中的细胞类型的GTEx组织样本。
> For box plots: horizonal line, median; lower hinge, 25 th percentile; upper hinge, 75 th percentile; whiskers, 1.5 interquartile range; points outside the whiskers indicate outliers.
> 对于盒子图：水平线，中位数；下铰链，第25百分位数；上铰链，第75百分位数；胡须，1.5个四分位数范围；胡须以外的点表示异常值。
> There are 30 bulk RNA seq samples for a given tissue except for the Bladder (n = 21), Kidney – Medulla (n = 4), and Whole Blood (n = 19).
> 除膀胱(n=21)、肾脏-髓质(n=4)和全血(n=19)外，其他组织均有30个RNA序列样本。
> (a) Root mean square error between predicted expression and measured expression in a given GTEx tissue.
> (A)==给定GTEx组织中预测表达和测量表达之间的均方根误差==。
> Units are zero-mean unit variance scaled CPM counts.
> 单位是零均值单位方差比例的CPM计数。
> Tissues present in TSP have reduced RMSE compared to those that are absent (Kidney – Medulla and Brain).
> ==TSP中存在的组织与不存在的组织==(肾脏、延髓和大脑)相比，RMSE降低。
> Tissues with high cellular heterogeneity (for example Lung, Bladder, Small Intestine, Kidney) exhibit reduced deconvolution performance compared to less heterogeneous tissues (for example Whole Blood, Spleen, Liver).
> ==细胞异质性高的组织==(如肺、膀胱、小肠、肾脏)与==异质性较低的组织==(如全血、脾、肝)相比，去卷积性能降低。
> (b) Pearson correlation between predicted expression and measured expression in a given GTEx tissue.
> (B)给定GTEx组织中预测表达和测量表达之间的皮尔逊相关性。

* We used this matrix to deconvolve the cell types of origin in the plasma cell-free transcriptome (Fig. 1d and Extended Data Figs. 4 and 5).
  我们用这个矩阵去卷积了==浆细胞==无转录组中起源的细胞类型(图1D和扩展数据图4和5)。

![image-20220216013536850](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq02d7m8j21bp0u079q.jpg)

> d, Mean fractional contributions of cell-type-specific RNA in the plasma cell-free transcriptome (n = 18 patients).
> D，==血浆==无细胞转录组(n=18)中==细胞类型特异性RNA==的平均贡献率。

* Altogether, the observation of contributions from many non-hematopoietic cell types underscores the ability to simultaneously non-invasively resolve contributions to cfRNA from disparate cell types across the body.
  总之，对许多==非造血细胞类型==的贡献的观察强调了同时非侵入性地解决==全身不同细胞类型对cfRNA的贡献==的能力。

* Some cell types likely present in the plasma cell-free transcriptome were missing in this decomposition because the source tissues were not represented in TSP.
  一些可能存在于浆细胞无转录组中的细胞类型在这种分解中==缺失==，因为==源组织在TSP中不存在==。

* To identify cell type contributions possibly absent from this analysis, we intersected the genes measured in cfRNA missing from the basis matrix with tissue-specific genes from the Human Protein Atlas (HPA) RNA consensus dataset15 .
  为了确定这项分析中可能缺少的细胞类型贡献，我们将==基础矩阵中缺失==的cfRNA中测量的基因与==人类蛋白图谱(HPA)RNA共识数据集==15中的==组织特异性基因交叉==。

* This identified both the brain and the testis as tissues whose cell types were not found during systems-level deconvolution and additional genes specific to the blood, skeletal muscle and lymphoid tissues that were not used by the basis matrix (Fig. 1e and Methods).
  这确定了大脑和睾丸都是在系统级去卷积过程中==没有发现细胞类型的组织==，以及基础矩阵没有使用的==血液、骨骼肌和淋巴组织的额外基因==(图1E和方法)。

### fig.1e

![image-20220216015052696](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfq00ry0jj213g0u00uw.jpg)

> e, Top tissues in cfRNA not captured by basis matrix (the set difference of all genes detected in a given cfRNA sample and the row space of the basis matrix intersection with HPA tissue-specific genes).
> E，未被基础矩阵捕获的cfRNA中的top组织(在给定的cfRNA样本中检测到的==所有基因的集合==差值以及与HPA组织特异性基因相交的碱基矩阵的行空间)。
> Error bars denote the s.d of number of HPA tissue-specific genes with NX counts >10 and cell-free CPM expression ≥ 1 (n = 18 patients); the measure of center is the mean.
> 误差条表示Nx计数>10的HPA组织特异性基因数和无细胞cpm表达≥-1(n=18例)的标准差，中心为平均值。

* As an example of how to analyze cell type contributions from tissues that were not present in TSP, we used an independent brain single-cell atlas along with HPA to define cell type gene profiles and examined their expression in cfRNA (Fig. 2a and Extended Data Figs. 6 and 7).
  作为如何分析==TSP中不存在的组织==的细胞类型贡献的一个例子，我们使用独立的==大脑单细胞图谱以及HPA==来定义==细胞类型基因图谱==，并检查它们在cfRNA中的表达(图2A和扩展数据图6和7)。
* There was a strong signature score from excitatory neurons and a reduced signature score from inhibitory neurons.
  ==兴奋性神经元==的签名分数较高，而==抑制性神经元==的签名分数较低。
  We observed strong signals from astrocytes, oligodendrocytes and oligodendrocyte precursor cells.
  我们观察到来自==星形胶质细胞、少突胶质细胞和少突胶质前体细胞的强烈信号==。

### fig.2a

![image-20220216022431964](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzzgwp5j20pq0neq3w.jpg)

> a, Neuronal and glial cell type signature scores in healthy cfRNA plasma (n = 18) on a logarithmic scale.
> 健康cfRNA血浆(n=18)在对数尺度上的==神经元和胶质细胞==类型特征记分。
>
> Ast, astrocyte; Ex, excitatory neuron; In, inhibitory neuron; Oli, oligodendrocyte; Opc, oligodendrocyte precursor cell.
> AST，星形胶质细胞；Ex，兴奋性神经元；IN，抑制性神经元；OLI，少突胶质细胞；OPC，少突胶质前体细胞。

### exfig.6

![image-20220216023205325](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzy62kgj20u00vs78w.jpg)

> Extended Data Fig. 6 | establishing gene profile cell type specificity in context of the whole body using single cell and bulk RNa-seq data.
> 扩展数据图6：使用==单细胞和批量RNA-SEQ数据==在==全身范围内==建立==基因图谱细胞类型特异性==。
> (a) Cell type signature scoring procedure; please see the ‘Signature Scoring’ in the Methods for the full derivation procedure of a given cell type gene profile.
> (A)细胞类型签名评分程序；有关给定细胞类型基因图谱的完整推导程序，请==参阅方法中的“签名评分”==。
> (b) Single cell heatmaps for gene cell type profiles within the corresponding tissue cell atlas, demonstrating that a cell type specific profile is unique to a given cell type across those within a given tissue.
> (B)相应组织细胞图谱内的基因细胞类型图谱的单细胞热图，表明细胞类型特定图谱在给定组织内的给定细胞类型中是独一无二的。
> Columns denote marker genes for a given cell type; rows indicate individual cells.
> ==列表示给定细胞类型的标记基因==；==行表示单个细胞==。
> The color bar scale corresponds to log-transformed counts-per-ten thousand.
> 颜色条标度对应于经对数变换的每万个计数。
> (c) Gini coefficient density plot for genes in cell type profiles derived from brain and liver single cell atlases using HPA NX counts.
> (C)用HPA NX计数绘制脑和肝单细胞图谱中细胞类型基因的基尼系数密度图。
> The area under the curve for a given cell type sums to one.
> 给定单元格类型的曲线下面积之和为1。
> (d) Log fold change in bulk RNA-seq data of a given cell type profile, demonstrating that the predominant expression of the cell type signature in its native tissue is highest relative to other non-native tissues.
> (D)给定细胞类型图谱的大宗RNA-seq数据的对数折叠变化，表明==该细胞类型特征在其固有组织中的优势表达高于其他非固有组织==。
> Values are the log-fold change of the signature score of a given cell type profile in the native tissue (indicated by the y-axis) to the mean expression in the remaining non-native tissues.
> 这些值是自然组织(由y轴表示)中给定细胞类型简档的签名分数到其余非自然组织中的平均表达的对数倍变化。
> Box plot: horizontal line, median; lower hinge, 25th percentile; upper hinge, 75th percentile; whiskers span the 1.5 interquartile range; points outside the whiskers indicate outliers (n = 2462 GTEx brain samples for box plot on left; n = 226 GTEx liver samples, right).
> 盒子图：水平线，中位数；下铰链，第25百分位数；上铰链，第75百分位数；胡须跨越1.5个四分位数范围；胡须外面的点表示异常值(n=2462 GTEx大脑样本，左侧为盒子图；n=226 GTEx肝脏样本，右侧)。

### exfig.7

![image-20220216024935363](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzw9lgtj20u00yhdjm.jpg)

> Extended Data Fig. 7 | Distribution of Gini coefficient and Tau for all genes denoted by HPA as specific to the brain, liver, placenta, and kidney.
> 扩展数据图7：HPA表示的大脑、肝脏、胎盘和肾脏特有的所有基因的基尼系数和Tau的分布。

* Similarly, we used published cell atlases for the placenta19,20 , kidney 21 and liver 22 to define cell-type-specific gene profiles (Extended Data Figs. 6 and 8) for signature scoring.
  类似地，我们使用已发表的胎盘19、20、肾脏21和肝脏22的细胞图谱来定义==特定细胞类型的基因图谱==(扩展数据图6和8)，用于签名评分。
  These observations augment the resolution of previously observed tissue-specific genes reported to date in cfRNA 1–7 and formed a baseline from which to measure aberrations in disease.
  这些观察结果增强了之前在cfRNA1-7中观察到的组织特异性基因的分辨率，并形成了测量==疾病中畸变==的基线。

### exfig.8

![image-20220216112725121](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzu9hbej20u00xen2i.jpg)

> Extended Data Fig. 8 | Comprehensive placental and renal cell type gene profile specificity at single cell and whole body resolution.
> 扩展数据图8：全面的胎盘和肾细胞类型基因图谱在单细胞和全身分辨率上的特异性。
> For box plots in f, g: horizontal line, median; lower hinge, 25th percentile; upper hinge, 75th percentile; whiskers span the 1.5 interquartile range; points outside whiskers indicate outliers.
> 对于f中的框图，g：水平线，中位数；下铰链，25%；上铰链，75%；胡须跨越1.5个四分位数范围；胡须外部的点表示异常值。
> (a) Violin plot of derived syncytiotrophoblast and extravillous trophoblast gene profiles from Vento-Tormo et al.
> (A)来自Vento-Tormo等人的合体滋养细胞和绒毛外滋养细胞基因图谱的小提琴曲线图。
> (b) Violin plot of derived syncytiotrophoblast and extravillous trophoblast gene profiles from Suryawanshi et al.
> (B)来自Suryawshi等人的合体滋养细胞和绒毛外滋养细胞基因图谱的小提琴曲线图。
> (c) Violin plot of derived proximal tubule gene profile (d) Gini coefficient distribution for placental trophoblast cell types in (a) and (b) (e) Gini coefficient distribution for renal cell type in (c) (f) Distribution of placental trophoblast signature scores across all GTEx tissues.
> (C)近端小管基因图谱的小提琴曲线图(D)胎盘滋养层细胞类型的基尼系数分布(A)和(B)(E)肾细胞类型的基尼系数分布(C)(F)胎盘滋养层细胞签名分数在所有GTEx组织中的分布。
> Note: given that the placenta is not in GTEx, the box plots correspond to the distribution of signature scores across non-placental tissues (sum of log-transformed counts-per-ten thousand) (n = 17382 non-placenta GTEx samples) (g) Log-fold change of renal cell type signature score in GTEx Kidney Cortex/Medulla samples relative to the mean non-kidney signature score, demonstrating that the predominant expression of the cell type signature in its native tissue is highest relative to other non-native tissues.
> 注：鉴于胎盘不在GTEx中，盒子图对应于签名分数在非胎盘组织中的分布(对数变换计数之和-每万个)(n=17382个非胎盘GTEx样本)(G)GTEx肾皮质/髓质样本中肾细胞类型签名分数相对于平均非肾脏签名分数的对数倍变化，表明细胞类型签名在其固有组织中的优势表达高于其他非天然组织。
> Values are the log ratio of the signature score in the kidney to the mean signature score in the remaining non-kidney GTEx tissue samples (n = 89 GTEx renal cortex or medulla samples).
> 这些值是肾脏中的签名分数与其余非肾脏GTEx组织样本(n=89 GTEx肾皮质或髓质样本)中的平均签名分数的对数比率。

* Cell-type-specific changes drive disease etiology8 , and we asked whether cfRNA reflected cellular pathophysiology.
  ==细胞类型特异性变化驱动疾病==病因，我们询问cfRNA是否反映了细胞病理生理学。

* The proximal tubule is a highly metabolic, predominant kidney cell type and is a major source for injury and disease progression in CKD25,26 .
  ==近端小管==是一种高度代谢的、占主导地位的==肾细胞类型==，是CKD25、26中损伤和疾病进展的主要来源。
  Using data from Ibarra et al., we discovered a striking decrease in the proximal tubule cell signature score of patients with CKD (ages 67–91 years, CKD stage 3–5 or peritoneal dialysis) compared to healthy controls (Fig. 2b and Extended Data Fig. 10a,b).
  使用Ibarra等人的数据，我们发现==CKD(慢性肾病)==患者(年龄67-91岁，CKD分期3-5或腹膜透析)的==近端小管细胞签名评分与健康对照组相比显著降低==(图2B和扩展数据图10A，b)。

### fig.2b

![image-20220216114118339](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzrzkocj20xs0u0ack.jpg)

> b, Comparison of the proximal tubule signature score in CKD stages 3+ (n = 51 samples; nine patients) and healthy controls (n = 9 samples; three patients) (P = 9.66 × 10 −3 , U = 116, one sided).
> B、==CKD3+期==(n=5 1例，9例)与==健康对照组==(n=9例，3例)==近端小管信号积分比较==(P=9.6 6×10−3，U=116，单侧)。
> Dot color denotes each patient.
> 圆点颜色表示每个病人。

### exfig.10ab

<img src="https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzq77knj20j21eqwkk.jpg" alt="image-20220216114500462" style="zoom:25%;" />

> Extended Data Fig. 10 | assessment of cell type gene profile discriminatory power during signature scoring.
> 扩展数据图10：签名评分过程中细胞类型基因图谱==区分力==的评估。
> (a) Density of p-values over 10,000 trial permutation test to assess p-value calibration for a given signature score.
> (A)超过10,000个p值的密度试验排列测试，以评估给定签名分数的p值校准。
> In all cases, the distribution is uniform, as expected under the null.
> 在所有情况下，分布都是均匀的，正如在空值下预期的那样。
> (b) Density of U values over 10,000 trial permutation test; red line indicates the U value corresponding to the experimental comparison reported in Fig. 2.
> (B)U值超过10,000次试验排列试验的密度；红线表示与图2中报告的实验比较相对应的U值。

* These results demonstrate non-invasive resolution of proximal tubule deterioration observed in CKD histology 31 and are consistent with findings from invasive biopsy.
  这些结果证实了CKD组织学31中观察到的==近端小管恶化的非侵入性消退==，并与==侵袭性活检的结果一致==。

* Hepatocyte steatosis is a histologic hallmark of NASH and NAFLD phenotypes, whereby the accumulation of cellular stressors results in hepatocyte death27 .
  ==肝细胞脂肪变性==是<u>NASH</u>和<u>NAFLD</u>表型的组织学标志，由此==细胞应激源的积累==导致肝细胞死亡27。

  > 非酒精性脂肪性肝炎(NASH)/非酒精性脂肪性肝病(NAFLD)

  Notable hepatocyte-specific differentially expressed genes (DEGs) include genes encoding cytochrome P450 enzymes (including CYP1A2, CYP2E1 and CYP3A4), lipid secretion (MTTP) and hepatokines (AHSG and LECT2)32 .
  值得注意的肝细胞特异性差异表达基因(DEG)包括编码细胞色素P450酶(包括CYP1A2、CYP2E1和CYP3A4)、脂质分泌(MTTP)和肝素(AHSG和LECT2)32的基因。
  We further observed striking differences in the hepatocyte signature score between healthy and both NAFLD and NASH cohorts and no difference between the NASH and NAFLD cohorts (Fig. 2c and Extended Data Fig. 10).
  我们进一步观察到，健康人群、NAFLD和NASH人群之间的==肝细胞签名评分有显著差异==，==NASH人群和NAFLD人群之间没有差异==(图2C和扩展数据图10)。

### fig.2c

![image-20220216115316341](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzncm4rj20xu0u0diq.jpg)

> c, Hepatocyte signature score between healthy (n = 16) and both NAFLD (n = 46) (P = 3.15 × 10 −4 , U = 155, one sided) and NASH (n = 163) (P = 4.68 × 10 −6 , U = 427, one sided); NASH versus NAFLD (P = 0.464, U = 3483, two sided).
> C：肝细胞签名分数，正常组16例，NAFLD组46例(P=3.15×10−4，U=155，单侧)与NASH组163例(P=4.68×10−6，U=427，单侧)，NASH组与NAFLD组(P=0.464，U=3483，双侧)。
> Color reflects sample collection center.
> 颜色反映==样本采集中心==。

* AD pathogenesis results in neuronal death and synaptic loss29 .
  AD发病导致==神经元死亡和突触丢失==29。
  We used brain single-cell data 28 to define brain cell type gene profiles in both the AD and the normal brain.
  我们使用==大脑单细胞数据==28来定义阿尔茨海默病和正常大脑中的脑细胞类型基因图谱。

* We then inferred neuronal death in plasma cfRNA between AD and healthy non-cognitive controls (NCIs) and also observed differences in oligodendrocyte, oligodendrocyte progenitor and astrocyte signature scores (Fig. 2d and Extended Data Fig. 10).
  然后，我们推断了==AD和健康非认知对照组==(NCIS)血浆cfRNA中的神经元死亡，还观察到了少突胶质细胞、少突胶质细胞前体细胞和星形胶质细胞签名评分的差异(图2D和扩展数据图10)。

### fig.2d

![image-20220216120402454](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfpzi6z8aj20xj0u0dhr.jpg)

> d, Neuronal and glial signature scores in AD (n = 40) and NCI (n = 18) cohorts.
> AD组(n=40)和NCI组(n=18)的D、神经元和胶质细胞签名评分。
> Excitatory neuron (P = 4.94 × 10 −3 , U = 206, one sided), oligodendrocyte (P = 2.28 × 10 −3 , U = 178, two sided), oligodendrocyte progenitor (P = 2.27 × 10 −2 , U = 224, two sided) and astrocyte (P = 6.11 × 10 −5 , U = 121, two sided).
> 兴奋性神经元(P=4.94×10−3，U=2 0 6，单侧)、少突胶质细胞(P=2.2 8×10−3，U=178，双侧)、少突胶质前体细胞(P=2.2 7×10−2，U=2 2 4，双侧)和星形胶质细胞(P=6.11×10−5，U=12 1，双侧)。
> Ast, astrocyte; Ex, excitatory neuron; In, inhibitory neuron; Oli, oligodendrocyte; Opc, oligodendrocyte precursor cell.
> AST，星形胶质细胞；Ex，兴奋性神经元；IN，抑制性神经元；OLI，少突胶质细胞；OPC，少突胶质前体细胞。

* Taken together, this work demonstrates consistent non-invasive detection of cell-type-specific changes in human health and disease using cfRNA.
  综上所述，这项工作展示了使用cfRNA对==人类健康和疾病中特定细胞类型的变化==进行==一致的非侵入性检测==。
  Our findings uphold and further augment the scope of previous work identifying immune cell types and hematopoietic tissues as primary contributors to the cell-free transcriptome cell type landscape.
  我们的发现支持并进一步扩大了先前工作的范围，==确定免疫细胞类型==和==造血组织==是无细胞转录组细胞类型图景的主要贡献者。

* Consistent detection of cell types responsible for drug metabolism (for example, liver and renal cell types) as well as cell types that are drug targets, such as neurons or oligodendrocytes for Alzheimer’s-protective drugs, could provide strong clinical trial endpoint data when evaluating drug toxicity and efficacy.
  对==负责药物新陈代谢的细胞类型==(例如，肝和肾细胞类型)以及作为==药物靶点的细胞类型==(如阿尔茨海默氏症保护性药物的神经元或少突胶质细胞)的==持续检测==，可以在==评估药物毒性和疗效==时提供强有力的临床试验终点数据。
  We anticipate that the ability to non-invasively resolve cell type signatures in plasma cfRNA will both enhance existing clinical knowledge and enable increased resolution in monitoring disease progression and drug response.
  我们预计，==非侵入性地解析血浆cfRNA中的细胞类型特征==的能力既能==增强现有的临床知识==，又能==提高监测疾病进展和药物反应的分辨率==。

## Online content

* Any methods, additional references, Nature Research reporting summaries, source data, extended data, supplementary information, acknowledgements, peer review information; details of author contributions and competing interests; and statements of data and code availability are available at https://doi.org/10.1038/ s41587-021-01188-9.
  任何方法、其他参考文献、自然研究报告摘要、源数据、扩展数据、补充信息、确认、同行评审信息；作者贡献和竞争兴趣的详细信息；以及数据和代码可用性的声明，请访问https://doi.org/10.1038/s41587-021-01188-9。

## Methods

### Data processing

#### data acquisition——数据获取

#### Bioinformatic processing

* Python+R+Trimomatic(修剪reads)+STAR(映射)+GATK中的MarkDuplates(删除重复reads)+Snakemake+MultiQC(工具性能统计数据)

#### Sample quality filtering

* RNA degradation, ribosomal read fraction and DNA contamination

#### Data normalization

* All gene counts were adjusted to counts per million (CPM) reads and per milliliter of plasma used.
  所有的基因计数都调整为==每百万读数(CPM)==和==每毫升血浆使用的计数==。
  For a given sample, i denotes gene index, and j denotes sample index:
  对于给定的样本，i表示基因索引，j表示样本索引：

### Cell type marker identification using <u>PanglaoDB</u>

> PanglaoDB:
>
> PanglaoDB is a database for the scientific community interested in exploration of single cell RNA sequencing experiments from mouse and human.
> PanglaoDB是一个面向科学界的数据库，该数据库对探索小鼠和人类的单细胞RNA测序实验感兴趣。
> We collect and integrate data from multiple studies and present them through a unified framework.
> 我们收集和整合来自多项研究的数据，并通过一个统一的框架提供这些数据。

* Markers were filtered for human (‘Hs’) only and for PanglaoDB’s defined specificity (how often marker was not expressed in a given cell type) and sensitivity (how frequently marker is expressed in cells of this type).
  仅针对==人类==(‘HS’)和PanglaoDB定义的==特异性==(标记==在给定细胞类型中不表达的频率==)和==敏感性==(标记在==该类型的细胞中表达的频率==)筛选标记。
  Gene synonyms from Panglao were determined using MyGene version 3.1.0 to ensure full gene space.
  利用MyGene版本3.1.0确定了庞老的基因同义词，确保了完整的==基因空间==。
  A given cell type marker was counted in a given healthy cfRNA sample if its gene expression was greater than zero in log +1 transformed CPM-TMM gene count space.
  在一个给定的健康cfRNA样本中，如果其基因在log+1转化的cpm-TMM基因计数空间中的==表达大于零==，则该给定的细胞类型标记被计数。
* We then intersected this gene space with a cohort of healthy cfRNA samples (n = 75, NCI individuals from Toden et al.).
  然后，我们将这个基因空间与一组健康的cfRNA样本(n=75，来自Toden等人的NCI个体)相交。
* Cell types with markers filtered by sensitivity = 0.9 and specificity = 0.2 and samples with >5 cell type markers on average are shown in Fig. 1b.
  ==图1B==显示了标记按==灵敏度=0.9和特异度=0.2==过滤的细胞类型和平均>5个细胞类型标记的样本。

### Basis matrix formation

* Given the non-specificity of the following annotations (for example, other cell type annotations at finer resolution existed), cells with these annotations were excluded from subsequent analysis:
  鉴于以下批注的==非特异性==(例如，存在分辨率更高的其他单元格类型批注)，具有这些批注的单元格将从后续分析中==排除==：
* The resulting cell type space still possessed several transcriptionally similar cell types (for example, various intestinal enterocytes, T cells or dendritic cells), which, left unaddressed, would reduce the linear independence of the basis matrix column space and, hence, would affect nu-SVR deconvolution.
  得到的细胞类型空间仍然具有几种==转录上相似的细胞类型==(例如，各种肠道肠道细胞、T细胞或树突状细胞)，如果不加以处理，将==降低==基本基质列空间的==线性独立性==，因此将==影响nu-SVR的去卷积==。
* Hierarchical clustering with complete linkage (sc.tl.dendrogram) was performed per compartment on the feature space comprising the first 50 principal components (sc.pp.pca).
  在包括==前50个主成分==(sc.pp.pca)的特征空间上对每个隔室执行具有完全链接的==分层聚类==(sc.tl.endrogram)。
  Epithelial and stromal compartment dendrograms were then cut (scipy.cluster.hierarchy.cut_tree) at 20% and 10% of the height of the highest node, respectively, such that cell types with high transcriptional similarity were grouped together, but overall granularity of the cell type labels was preserved.
  然后，分别在==最高节点高度的20%和10%处切割上皮和间质隔室树状图==(scipy.cluster.Hierarchy.Cut_tree)，使得具有==高转录相似性==的细胞类型被==分组在一起==，但细胞类型标记的总体粒度被保留。

### Nu-SVR deconvolution

* We formulated the cell-free transcriptome as a linear summation of the cell types from which it originates1,48 .
  我们将无细胞转录组表示为==其起源的细胞类型的线性总和==1，48。

* In contrast to the other methods, nu-SVR cell type contributions were the most consistent with the cell type markers detected using PanglaoDB and was, hence, chosen as the deconvolution model for this work.
  与其他方法相比，==nu-SVR细胞类型贡献与庞老DB检测到的细胞类型标记最一致==，因此被选为本工作的去卷积模型。

### Evaluating basis matrix on GTEx samples

### Identifying tissue-specific genes in cfRNA absent from basis matrix

* To identify cell-type-specific genes in cfRNA that were distinct to a given tissue, we considered the set difference of the non-zero genes measured in a given cfRNA sample with the row space of the basis matrix and intersected this with HPA tissue-specific genes:
  为了识别==cfRNA==中与==给定组织不同的细胞类型特异性基因==，我们考虑了在给定cfRNA样本中测量的非零基因与基本矩阵的行空间的集合差异，并将其与==HPA组织特异性基因==相交：

* The HPA tissue-specific gene set (HPA) comprised genes across all tissues with Tissue Specificity assignments ‘Group Enriched’, ‘Tissue Enhanced’, ‘Tissue Enriched’ and NX expression ≥10. This approach yielded tissues with several distinct genes present in cfRNA, which could then be subsequently interrogated using single-cell data.
  ==HPA组织特异性基因集(HPA)包括所有组织中的基因==，组织特异性指定为“组丰富”、“组织增强”、“组织丰富”和Nx表达≥10。这种方法产生的组织具有几个在==cfRNA中存在的不同基因==，随后可以使用==单细胞数据进行查询==。

### Derivation of cell-type-specific gene profiles in context of the whole body using single-cell data

**使用单细胞数据在全身范围内推导特定细胞类型的基因图谱**

* For this analysis, only cell types unique to a given tissue (that is, hepatocytes unique to the liver or excitatory neurons unique to the brain) were considered so that bulk transcriptomic data could be used to ensure specificity in context of the whole body.
  在这项分析中，只考虑了==特定组织特有的细胞类型==(即肝脏特有的肝细胞或大脑特有的兴奋性神经元)，以便可以使用大量转录数据来确保整个身体的特异性。
  A gene was asserted to be cell type specific if it was (1) differentially expressed within a given single-cell tissue atlas, (2) possessed a Gini coefficient ≥0.6 and was listed as specific to the native tissue for the cell type of interest, indicating comprehensive tissue specificity in context of the whole body (Extended Data Figs. 6 and 8).
  如果一个基因是(1)在给定的==单细胞组织图谱中差异表达==，(2)具有基尼系数≥0.6，并且被列为==感兴趣细胞类型的天然组织特有的==，则断言该基因是细胞类型特异性的，表明在整个身体的上下文中具有全面的组织特异性(扩展数据图6和8)。

#### Single-cell differential expression

#### Quantifying comprehensive whole-body tissue specificity using the Gini coefficient

**用基尼系数量化全身综合组织特异性**

* The distribution of all the Gini coefficiets and Tau values across all genes belonging to cell type gene profiles for cell types native to a given tissue were compared using the HPA gene expression Tissue Specificity and Tissue Distribution assignments 15 (Extended Data Fig. 7).
  使用HPA基因表达、组织特异性和组织分布指配15(扩展数据图7)比较了属于==特定组织固有细胞类型==的==细胞类型基因谱的所有基因==的所有基尼系数和Tau值的分布。
  The Gini coefficient better reflected the underlying distribution of gene expression tissue specificity than Tau (Extended Data Fig. 7) and, hence, were used for subsequent analysis.
  基尼系数比Tau(扩展数据图7)更好地反映了==基因表达组织特异性==的潜在分布，因此被用于后续分析。
  As the Gini coefficient approaches unity, this indicates extreme gene expression inequality or equivalently high specificity.
  当==基尼系数接近1==时，这表明==基因表达的极端不平等或相当高的特异性==。
* A single threshold (Gini coefficient ≥ 0.6) was applied across all atlases to facilitate a generalizable framework from which to define tissue-specific cell type gene profiles in context of the whole body in a principled fashion for signature scoring in cfRNA.
  将单一阈值(基尼系数cfRNA ≥ 0.6)应用于所有图谱，以便于以原则性方式以签名计分的方式在全身范围内定义组织特异性细胞类型基因图谱的可概括性框架。

### Gene expression in GTEx

* We confirmed ==the specificity of== ==a given gene profile to its corresponding cell type== by comparing the aggregate expression of a given cell type signature in its native tissue compared to that of the average across remaining GTEx tissues (Extended Data Figs. 6d and 8f,g).
  我们通过比较==给定细胞类型签名==在其==固有组织中的聚集表达==与==其它GTEx组织中的平均表达==来确认==给定基因图谱对其相应细胞类型==的==特异性==(扩展数据图6d和8f，g)。
  We uniformly observed a median fold change greater than 1 in the signature score of a cell type gene profile in its native tissue relative to the mean expression in other tissues, confirming high specificity.
  我们一致地观察到，相对于其他组织的平均表达，细胞类型基因图谱在其==自身组织==中的签名分数的中位数倍数变化大于1，证实了高特异性。

### Cell type specificity of DEGs in AD and NAFLD cfRNA

* After observing a significant intersection between the DEGs in AD 6 or NAFLD 7 in cfRNA with corresponding cell-type-specific genes (Extended Data Fig. 10c,e), we then assessed the cell type specificity of DEGs using a permutation test.
  在观察到cfRNA中AD6或NAFLD7中的DEG与相应的细胞类型特异基因(扩展数据图10C，e)之间的显著交集后，我们然后使用==置换测试==评估了DEG的细胞类型特异性。
  To assess whether DEGs that intersected with a cell type gene profile were more specific to a given cell type than DEGs that were generally tissue specific, we performed a permutation test.
  为了评估与==细胞类型==基因图谱相交的DEG是否比通常具有==组织==特异性的DEG对给定的细胞类型更具特异性，我们进行了一项排列测试。
  Specifically, we compared the Gini coefficient for genes in these two groups, computed using the mean expression of a given gene across brain cell types from healthy brain 28 or liver 22 single-cell data.
  具体地说，我们比较了这两组基因的基尼系数，使用健康大脑28或肝脏22单细胞数据中给定基因在不同脑细胞类型中的平均表达来计算。

### exfig.10c

![image-20220216223841501](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfqbtjabqj20p00jmmy0.jpg)

> (c) Donut plot reflecting the number of genes in the hepatocyte cell type gene profile that intersect with the reported NAFLD DEG in Chalasani et al.
> (C)Donut图，反映与Chalasani等人报道的NAFLD DEG相交的肝细胞类型基因谱中的基因数量

### exfig.10e

![image-20220216223859419](https://tva1.sinaimg.cn/large/e6c9d24ely1gzfqc4tadnj20ne0nu75v.jpg)

> (e) Donut plots reflecting the number of genes in brain cell type gene profiles that intersect with the reported AD DEG in Toden et al.
> (E)反映==脑细胞类型基因图谱==中与Toden等报道的AD DEG相交的基因数量的甜甜圈曲线图。

### Estimating signature scores for each cell type

### Assessing P value calibration for a given signature score
