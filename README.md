# 欢迎使用数据集标注小程序

基于python的数据集处理和标注小程序，没啥bug，可以将视频分解为图片，然后手动进行标注，程序会自动输出被标注的图片，标注的txt文件，后续可将其转变为mat文件以及您可能会用到的densitymat文件。

--

## 如何使用

首先，博主使用的环境：
win11
anaconda-navigator
pycharm
python3.9+
（在大多数环境下应该都可以使用）

---

调用的库有：
cv2
os
pil
pandas
numpy
scipy
您可以使用以下代码安装他们：

```js
pip install opencv-python -i -`https://pypi.tuna.tsinghua.edu.cn/simple
```

---

> 在进入库后，打开Video_cutting_code文件

> cutted为将视频剪切为照片，您需要确定每隔多少帧截取一张，视频应该导入主目录video文件下

> 接下来，您会在results/images/to_be_processed中看见它们

> 接下来运行label文件开始标注，

> 您需要点击需要标注的地方，下方终端会显示你标注得到的点(x,y)

> 功能键有：

> “q“退出并保存当前文件

> ”d“删除标注的最后一个点

> ”b“查看上一张及标注

> ”s”保存当前图片及标注

> 所有标注过的图片会保存在\results\images\annotated_image下

> 标注得到的txt文件会保存在\Dataset_labeling\results\txt\1文件夹下

> 程序会读取这个文件夹中的txt文件以告知您您已经标注过的点，如果您要标注新的点，请删除旧文件。

> 接下来运行txt_to_mat文件将其转化为mat文件在\Dataset_labeling\results\mat\1下

> 如有需要可以运行to_densitymat程序将mat其转变为density的cvs文件


> 作者：tjUni- lzy

