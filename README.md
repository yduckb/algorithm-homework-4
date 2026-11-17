# algorithm-homework-4
4th homework
# YOLOv5 目标检测作业

## 1. 视频来源
B站下载视频，截取了前14秒。

## 2. 类别名称与标注数量
* 类别名称：['Rick Astley', 'microphone', 'shoe', 'actress']
* 标注数量：Rick Astley : 36个; microphone : 18个; shoe : 7个; actress : 16个

## 3. 数据集划分
按 8:2 的比例划分。
* 训练集：45 张图片（放在 `my_project/images/train`）
* 验证集：11 张图片（放在 `my_project/images/val`）

## 4. 验证集指标
* Precision (P): 0.783
* Recall (R): 0.778
* mAP50: 0.956
* mAP50-95: 0.839

## 5. 遇到的问题与解决
* 标注时遇到labelImg闪退，降低PyQt5版本后解决了。
* 训练时遇到numpy报错，将numpy降级到1.26.4后解决了。
* 验证集一开始没读取到标签，删除了.cache缓存文件后重新训练恢复正常。
