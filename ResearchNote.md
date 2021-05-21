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
# bibliography: /Users/sunyufei/Desktop/Zotero.bib
csl: "/Users/sunyufei/Documents/Yufei_Sun/THU/Education/Programming/R/Zotero/styles/american-political-science-association.csl"
link-citations: true
colorlinks: true
toc: false

editor_options: 
  markdown: 
    wrap: sentence

title: '能力不够压力来凑：数字治理能力下的压力型体制'
subtitle: "——基于Covid19期间的春节返乡政策的混合方法研究"

author:
- 孙宇飞^[清华大学政治学系博士生，联系电话：18638750921，邮箱：sunyf20@mails.tsinghua.edu.cn]
- 陈佳静^[美国威斯康辛大学麦迪逊分校博士生，联系电话：，邮箱：]
---



This is a notebook recording the decisions for the project in collaboration with PhD. student Jiajing Chen to study the Covid-19 mandatory policy during the Spring Festival of 2021 in prefecture-level cities in China.



# 文章分析逻辑

政策加码过程：中央 - 省 - 地级市 - 基层

政策加码主体：下一级政府

中央 - **省**：公开政策比较

省 - **地级市**-政策的层面：公开政策比较

省 - **地级市**-执行的层面：公开政策与政务留言板的数值差异比较


# 分析模型

政策加码量（地级市） ~ 地级市数字治理能力 + 上级政府压力 + 同级政府压力 + 民众压力 + 其他控制变量

- 分析单位：中国大中城市101（副省级和省会城市33 + 普通大中城市68）

- 变量测量
  - 因变量：政策加码量
    - 政策层面
      - 地级市政策 - 省级政策
      - 地级市政策
    - 执行层面
      - 政务留言板的相对数量
      - 政务留言板的相对情绪
  - 自变量
    - 核心自变量：地级市数字治理能力（2020数字政府发展指数报告）
    - 上级政府压力
      - 上级政府开会的次数
      - 政府工作报告中提及的关键词数量
      - 该省的确诊人数
    - 同级政府压力
      - 其他同级城市（省会和副省级城市/同省普通大中城市）的确诊数量
      - 其他同级城市（省会和副省级城市/同省普通大中城市）的政策严格程度
    - 民众压力
      - 政府留言板的数量/情绪？
    - 其他控制变量
      - 人口流动
      - 经济发展
      - 疫情变量

