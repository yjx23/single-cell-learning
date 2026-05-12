# single-cell-learning
My single-cell RNA-seq learning journey


# 单细胞测序数据分析学习笔记 🧬

> 从零开始完成 PBMC3k 单细胞转录组数据分析

## 📌 项目简介

本项目记录了我学习单细胞 RNA 测序（scRNA-seq）数据分析的完整过程。

**数据来源**: 10x Genomics PBMC3k 数据集（2700 个外周血单核细胞）

## 🎯 完成的分析内容

- ✅ 质量控制（QC）- 过滤低质量细胞
- ✅ 数据标准化与高变基因筛选
- ✅ PCA 降维与 UMAP 可视化
- ✅ 细胞聚类与标记基因鉴定
- ✅ 细胞类型注释（T细胞、B细胞、单核细胞等）
- ✅ 功能富集分析（GO/KEGG）

## 📊 分析结果展示

### UMAP 聚类图
![UMAP](outputs/figures/02_umap_clusters.svg)

### 细胞类型注释
![Annotated UMAP](outputs/figures/04_umap_annotated.svg)

### 标记基因热图
![Heatmap](outputs/figures/03_marker_heatmap.svg)

## 📁 代码结构

| 脚本 | 功能 |
|:---|:---|
| `01_qc_analysis.R` | 数据加载 + 质量控制 |
| `02_normalization_pca_clustering.R` | 标准化 + PCA + 聚类 + UMAP |
| `03_markers_annotation.R` | 标记基因鉴定 + 细胞注释 |
| `04_functional_enrichment.R` | GO/KEGG 功能富集分析 |

## 🚀 运行说明

1. 安装 R 和 RStudio
2. 安装所需包：`Seurat`, `SeuratData`, `clusterProfiler`, `org.Hs.eg.db`
3. 运行 `code/` 目录下的脚本（按编号顺序）

## 📄 License

MIT