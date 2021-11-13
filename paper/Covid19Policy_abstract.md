---
output:
  bookdown::pdf_document2:
    keep_tex: true
    fig_caption: true
    latex_engine: xelatex
    number_sections: true
  bookdown::word_document2:
    reference_docx: "template_CHN.docx"
    keep_md: true
    number_sections: FALSE
knit: (function(inputFile, encoding) {rmarkdown::render(inputFile, encoding = encoding, output_format = c("bookdown::word_document2", "bookdown::pdf_document2")) })
documentclass: ctexart

fontsize: 12pt
geometry: margin=1in
bibliography: Covid19Policy.bib
csl: "china-national-standard-gb-t-7714-2015-author-date.csl"
link-citations: true
colorlinks: true
toc: false
indent: true
always_allow_html: true

editor_options: 
  markdown: 
    wrap: sentence

title: '能力不够压力来凑：治理能力与压力型体制'
subtitle: "——基于2021年春节期间地方疫情防控政策的实证研究"

author:
- 孙宇飞^[清华大学政治学系博士生，联系电话：18638750921，邮箱：sunyf20@mails.tsinghua.edu.cn]
- 杨雪冬^[清华大学社科学院政治学系教授，博士生导师]

abstract: |
  “压力型体制”作为对中国地方治理实践的理论描绘，得到了国内外学者的广泛关注和讨论。十八大以来，党和政府推动的一系列政治体制改革，深刻得改变了“压力型体制”的运行环境，“压力型体制”在保持生动的描述力和较强的解释力的同时，遇到“减压阀失灵”等理论困境和解释力不足等问题。本研究在梳理已有理论的基础上，结合地方治理能力和数字政府建设等视角，以2021年春节期间疫情防控政策在中国293个地级市的差异化制定为案例，通过自然语言处理和回归分析等方法对“压力型体制”进行了理论检验与修正。
  笔者发现，和原有“压力型体制”的理论一致，上级、同级政府和民众的压力对地方政府的政策加码程度均有显著影响。在检验经典理论的基础上，笔者着重识别和检验了地方政府治理能力的影响。笔者发现，**地方政府的治理能力对“压力型体制”的运行有着明显的“减压阀”效应**，这一减压阀的存在使得地方政府在多方的压力下还能保留一定的自主性空间。地方政府的治理能力强弱决定着地方自主性空间的大小，治理能力越强的地方政府的行政自主性就越大，从而能够较为灵活的处理多方压力和政策加码。具体来说，在控制其他变量的前提下，地方政府的数字治理能力和卫生能力对地方政府疫情防控政策加码程度有着显著的负向影响。在此基础上，笔者提出了提出压力型体制运行过程中地方政府**“能力空间”**的概念，从而实现了对“压力型体制”的理论检验与修正。
  
  **关键词**：压力型体制；层层加码；数字治理能力；能力空间。

---