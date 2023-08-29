## MESA-Web
#### 为什么用MESA-Web？
MESA-Web没有MESA那么复杂的安装方式，而是直接在网页上提交，在邮件上接收，参数也非常简单

但是，MESA-Web没有MESA的高级功能，也不能进行恒星工程，而且没法改变PGSTAR


#### 提交页面
1.打开这个网站：[MESA-Web提交页面](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-submit)，或打开[主页面](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web)并进入calculation submission

2.参数说明：

​	Initial Properties：

| 名称          | 含义     | 单位   | 类型+范围         |
| ------------- | -------- | ------ | ----------------- |
| Mass          | 初始质量 | Msun   | 输入值；[0.1-100] |
| Metallicity   | 金属量   | (分数) | 选择；[.0001-.04] |
| Rotation Rate | 初始转速 | (分数) | 输入值；[0-1]     |

​	Nuclear Reactions：

| 名称                         | 含义           | 备注               |
| ---------------------------- | -------------- | ------------------ |
| Network                      | 核反应网络     | 解释见下           |
| Custom Nuclear Reaction Rate | 自定义反应速率 | 只能定义一个       |
| Upload Rate                  | 上传速率表     | 与上面必须配合使用 |

| 名称           | 说明                        | 建议场景         |
| -------------- | --------------------------- | ---------------- |
| basic          | 基础，速度快                | 一般H/He燃烧     |
| agb            | AGB扩展核反应网             | 小质量恒星，AGB  |
| approx21       | 大质量恒星，包括到铁的核素  | 大质量恒星       |
| co_burn        | 加入CO网络                  | 一般H/He/C/O燃烧 |
| h_burn         | 详细的H燃烧                 | 只有主序星       |
| mesa_49        | 详细的核反应网络，速度慢    | 详细H/He燃烧     |
| sagb_NeNa_MgAl | 加入适用于C燃烧的详细核反应 | SAGB/中质量恒星  |

​	Mixing：

​	Convection：

| 名称                                                         | 说明           | 备注                       |
| ------------------------------------------------------------ | -------------- | -------------------------- |
| Mixing Length Alpha                                          | 混合长参数     | >=0                        |
| [Mixing Length Theory Prescription](http://user.astro.wisc.edu/~townsend/static.php?ref=mesa-web-input#mltpresc) | 混合长处理方法 | 打开前面的网址查看         |
| Convective Premixing                                         | 对流预混       | 混合错误可以尝试打开或关闭 |

