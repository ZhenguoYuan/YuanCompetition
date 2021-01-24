## 先上结果
- 使用1024x1024尺寸，步长为512切图，可得有标注的`coco`格式数据集3.8万，见[0_split.ipynb](https://github.com/ZhenguoYuan/YuanCompetition/blob/main/%E7%93%B7%E7%A0%96%E8%A1%A8%E9%9D%A2%E7%91%95%E7%96%B5%E6%99%BA%E8%83%BD%E6%A3%80%E6%B5%8B-2021%E5%B9%BF%E4%B8%9C%E5%B7%A5%E4%B8%9A%E6%99%BA%E9%80%A0%E5%88%9B%E6%96%B0%E5%A4%A7%E8%B5%9B/0_split.ipynb)
-使用单进程切图，目前较慢，如果成绩高了再考虑多进程优化；批预测(batchsize=28)转换为单张大图预测时间约为5秒/张
- 训练只使用有标注的数据，预测使用批预测[1_inference_paddle.ipynb](https://github.com/ZhenguoYuan/YuanCompetition/blob/main/%E7%93%B7%E7%A0%96%E8%A1%A8%E9%9D%A2%E7%91%95%E7%96%B5%E6%99%BA%E8%83%BD%E6%A3%80%E6%B5%8B-2021%E5%B9%BF%E4%B8%9C%E5%B7%A5%E4%B8%9A%E6%99%BA%E9%80%A0%E5%88%9B%E6%96%B0%E5%A4%A7%E8%B5%9B/1_inference_paddle.ipynb)
- 提交结果59分

# 环境配置

## 训练-百度AI Studio
- fork自[weihongwei](https://tianchi.aliyun.com/forum/postDetail?postId=163756)
- 数据预处理部分亦修改自[weihongwei](https://tianchi.aliyun.com/forum/postDetail?postId=163756)
## 测试-本地机
GPU: 2080TI 11G

## requirements
- [ensemble-boxes](https://github.com/ZFTurbo/Weighted-Boxes-Fusion)
- [paddlepaddle-gpu==2.0.0rc1](https://www.paddlepaddle.org.cn)

## 修改记录
- 20210124 上传图像切块, 批预测ipynb

    


