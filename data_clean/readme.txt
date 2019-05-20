该项目是基于一位推特用户对狗评分的数据集。

**项目目标**：清洗 WeRateDogs 推特数据，创建有趣且可靠的分析和可视化。

****

该项目包括以下文件：

- `wrangle_act.ipynb`：用于收集、评估、清洗、分析和可视化数据的代码
- `wrangle_report.pdf`：汇总数据整理步骤的文档：收集，评估和清洗
- `act_report.pdf`：对最终数据进行观察与分析的文档
- `twitter_archive_enhanced.csv`：给定的文件
- `image_predictions.tsv`：以编程方式下载的文件
- `tweet_json.txt`：通过 API 构建的文件
- `twitter_archive_master.csv`：合并与清洗后的数据





其中，image_predictions.tsv表中各列含义：



- `tweet_id` 是推特链接的最后一部分，位于 "status/" 后面 → <https://twitter.com/dog_rates/status/889531135344209921>
- `jpg_url` 是预测的图像资源链接
- `img_num` 最可信的预测结果对应的图像编号 → 1 推特中的第一张图片
- `p1` 是算法对推特中图片的一号预测 → 金毛犬
- `p1_conf` 是算法的一号预测的可信度 → 95%
- `p1_dog` 是一号预测该图片是否属于“狗”（有可能是其他物种，比如熊、马等） → True 真
- `p2` 是算法对推特中图片预测的第二种可能性 → 拉布拉多犬
- `p2_conf` 是算法的二号预测的可信度 → 1%
- `p2_dog` 是二号预测该图片是否属于“狗” → True 真
- 以此类推...