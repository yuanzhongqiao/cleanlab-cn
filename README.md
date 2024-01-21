<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><p align="center" dir="auto">
  <a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source_transparent_optimized_size.png"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source_transparent_optimized_size.png" width="60%" height="60%" style="max-width: 100%;"></a>
</p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab通过自动检测 ML 数据集中的问题来</font><font style="vertical-align: inherit;">帮助您</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">清理</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据和</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标签。</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为了促进</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用混乱的真实数据进行机器学习</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，这个以数据为中心的 AI 包使用您</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现有的</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型来估计数据集问题，这些问题可以修复以训练</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更好的</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型。</font></font></p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"># cleanlab works with **any classifier**. Yup, you can use PyTorch/TensorFlow/OpenAI/XGBoost/etc.</span>
<span class="pl-s1">cl</span> <span class="pl-c1">=</span> <span class="pl-s1">cleanlab</span>.<span class="pl-s1">classification</span>.<span class="pl-v">CleanLearning</span>(<span class="pl-s1">sklearn</span>.<span class="pl-v">YourFavoriteClassifier</span>())

<span class="pl-c"># cleanlab finds data and label issues in **any dataset**... in ONE line of code!</span>
<span class="pl-s1">label_issues</span> <span class="pl-c1">=</span> <span class="pl-s1">cl</span>.<span class="pl-en">find_label_issues</span>(<span class="pl-s1">data</span>, <span class="pl-s1">labels</span>)

<span class="pl-c"># cleanlab trains a robust version of your model that works more reliably with noisy data.</span>
<span class="pl-s1">cl</span>.<span class="pl-en">fit</span>(<span class="pl-s1">data</span>, <span class="pl-s1">labels</span>)

<span class="pl-c"># cleanlab estimates the predictions you would have gotten if you had trained with *no* label issues.</span>
<span class="pl-s1">cl</span>.<span class="pl-en">predict</span>(<span class="pl-s1">test_data</span>)

<span class="pl-c"># A universal data-centric AI tool, cleanlab quantifies class-level issues and overall data quality, for any dataset.</span>
<span class="pl-s1">cleanlab</span>.<span class="pl-s1">dataset</span>.<span class="pl-en">health_summary</span>(<span class="pl-s1">labels</span>, <span class="pl-s1">confident_joint</span><span class="pl-c1">=</span><span class="pl-s1">cl</span>.<span class="pl-s1">confident_joint</span>)</pre><div class="zeroclipboard-container">
   
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开始使用：</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/image.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">教程</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://docs.cleanlab.ai/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://github.com/cleanlab/examples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://cleanlab.ai/blog/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">学习在 5 分钟内对您的数据运行 cleanlab：</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/image.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">图像</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/datalab/text.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文本</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/audio.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">音频</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">表格</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 cleanlab 自动：</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/datalab/datalab_quickstart.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检测数据问题（异常值、重复项、标签错误等）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练稳健模型</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/multiannotator.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">推断多注释器数据的共识 + 注释器质量</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://github.com/cleanlab/examples/blob/master/active_learning_multiannotator/active_learning.ipynb"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">建议下一步（重新）标记数据（主动学习）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
</ul>
<p dir="auto"><a href="https://pypi.org/pypi/cleanlab/" rel="nofollow"><img src="https://camo.githubusercontent.com/bc818bc3023beb4ecd3b1b19ff4e6a8e08030cc5c7552304337d45635b43beed/68747470733a2f2f696d672e736869656c64732e696f2f707970692f762f636c65616e6c61622e737667" alt="皮皮" data-canonical-src="https://img.shields.io/pypi/v/cleanlab.svg" style="max-width: 100%;"></a>
<a href="https://pypi.org/pypi/cleanlab/" rel="nofollow"><img src="https://camo.githubusercontent.com/615105962da1d51015c3fbc59f0d14900421ac7936a75407add4f8b7b75a156f/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f706c6174666f726d2d6e6f617263682d6c6967687467726579" alt="你" data-canonical-src="https://img.shields.io/badge/platform-noarch-lightgrey" style="max-width: 100%;"></a>
<a href="https://pypi.org/pypi/cleanlab/" rel="nofollow"><img src="https://camo.githubusercontent.com/48de47b6c2927699b6abb34bd11ffa11a74f11222c0ddd6f17b051d254b274ef/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f707974686f6e2d332e372532422d626c7565" alt="py_版本" data-canonical-src="https://img.shields.io/badge/python-3.7%2B-blue" style="max-width: 100%;"></a>
<a href="https://github.com/cleanlab/cleanlab/actions?query=workflow%3ACI"><img src="https://github.com/cleanlab/cleanlab/workflows/CI/badge.svg" alt="构建状态" style="max-width: 100%;"></a>
<a href="https://app.codecov.io/gh/cleanlab/cleanlab" rel="nofollow"><img src="https://camo.githubusercontent.com/ef06c266a713d27bea30c914333fcfb02b45bff00efd7cdbb7f85025d1d49482/68747470733a2f2f636f6465636f762e696f2f67682f636c65616e6c61622f636c65616e6c61622f6272616e63682f6d61737465722f67726170682f62616467652e737667" alt="覆盖范围" data-canonical-src="https://codecov.io/gh/cleanlab/cleanlab/branch/master/graph/badge.svg" style="max-width: 100%;"></a>
<a href="https://docs.cleanlab.ai/" rel="nofollow"><img src="https://camo.githubusercontent.com/01d0f74c4a166f5435d186aaf59d8efb9590ea65064ec2ce5662992c07fb2687/68747470733a2f2f696d672e736869656c64732e696f2f7374617469632f76313f6c6f676f3d676974687562267374796c653d666c617426636f6c6f723d70696e6b266c6162656c3d646f6373266d6573736167653d636c65616e6c6162" alt="文档" data-canonical-src="https://img.shields.io/static/v1?logo=github&amp;style=flat&amp;color=pink&amp;label=docs&amp;message=cleanlab" style="max-width: 100%;"></a>
<a href="https://cleanlab.ai/slack" rel="nofollow"><img src="https://camo.githubusercontent.com/c045cc1f174ace28cff33995150ee6eafb80706e3bdc6507c1b12580054bb7c1/68747470733a2f2f696d672e736869656c64732e696f2f7374617469632f76313f6c6f676f3d736c61636b267374796c653d666c617426636f6c6f723d7768697465266c6162656c3d736c61636b266d6573736167653d636f6d6d756e697479" alt="松弛社区" data-canonical-src="https://img.shields.io/static/v1?logo=slack&amp;style=flat&amp;color=white&amp;label=slack&amp;message=community" style="max-width: 100%;"></a>
<a href="https://twitter.com/CleanlabAI" rel="nofollow"><img src="https://camo.githubusercontent.com/31150b659e7a6d9a7ae9afbb1d1550021ac81f16b140e08ed4f530e54c239f54/68747470733a2f2f696d672e736869656c64732e696f2f747769747465722f666f6c6c6f772f436c65616e6c616241493f7374796c653d736f6369616c" alt="推特" data-canonical-src="https://img.shields.io/twitter/follow/CleanlabAI?style=social" style="max-width: 100%;"></a>
<a href="https://cleanlab.ai/studio/?utm_source=github&amp;utm_medium=readme&amp;utm_campaign=clostostudio" rel="nofollow"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/shields/cl-studio-shield.svg" alt="清洁实验室工作室" style="max-width: 100%;"></a></p>
<p align="center" dir="auto">
  <a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/datalab_issues.png"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/datalab_issues.png" width="74%" height="74%" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 通过以下代码    
</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自动检测</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
    到 Cat/Dog 数据集中各种问题的示例：</font></font></p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre>        <span class="pl-s1">lab</span> <span class="pl-c1">=</span> <span class="pl-s1">cleanlab</span>.<span class="pl-v">Datalab</span>(<span class="pl-s1">data</span><span class="pl-c1">=</span><span class="pl-s1">dataset</span>, <span class="pl-s1">label</span><span class="pl-c1">=</span><span class="pl-s">"column_name_for_labels"</span>)
        <span class="pl-c"># Fit any ML model, get its feature_embeddings &amp; pred_probs for your data</span>
        <span class="pl-s1">lab</span>.<span class="pl-en">find_issues</span>(<span class="pl-s1">features</span><span class="pl-c1">=</span><span class="pl-s1">feature_embeddings</span>, <span class="pl-s1">pred_probs</span><span class="pl-c1">=</span><span class="pl-s1">pred_probs</span>)
        <span class="pl-s1">lab</span>.<span class="pl-en">report</span>()</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="        lab = cleanlab.Datalab(data=dataset, label=&quot;column_name_for_labels&quot;)
        # Fit any ML model, get its feature_embeddings &amp; pred_probs for your data
        lab.find_issues(features=feature_embeddings, pred_probs=pred_probs)
        lab.report()" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-so-fresh-so-cleanlab" class="anchor" aria-hidden="true" tabindex="-1" href="#so-fresh-so-cleanlab"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如此新鲜，如此干净的实验室</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab通过</font><a href="https://jair.org/index.php/jair/article/view/12125" rel="nofollow"><font style="vertical-align: inherit;">本文</font></a><font style="vertical-align: inherit;">和</font><a href="https://l7.curtisnorthcutt.com/confident-learning" rel="nofollow"><font style="vertical-align: inherit;">博客</font></a><font style="vertical-align: inherit;">中发布的最先进的</font><em><font style="vertical-align: inherit;">置信学习</font></em><font style="vertical-align: inherit;">算法来</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">清理</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您的数据</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实验室</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><a href="https://labelerrors.com" rel="nofollow"><font style="vertical-align: inherit;">请访问labelerrors.com</font></a><font style="vertical-align: inherit;">查看使用 cleanlab 清理的一些数据集</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">这款以数据为中心的 AI 工具可帮助您查找数据和标签问题，以便您可以训练可靠的 ML 模型。</font></font><em><font style="vertical-align: inherit;"></font></em><font style="vertical-align: inherit;"></font><a href="https://jair.org/index.php/jair/article/view/12125" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://l7.curtisnorthcutt.com/confident-learning" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font><a href="https://labelerrors.com" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">清洁实验室是：</font></font></p>
<ol dir="auto">
<li><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有理论支持</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">——</font><font style="vertical-align: inherit;">即使模型不完美，也</font></font><a href="https://arxiv.org/abs/1911.00068" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">能保证精确的标签噪声估计。</font></font></a><font style="vertical-align: inherit;"></font></li>
<li><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快速</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">——代码是并行的和可扩展的。</font></font></li>
<li><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">易于使用</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">——一行代码即可找到错误标记的数据、错误的注释器、异常值或训练抗噪声模型。</font></font></li>
<li><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">通用</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">——适用于</font></font><strong><a href="https://labelerrors.com/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任何数据集</font></font></a></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（文本、图像、表格、音频……）+</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任何模型</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（PyTorch、OpenAI、XGBoost……）</font></font></li>
</ol>
<br>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/label-errors-examples.png"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/label-errors-examples.png" alt="" style="max-width: 100%;"></a></p>
<p align="center" dir="auto"><font style="vertical-align: inherit;"></font><a href="https://l7.curtisnorthcutt.com/label-errors" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 cleanlab发现并纠正</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
各种图像数据集中不正确的给定标签的示例</font><font style="vertical-align: inherit;">。
</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-run-cleanlab" class="anchor" aria-hidden="true" tabindex="-1" href="#run-cleanlab"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行cleanlab</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 支持 Linux、macOS 和 Windows，并在 Python 3.7+ 上运行。</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"></font><a href="https://docs.cleanlab.ai/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从这里</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开始吧</font><font style="vertical-align: inherit;">！</font><font style="vertical-align: inherit;">通过</font></font><code>pip</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或按照</font><a href="https://docs.cleanlab.ai/" rel="nofollow"><font style="vertical-align: inherit;">此处</font></a></font><code>conda</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所述进行安装</font><font style="vertical-align: inherit;">。</font></font><a href="https://docs.cleanlab.ai/" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从源代码安装前沿的开发人员应参考</font></font><a href="https://docs.cleanlab.ai/master/index.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此主分支文档</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如需帮助，请查看我们详细的</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/faq.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">常见问题解答</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://github.com/cleanlab/cleanlab/issues?q=is%3Aissue"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Github 问题</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或</font></font><a href="https://cleanlab.ai/slack" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Slack</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们欢迎任何问题！</font></font></li>
</ul>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实践以数据为中心的人工智能可以如下所示：</font></font></strong></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在原始数据集上训练初始 ML 模型。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">利用此模型来诊断数据问题（通过 cleanlab 方法）并改进数据集。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在改进的数据集上训练相同的模型。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">尝试各种建模技术以进一步提高性能。</font></font></li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大多数人从步骤 1 → 4 跳转，但是通过使用 cleanlab，您可以在不</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更改</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">建模代码的情况下获得巨大收益！</font><font style="vertical-align: inherit;">通过迭代步骤 2 → 4 不断提高性能（并尝试使用</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">清理后的</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据进行评估）。</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/dcai_flowchart.png"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/dcai_flowchart.png" alt="" style="max-width: 100%;"></a></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-use-cleanlab-with-any-model-for-most-ml-tasks" class="anchor" aria-hidden="true" tabindex="-1" href="#use-cleanlab-with-any-model-for-most-ml-tasks"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">将 cleanlab 与任何模型结合使用来完成大多数 ML 任务</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 的所有功能都适用于</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任何数据集</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">任何模型</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">是的，任何模型：PyTorch、Tensorflow、Keras、JAX、HuggingFace、OpenAI、XGBoost、scikit-learn 等。如果您使用 sklearn 兼容的分类器，所有 cleanlab 方法都可以开箱即用。</font></font></p>
<details><summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
也可以轻松使用您最喜欢的非 sklearn 兼容模型（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击了解更多</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）
</font></font></summary>
<br>
<p dir="auto">cleanlab can find label issues from any model's predicted class probabilities if you can produce them yourself.</p>
<p dir="auto">Some cleanlab functionality may require your model to be sklearn-compatible.
There's nothing you need to do if your model already has <code>.fit()</code>, <code>.predict()</code>, and <code>.predict_proba()</code> methods.
Otherwise, just wrap your custom model into a Python class that inherits the <code>sklearn.base.BaseEstimator</code>:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">sklearn</span>.<span class="pl-s1">base</span> <span class="pl-k">import</span> <span class="pl-v">BaseEstimator</span>
<span class="pl-k">class</span> <span class="pl-v">YourFavoriteModel</span>(<span class="pl-v">BaseEstimator</span>): <span class="pl-c"># Inherits sklearn base classifier</span>
    <span class="pl-k">def</span> <span class="pl-en">__init__</span>(<span class="pl-s1">self</span>, ):
        <span class="pl-k">pass</span>  <span class="pl-c"># ensure this re-initializes parameters for neural net models</span>
    <span class="pl-k">def</span> <span class="pl-en">fit</span>(<span class="pl-s1">self</span>, <span class="pl-v">X</span>, <span class="pl-s1">y</span>, <span class="pl-s1">sample_weight</span><span class="pl-c1">=</span><span class="pl-c1">None</span>):
        <span class="pl-k">pass</span>
    <span class="pl-k">def</span> <span class="pl-en">predict</span>(<span class="pl-s1">self</span>, <span class="pl-v">X</span>):
        <span class="pl-k">pass</span>
    <span class="pl-k">def</span> <span class="pl-en">predict_proba</span>(<span class="pl-s1">self</span>, <span class="pl-v">X</span>):
        <span class="pl-k">pass</span>
    <span class="pl-k">def</span> <span class="pl-en">score</span>(<span class="pl-s1">self</span>, <span class="pl-v">X</span>, <span class="pl-s1">y</span>, <span class="pl-s1">sample_weight</span><span class="pl-c1">=</span><span class="pl-c1">None</span>):
        <span class="pl-k">pass</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from sklearn.base import BaseEstimator
class YourFavoriteModel(BaseEstimator): # Inherits sklearn base classifier
    def __init__(self, ):
        pass  # ensure this re-initializes parameters for neural net models
    def fit(self, X, y, sample_weight=None):
        pass
    def predict(self, X):
        pass
    def predict_proba(self, X):
        pass
    def score(self, X, y, sample_weight=None):
        pass" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">This inheritance allows to apply a wide range of sklearn functionality like hyperparameter-optimization to your custom model.
Now you can use your model with every method in cleanlab. Here's one example:</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">cleanlab</span>.<span class="pl-s1">classification</span> <span class="pl-k">import</span> <span class="pl-v">CleanLearning</span>
<span class="pl-s1">cl</span> <span class="pl-c1">=</span> <span class="pl-v">CleanLearning</span>(<span class="pl-s1">clf</span><span class="pl-c1">=</span><span class="pl-v">YourFavoriteModel</span>())  <span class="pl-c"># has all the same methods of YourFavoriteModel</span>
<span class="pl-s1">cl</span>.<span class="pl-en">fit</span>(<span class="pl-s1">train_data</span>, <span class="pl-s1">train_labels_with_errors</span>)
<span class="pl-s1">cl</span>.<span class="pl-en">predict</span>(<span class="pl-s1">test_data</span>)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="from cleanlab.classification import CleanLearning
cl = CleanLearning(clf=YourFavoriteModel())  # has all the same methods of YourFavoriteModel
cl.fit(train_data, train_labels_with_errors)
cl.predict(test_data)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h4 tabindex="-1" dir="auto"><a id="user-content-want-to-see-a-working-example-heres-a-compliant-pytorch-mnist-cnn-class" class="anchor" aria-hidden="true" tabindex="-1" href="#want-to-see-a-working-example-heres-a-compliant-pytorch-mnist-cnn-class"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>Want to see a working example? <a href="https://github.com/cleanlab/cleanlab/blob/master/cleanlab/experimental/mnist_pytorch.py">Here’s a compliant PyTorch MNIST CNN class</a></h4>
<p dir="auto">More details are provided in documentation of <a href="https://docs.cleanlab.ai/stable/cleanlab/classification.html" rel="nofollow">cleanlab.classification.CleanLearning</a>.</p>
<p dir="auto">Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the <a href="https://skorch.readthedocs.io/" rel="nofollow">skorch</a> Python library which will wrap your PyTorch model into a sklearn-compatible model (<a href="https://docs.cleanlab.ai/stable/tutorials/image.html" rel="nofollow">example</a>). For TensorFlow/Keras, check out our <a href="https://docs.cleanlab.ai/stable/cleanlab/models/keras.html" rel="nofollow">Keras wrapper</a>. Many libraries also already offer a special scikit-learn API, for example: <a href="https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn" rel="nofollow">XGBoost</a> or <a href="https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html" rel="nofollow">LightGBM</a>.</p>
<br>
</details>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 在各种机器学习任务中都很有用。</font><font style="vertical-align: inherit;">这种以数据为中心的人工智能解决方案提供专用功能的具体任务包括：</font></font></p>
<ol dir="auto">
<li><a href="https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">二元和多类分类</font></font></a></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/multilabel_classification.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多标签分类</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（例如图像/文档标记）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/token_classification.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标记分类</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（例如文本中的实体识别）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/regression.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">回归</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（预测数据集中的数字列）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/segmentation.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">图像分割</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（带有每像素注释的图像）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/object_detection.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对象检测</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（带有边界框注释的图像）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/multiannotator.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用多个注释器标记的数据进行分类</font></font></a></li>
<li><a href="https://github.com/cleanlab/examples/blob/master/active_learning_multiannotator/active_learning.ipynb"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用多个注释器进行主动学习</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（建议标记或重新标记哪些数据以最大程度地改进模型）</font></font></li>
<li><a href="https://docs.cleanlab.ai/stable/tutorials/outliers.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">异常值检测</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（识别不符合分布的非典型数据）</font></font></li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于其他 ML 任务，如果应用得当，cleanlab 仍然可以帮助您改进数据集。</font></font><a href="https://github.com/cleanlab/examples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的示例笔记本</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中演示了许多实际应用</font><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-citation-and-related-publications" class="anchor" aria-hidden="true" tabindex="-1" href="#citation-and-related-publications"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引文及相关出版物</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 基于同行评审的研究。</font><font style="vertical-align: inherit;">如果您使用此软件包，请引用以下相关论文：</font></font></p>
<details><summary><a href="https://arxiv.org/abs/1911.00068" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自信学习（JAIR '21）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@article{northcutt2021confidentlearning,
    title={Confident Learning: Estimating Uncertainty in Dataset Labels},
    author={Curtis G. Northcutt and Lu Jiang and Isaac L. Chuang},
    journal={Journal of Artificial Intelligence Research (JAIR)},
    volume={70},
    pages={1373--1411},
    year={2021}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@article{northcutt2021confidentlearning,
    title={Confident Learning: Estimating Uncertainty in Dataset Labels},
    author={Curtis G. Northcutt and Lu Jiang and Isaac L. Chuang},
    journal={Journal of Artificial Intelligence Research (JAIR)},
    volume={70},
    pages={1373--1411},
    year={2021}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/1705.01936" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">排名修剪（UAI '17）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{northcutt2017rankpruning,
    author={Northcutt, Curtis G. and Wu, Tailin and Chuang, Isaac L.},
    title={Learning with Confident Examples: Rank Pruning for Robust Classification with Noisy Labels},
    booktitle = {Proceedings of the Thirty-Third Conference on Uncertainty in Artificial Intelligence},
    series = {UAI'17},
    year = {2017},
    location = {Sydney, Australia},
    numpages = {10},
    url = {http://auai.org/uai2017/proceedings/papers/35.pdf},
    publisher = {AUAI Press},
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{northcutt2017rankpruning,
    author={Northcutt, Curtis G. and Wu, Tailin and Chuang, Isaac L.},
    title={Learning with Confident Examples: Rank Pruning for Robust Classification with Noisy Labels},
    booktitle = {Proceedings of the Thirty-Third Conference on Uncertainty in Artificial Intelligence},
    series = {UAI'17},
    year = {2017},
    location = {Sydney, Australia},
    numpages = {10},
    url = {http://auai.org/uai2017/proceedings/papers/35.pdf},
    publisher = {AUAI Press},
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://people.csail.mit.edu/jonasmueller/info/LabelQuality_icml.pdf" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标签质量评分 (ICML '22)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{kuan2022labelquality,
    title={Model-agnostic label quality scoring to detect real-world label errors},
    author={Kuan, Johnson and Mueller, Jonas},
    booktitle={ICML DataPerf Workshop},
    year={2022}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{kuan2022labelquality,
    title={Model-agnostic label quality scoring to detect real-world label errors},
    author={Kuan, Johnson and Mueller, Jonas},
    booktitle={ICML DataPerf Workshop},
    year={2022}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2207.03061" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">分布外检测 (ICML '22)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{kuan2022ood,
    title={Back to the Basics: Revisiting Out-of-Distribution Detection Baselines},
    author={Kuan, Johnson and Mueller, Jonas},
    booktitle={ICML Workshop on Principles of Distribution Shift},
    year={2022}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{kuan2022ood,
    title={Back to the Basics: Revisiting Out-of-Distribution Detection Baselines},
    author={Kuan, Johnson and Mueller, Jonas},
    booktitle={ICML Workshop on Principles of Distribution Shift},
    year={2022}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2210.03920" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">令牌分类标签错误 (NeurIPS '22)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{wang2022tokenerrors,
    title={Detecting label errors in token classification data},
    author={Wang, Wei-Chen and Mueller, Jonas},
    booktitle={NeurIPS Workshop on Interactive Learning for Natural Language Processing (InterNLP)},
    year={2022}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{wang2022tokenerrors,
    title={Detecting label errors in token classification data},
    author={Wang, Wei-Chen and Mueller, Jonas},
    booktitle={NeurIPS Workshop on Interactive Learning for Natural Language Processing (InterNLP)},
    year={2022}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2210.06812" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用于具有多个注释器的数据的 CROWDLAB (NeurIPS '22)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{goh2022crowdlab,
    title={CROWDLAB: Supervised learning to infer consensus labels and quality scores for data with multiple annotators},
    author={Goh, Hui Wen and Tkachenko, Ulyana and Mueller, Jonas},
    booktitle={NeurIPS Human in the Loop Learning Workshop},
    year={2022}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{goh2022crowdlab,
    title={CROWDLAB: Supervised learning to infer consensus labels and quality scores for data with multiple annotators},
    author={Goh, Hui Wen and Tkachenko, Ulyana and Mueller, Jonas},
    booktitle={NeurIPS Human in the Loop Learning Workshop},
    year={2022}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2301.11856" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ActiveLab：通过数据重新标记进行主动学习 (ICLR '23)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{goh2023activelab,
    title={ActiveLab: Active Learning with Re-Labeling by Multiple Annotators},
    author={Goh, Hui Wen and Mueller, Jonas},
    booktitle={ICLR Workshop on Trustworthy ML},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{goh2023activelab,
    title={ActiveLab: Active Learning with Re-Labeling by Multiple Annotators},
    author={Goh, Hui Wen and Mueller, Jonas},
    booktitle={ICLR Workshop on Trustworthy ML},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2211.13895" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多标签分类中的不正确注释（ICLR '23）</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{thyagarajan2023multilabel,
    title={Identifying Incorrect Annotations in Multi-Label Classification Data},
    author={Thyagarajan, Aditya and Snorrason, Elías and Northcutt, Curtis and Mueller, Jonas},
    booktitle={ICLR Workshop on Trustworthy ML},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{thyagarajan2023multilabel,
    title={Identifying Incorrect Annotations in Multi-Label Classification Data},
    author={Thyagarajan, Aditya and Snorrason, Elías and Northcutt, Curtis and Mueller, Jonas},
    booktitle={ICLR Workshop on Trustworthy ML},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2305.15696" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检测数据集漂移和非独立同分布采样 (ICML '23)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{cummings2023drift,
    title={Detecting Dataset Drift and Non-IID Sampling via k-Nearest Neighbors},
    author={Cummings, Jesse and Snorrason, Elías and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{cummings2023drift,
    title={Detecting Dataset Drift and Non-IID Sampling via k-Nearest Neighbors},
    author={Cummings, Jesse and Snorrason, Elías and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2305.16583" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检测数值数据中的错误 (ICML '23)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">点击显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{zhou2023errors,
    title={Detecting Errors in Numerical Data via any Regression Model},
    author={Zhou, Hang and Mueller, Jonas and Kumar, Mayank and Wang, Jane-Ling and Lei, Jing},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{zhou2023errors,
    title={Detecting Errors in Numerical Data via any Regression Model},
    author={Zhou, Hang and Mueller, Jonas and Kumar, Mayank and Wang, Jane-Ling and Lei, Jing},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2309.00832" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ObjectLab：对象检测数据中错误标记的图像 (ICML '23)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单击以显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{tkachenko2023objectlab,
    title={ObjectLab: Automated Diagnosis of Mislabeled Images in Object Detection Data},
    author={Tkachenko, Ulyana and Thyagarajan, Aditya and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{tkachenko2023objectlab,
    title={ObjectLab: Automated Diagnosis of Mislabeled Images in Object Detection Data},
    author={Tkachenko, Ulyana and Thyagarajan, Aditya and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<details><summary><a href="https://arxiv.org/abs/2307.05080" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">分段数据中的标签错误 (ICML '23)</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（</font></font><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单击以显示 bibtex</font></font></b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）</font></font></summary>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@inproceedings{lad2023segmentation,
    title={Estimating label quality and errors in semantic segmentation data via any model},
    author={Lad, Vedang and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{lad2023segmentation,
    title={Estimating label quality and errors in semantic segmentation data via any model},
    author={Lad, Vedang and Mueller, Jonas},
    booktitle={ICML Workshop on Data-centric Machine Learning Research},
    year={2023}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</details>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要了解/引用上面未描述的其他 cleanlab 功能，请查看我们的</font></font><a href="https://cleanlab.ai/research/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其他出版物</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-other-resources" class="anchor" aria-hidden="true" tabindex="-1" href="#other-resources"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其他资源</font></font></h2>
<ul dir="auto">
<li>
<p dir="auto"><a href="https://github.com/cleanlab/examples"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示该软件包实际应用的示例笔记本</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://cleanlab.ai/blog/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Cleanlab 博客</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://l7.curtisnorthcutt.com/confident-learning" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客文章：自信学习简介</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://arxiv.org/abs/2103.14749" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">NeurIPS 2021 论文：测试集中普遍存在的标签错误破坏了机器学习基准的稳定性</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://dcai.csail.mit.edu/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以数据为中心的人工智能简介（麻省理工学院 IAP 课程 2023）</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://github.com/cleanlab/cleanlab/releases"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">过去版本的发行说明</font></font></a></p>
</li>
<li>
<p dir="auto"><a href="https://cleanlab.ai/studio/?utm_source=github&amp;utm_medium=readme&amp;utm_campaign=clostostudio" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Cleanlab Studio</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无代码数据改进</font></font></em></p>
</li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">虽然这个开源库</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以发现</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据问题，但它的实用性取决于您是否拥有合适的现有 ML 模型和接口来有效地</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">解决</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据集中的这些问题。</font></font><a href="https://cleanlab.ai/studio/?utm_source=github&amp;utm_medium=readme&amp;utm_campaign=clostostudio" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Cleanlab Studio</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提供所有这些功能，</font><font style="vertical-align: inherit;">是一个无代码平台，用于</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">查找和修复</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现实 ML 数据集中的问题。</font><font style="vertical-align: inherit;">Cleanlab Studio在适合您的数据的 AutoML 和 Foundation 模型之上</font></font><a href="https://cleanlab.ai/blog/data-centric-ai/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自动运行</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此开源库中算法的优化版本，并在智能数据编辑界面中显示检测到的问题。</font><font style="vertical-align: inherit;">它是一个数据清理助手，可以快速将不可靠的数据转化为可靠的模型/见解（通过人工智能/自动化+简化的用户体验）。</font></font><a href="https://cleanlab.ai/signup" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">免费试用！</font></font></a></p>
<p align="center" dir="auto">
  <a target="_blank" rel="noopener noreferrer nofollow" href="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/studio.png"><img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/studio.png" width="80%" height="80%" alt="Cleanlab 工作室徽标" style="max-width: 100%;"></a>
</p>
<h2 tabindex="-1" dir="auto"><a id="user-content-join-our-community" class="anchor" aria-hidden="true" tabindex="-1" href="#join-our-community"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加入我们的社区</font></font></h2>
<ul dir="auto">
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最好的学习场所是</font></font><a href="https://cleanlab.ai/slack" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的 Slack 社区</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对清洁实验室的未来有什么想法吗？</font><font style="vertical-align: inherit;">您如何使用 cleanlab？</font></font><a href="https://github.com/cleanlab/cleanlab/discussions"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加入讨论</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并查看</font></font><a href="https://github.com/cleanlab/cleanlab/projects"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们正在进行的/计划中的项目以及我们可以在哪些方面需要您的帮助</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有兴趣贡献吗？</font><font style="vertical-align: inherit;">请参阅</font></font><a href="/cleanlab/cleanlab/blob/master/CONTRIBUTING.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贡献指南</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://github.com/cleanlab/cleanlab/wiki#ideas-for-contributing-to-cleanlab"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有用贡献的想法</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们欢迎您帮助构建以数据为中心的人工智能的标准开源平台！</font></font></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 的代码有改进吗？</font><font style="vertical-align: inherit;">参见</font></font><a href="/cleanlab/cleanlab/blob/master/DEVELOPMENT.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开发指南</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对 cleanlab 有疑问吗？</font><font style="vertical-align: inherit;">搜索</font></font><a href="https://docs.cleanlab.ai/stable/tutorials/faq.html" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的常见问题解答</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://github.com/cleanlab/cleanlab/issues?q=is%3Aissue"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">现有问题</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，或</font></font><a href="https://github.com/cleanlab/cleanlab/issues/new"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提交新问题</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
</li>
<li>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">需要 cleanlab 方面的专业帮助吗？</font><font style="vertical-align: inherit;">加入我们的</font></font><a href="https://cleanlab.ai/slack" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">#help Slack 频道</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并向我们发送消息，或通过电子邮件联系：</font></font><a href="mailto:team@cleanlab.ai"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">team@cleanlab.ai</font></font></a></p>
</li>
</ul>
<h2 tabindex="-1" dir="auto"><a id="user-content-license" class="anchor" aria-hidden="true" tabindex="-1" href="#license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执照</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">版权所有 (c) 2017 Cleanlab Inc.</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 是免费软件：您可以根据自由软件基金会发布的 GNU Affero 通用公共许可证（许可证的第 3 版）或（由您选择）任何更高版本的条款重新分发和/或修改它。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">cleanlab 的发布是希望它有用，但不提供任何保证；</font><font style="vertical-align: inherit;">甚至没有适销性或特定用途适用性的默示保证。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有关详细信息，请参阅</font></font><a href="https://github.com/cleanlab/cleanlab/blob/master/LICENSE"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GNU Affero 通用公共许可证</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">您可以给我们发电子邮件讨论许可事宜：</font></font><a href="mailto:team@cleanlab.ai"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">team@cleanlab.ai</font></font></a></p>
<h3 tabindex="-1" dir="auto"><a id="user-content-commercial-licensing" class="anchor" aria-hidden="true" tabindex="-1" href="#commercial-licensing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">商业许可</font></font></h3>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://github.com/cleanlab/cleanlab/blob/master/LICENSE"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">商业许可适用于想要在生产工作流程中使用 cleanlab 但无法按照当前许可证的要求</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开源其代码的团队和企业</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">请给我们发电子邮件：</font></font><a href="mailto:team@cleanlab.ai"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">team@cleanlab.ai</font></font></a></p>
</article></div>
