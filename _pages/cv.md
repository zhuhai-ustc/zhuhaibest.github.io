---
layout: default
title: "完整简历"
permalink: /cv/
---

<div class="home-container">

  <h1 style="font-size: 2.5em; margin-bottom: 40px; color: var(--primary-color);">完整简历</h1>

  <!-- 个人总结 -->
  <div class="content-section">
    <h2>个人总结</h2>
    <p>拥有2年阿里国际搜推算法经验，专注于推荐精排模型优化和生成式推荐。独立一作发表过AAAI、COLING等顶级会议论文，引用量90。对大模型/生成式推荐前沿技术保持热情。</p>
  </div>

  <!-- 工作经历 -->
  <div class="content-section">
    <h2>工作经历</h2>

    <h3>阿里国际 AliExpress - 推荐算法工程师</h3>
    <p><strong>2024.07 - 至今</strong></p>
    <ul>
      <li>专注推荐精排模型商品建模方向，主导物流偏好建模，深度参与量价模型等工作，覆盖多个核心业务场景，服务亿级用户</li>
      <li>主导语义ID在排序模型中的探索与落地，设计并实现GateSID优化方案，提升新物品冷启动效率</li>
      <li>参与生成式排序Transformer模型（SORT）的设计与落地，实现订单 <span class="highlight">+6.35%</span>、GMV <span class="highlight">+5.47%</span> 的全场景业务提升</li>
    </ul>

    <h3>阿里国际 Lazada - 搜索算法工程师（实习）</h3>
    <p><strong>2023.07 - 2024.07</strong></p>
    <ul>
      <li>针对传统搜索相关性计算仅基于文本信息的局限，负责利用多模态大模型提升搜索相关性，提出Query-LIFE方法</li>
      <li>实现基于查询感知的图文模态融合，有效结合图像和标题信息，增强商品表示准确性</li>
      <li>线上取得订单UV提升 <span class="highlight">3.06%</span>，GMV提升 <span class="highlight">3.19%</span>，成果发表于 <a href="https://aclanthology.org/2025.coling-industry.2.pdf" target="_blank">COLING 2025</a></li>
    </ul>
  </div>

  <!-- 项目经历 -->
  <div class="content-section">
    <h2>项目经历</h2>

    <h3>语义ID精排建模（GateSID）</h3>
    <p><strong>2025.07 - 2026.01</strong></p>

    <p><strong>情境</strong>：推荐冷启动场景中，排序模型面临协同信号与语义信号权衡难题，新物品因缺乏协同信息难以获得足够曝光</p>

    <p><strong>任务</strong>：设计能够根据物品成熟度动态平衡语义信息与协同信号的推荐框架，提升冷启动效率</p>

    <p><strong>行动</strong>：</p>
    <ul>
      <li>提出GateSID框架，利用RQ-VAE将多模态特征离散化为分层语义ID，并构造用户语义ID行为序列</li>
      <li>设计门控融合共享注意力机制，对冷启动物品依赖语义信号，对热门物品保留协同信号</li>
    </ul>

    <p><strong>结果</strong>：</p>
    <ul>
      <li>GateSID在所有指标上均优于SOTA基线（COINS、SaviorRec）</li>
      <li>CTCVR AUC <span class="highlight">+0.4%</span>、GMV <span class="highlight">+2.6%</span>、订单量 <span class="highlight">+1.6%</span></li>
      <li>成果投稿于 SIGIR 2026</li>
    </ul>

    <hr>

    <h3>工业级推荐系统排序Transformer模型（SORT）</h3>
    <p><strong>2025.07 - 至今</strong></p>

    <p><strong>情境</strong>：单场域数据独立训练导致用户全域意图建模缺失，传统排序模型scaling up收益递减</p>

    <p><strong>任务</strong>：设计并落地基于生成式架构的transformer排序大模型，突破传统模型瓶颈</p>

    <p><strong>行动</strong>：</p>
    <ul>
      <li>实现请求级样本组织、局部注意力</li>
      <li>改进Transformer架构，引入特殊token、QKNorm、Attention Gate和Sparse MoE模块</li>
      <li>优化训练/推理系统，联动工程团队开发稀疏注意力算子、算子融合，MFU从13%提升至22%</li>
    </ul>

    <p><strong>结果</strong>：</p>
    <ul>
      <li>线上A/B测试订单 <span class="highlight">+6.35%</span>、GMV <span class="highlight">+5.47%</span></li>
      <li>服务效率提升：延迟降低 <span class="highlight">44.67%</span>，吞吐量 <span class="highlight">+121.33%</span></li>
      <li>模型性能：CTR-AUC提升 <span class="highlight">2.1pt</span>，在数据/模型/序列长度维度均展现优秀扩展性</li>
      <li>成果投稿 KDD 2026，详见 <a href="https://arxiv.org/pdf/2603.03988" target="_blank">arXiv论文</a></li>
    </ul>

    <hr>

    <h3>量价模型优化</h3>
    <p><strong>2024.07 - 2025.03</strong></p>

    <p><strong>情境</strong>：原有排序模型对价格变动商品响应滞后，无法实时捕捉量价关系变化，影响流量分配效率</p>

    <p><strong>任务</strong>：设计量价感知排序模型，实现对价格变化的快速响应，优化流量生态</p>

    <p><strong>行动</strong>：</p>
    <ul>
      <li>深入研究量价关系，提出基于量价排序模型</li>
      <li>增强价格信息表示，引入价格单调网络，优化CTR/CVR对价格变化的实时调整能力</li>
    </ul>

    <p><strong>结果</strong>：</p>
    <ul>
      <li>降价商品流量 <span class="highlight">+41%</span>，涨价商品流量 <span class="highlight">-18%</span>，总订单 <span class="highlight">+1.9%</span></li>
      <li>有效提升大盘效率，优化流量生态</li>
    </ul>

    <hr>

    <h3>物流偏好建模</h3>
    <p><strong>2025.03 - 2025.09</strong></p>

    <p><strong>情境</strong>：传统策略信号调整物流偏好方式僵硬且效率有损，无法精准识别优质物流服务</p>

    <p><strong>任务</strong>：将物流履约信号融合进排序模型，实现自动化的物流质量识别与流量分配</p>

    <p><strong>行动</strong>：</p>
    <ul>
      <li>构造用户/商品/交叉三侧物流信号</li>
      <li>构建物流偏好建模模块，让模型自动识别并偏好优质物流服务</li>
    </ul>

    <p><strong>结果</strong>：</p>
    <ul>
      <li>在GMV <span class="highlight">+0.5% 至 +1.1%</span> 前提下，物流优品订单 <span class="highlight">+1.0% 至 +1.9%</span></li>
      <li>物流差品订单 <span class="highlight">-1.5% 至 -1.9%</span>，签收时长降低 <span class="highlight">0.2 至 0.35天</span></li>
    </ul>

    <hr>

    <h3>搜索相关性多模态（Query-LIFE）</h3>
    <p><strong>2023.07 - 2024.07</strong></p>

    <p><strong>情境</strong>：传统相关性计算方法仅基于产品标题和查询建模，无法充分利用图像信息，影响搜索准确性</p>

    <p><strong>任务</strong>：设计多模态相关性计算方法，提升搜索结果的准确性和用户体验</p>

    <p><strong>行动</strong>：</p>
    <ul>
      <li>提出Query-LIFE方法，采用基于查询的图文模态融合</li>
      <li>有效结合图像和标题信息，利用查询感知的模态对齐增强商品表示准确性</li>
    </ul>

    <p><strong>结果</strong>：</p>
    <ul>
      <li>线上A/B测试订单UV提升 <span class="highlight">3.06%</span>，GMV提升 <span class="highlight">3.19%</span></li>
      <li>成果发表于 <a href="https://aclanthology.org/2025.coling-industry.2.pdf" target="_blank">COLING 2025</a></li>
    </ul>
  </div>

  <!-- 技术影响 -->
  <div class="content-section">
    <h2>技术影响</h2>
    <ul>
      <li>在NLP/多模态/搜推方向均有相关经验，发表 <span class="highlight">AAAI、COLING</span> 等多篇会议论文，引用量 <span class="highlight">90</span>，详见 <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=fKOITdsAAAAJ" target="_blank">Google Scholar</a></li>
      <li>对前沿技术保持好奇和关注，业余时间搭建AI论文阅读助手，包含前后端、数据库、大模型Agent等多种技术，提升算法同学阅读论文效率。累计收录 <span class="highlight">36w+</span> 论文，触达 <span class="highlight">400+</span> 用户，累计访问 <span class="highlight">3w+</span>，工作日DAU <span class="highlight">30-40</span></li>
    </ul>
  </div>

  <!-- 教育背景 -->
  <div class="content-section">
    <h2>教育背景</h2>

    <h3>中国科学技术大学 - 计算机技术（硕士）</h3>
    <p><strong>2021.09 - 2024.06</strong></p>

    <h3>杭州电子科技大学 - 信息安全（学士）</h3>
    <p><strong>2017.09 - 2021.06</strong></p>
  </div>

  <!-- 返回首页 -->
  <div class="content-section" style="text-align: center;">
    <a href="{{ '/' | relative_url }}" style="font-size: 1.1em; font-weight: 500;">← 返回首页</a>
  </div>

</div>