# 品牌设计风格注册表

> **版本**: v2.0.0
> **说明**: 本文件是 ui-design-aitool-plus Skill 的核心参考文件，定义了100家知名互联网/科技公司的设计风格规范。国内80家 + 国外20家，以国内大厂为主重新分类。每个品牌包含唯一 slug、风格描述、主色、平台类型和设计关键词，供设计生成时快速检索与引用。每个品牌均有独立的设计规范文件（`references/brands/{slug}.md`），包含完整的9大章节（设计价值观、配色体系、字体排版、组件规范、间距圆角、动效规范、暗色模式、设计禁忌、CSS变量参考），可直接作为AI生成的约束参考。
> **获取完整设计规范**: `npx getdesign@latest add <slug>`

---

## 一、国内互联网巨头（15家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 1 | `tencent` | 腾讯 | Tencent | 社交绿洲·连接万物·生态织网 | `#07C160` | Cross | 社交织网/生态绿/即时连接 | `references/brands/tencent.md` |
| 2 | `alibaba` | 阿里巴巴 | Alibaba | 商业橙光·让天下没有难做的生意 | `#FF6A00` | Web | 商业橙/平台经济/数据驱动 | `references/brands/alibaba.md` |
| 3 | `bytedance` | 字节跳动 | ByteDance | 算法彩虹·内容宇宙·激发创造 | `#161823` | Cross | 算法驱动/内容宇宙/多彩信息流 | `references/brands/bytedance.md` |
| 4 | `huawei-dev` | 华为 | Huawei | 全场景红·科技自立·智慧全连接 | `#CF0A2C` | Cross | 全场景/科技红/智慧连接 | `references/brands/huawei-dev.md` |
| 5 | `xiaomi-dev` | 小米 | Xiaomi | 澎湃橙·感动人心·价格厚道 | `#FF6700` | Cross | 澎湃橙/性价比/生态互联 | `references/brands/xiaomi-dev.md` |
| 6 | `jd-com` | 京东 | JD.com | 品质红·多快好省·信赖之选 | `#E2231A` | Web | 品质红/物流速达/正品保障 | `references/brands/jd-com.md` |
| 7 | `meituan` | 美团 | Meituan | 生活黄·吃喝玩乐·即时送达 | `#FFD100` | Cross | 生活黄/即时配送/本地服务 | `references/brands/meituan.md` |
| 8 | `didi` | 滴滴 | DiDi | 出行橙·安全到达·一路顺风 | `#FF7F27` | Cross | 出行橙/安全守护/智能调度 | `references/brands/didi.md` |
| 9 | `netease` | 网易 | NetEase | 态度红·有态度·匠心内容 | `#C10A0A` | Web | 态度红/匠心内容/社区氛围 | `references/brands/netease.md` |
| 10 | `bilibili` | B站 | Bilibili | Z次元蓝·弹幕宇宙·兴趣部落 | `#00A1D6` | Web | Z次元/弹幕文化/粉蓝渐变 | `references/brands/bilibili.md` |
| 11 | `douyin` | 抖音 | Douyin | 沉浸黑·全屏世界·记录美好生活 | `#161823` | Cross | 沉浸黑/全屏滑动/动感节奏 | `references/brands/douyin.md` |
| 12 | `wechat` | 微信 | WeChat | 社交绿·一个生活方式·小程序生态 | `#07C160` | Cross | 社交绿/小程序/轻量连接 | `references/brands/wechat.md` |
| 13 | `alipay` | 支付宝 | Alipay | 信任蓝·支付无忧·生活服务 | `#1677FF` | Cross | 信任蓝/金融安全/生活服务 | `references/brands/alipay.md` |
| 14 | `taobao` | 淘宝 | Taobao | 发现橙红·淘你喜欢·万能市场 | `#FF5000` | Cross | 发现橙红/万能市场/逛感设计 | `references/brands/taobao.md` |
| 15 | `pinduoduo` | 拼多多 | Pinduoduo | 拼团红·百亿补贴·多人成团 | `#E02E24` | Cross | 拼团红/社交裂变/下沉友好 | `references/brands/pinduoduo.md` |

---

## 二、国内AI与科技新锐（15家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 16 | `baidu` | 百度 | Baidu | 搜索蓝·智能搜索·文心一言 | `#2932E1` | Web | 搜索蓝/AI大模型/信息检索 | `references/brands/baidu.md` |
| 17 | `deepseek` | DeepSeek | DeepSeek | 深度蓝紫·开源先锋·推理之光 | `#4D6BFE` | Web | 深度蓝紫/开源推理/暗色科技 | `references/brands/deepseek.md` |
| 18 | `kimi` | Kimi | Moonshot AI | 长文蓝·超长上下文·智能阅读 | `#4F6BED` | Web | 长文蓝/智能阅读/上下文理解 | `references/brands/kimi.md` |
| 19 | `zhipu` | 智谱 | Zhipu AI | 学术蓝绿·GLM大模型·知识引擎 | `#3B82F6` | Web | 学术蓝绿/知识引擎/国产大模型 | `references/brands/zhipu.md` |
| 20 | `qwen` | 通义千问 | Qwen | 通义橙·阿里AI·万知万能 | `#6236FF` | Web | 通义紫/阿里系AI/多模态 | `references/brands/qwen.md` |
| 21 | `doubao` | 豆包 | Doubao | 活力橙·字节AI·创意无限 | `#FF6B2B` | Web | 活力橙/字节系AI/创意工具 | `references/brands/doubao.md` |
| 22 | `yuanbao` | 元宝 | Yuanbao | 金融金·腾讯AI·理财智慧 | `#D4A017` | Web | 金融金/腾讯系AI/理财助手 | `references/brands/yuanbao.md` |
| 23 | `tiangong` | 天工 | Tiangong | 天工蓝·昆仑万维·搜索增强 | `#1E90FF` | Web | 天工蓝/搜索增强/AI助手 | `references/brands/tiangong.md` |
| 24 | `sensetime` | 商汤 | SenseTime | 视觉紫·AI视觉·智慧赋能 | `#7B2D8E` | Web | 视觉紫/AI视觉/智慧城市 | `references/brands/sensetime.md` |
| 25 | `iflytek` | 科大讯飞 | iFlytek | 语音蓝·AI语音·听见未来 | `#005BAC` | Web | 语音蓝/AI语音/智能交互 | `references/brands/iflytek.md` |
| 26 | `minimax` | MiniMax | MiniMax | 创意紫红·多模态·角色扮演 | `#6B21A8` | Web | 创意紫红/多模态/角色AI | `references/brands/minimax.md` |
| 27 | `stepfun` | 阶跃星辰 | StepFun | 星辰蓝·跃迁智能·多模态 | `#2563EB` | Web | 星辰蓝/跃迁智能/多模态 | `references/brands/stepfun.md` |
| 28 | `baichuan` | 百川智能 | Baichuan | 百川绿·汇聚百川·知识流淌 | `#059669` | Web | 百川绿/知识汇聚/中文大模型 | `references/brands/baichuan.md` |
| 29 | `moonshot` | Moonshot | Moonshot | 月光银·登月精神·长文本 | `#94A3B8` | Web | 月光银/登月精神/长文本 | `references/brands/moonshot.md` |
| 30 | `01ai` | 零一万物 | 01.AI | 零一黑金·从0到1·万物生 | `#1A1A2E` | Web | 零一黑金/从0到1/万物生 | `references/brands/01ai.md` |

---

## 三、国内电商与本地生活（10家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 31 | `pdd-temu` | Temu | Temu | 全球橙红·低价风暴·席卷全球 | `#F64400` | Web | 全球橙红/低价风暴/跨境出海 | `references/brands/pdd-temu.md` |
| 32 | `shein` | SHEIN | SHEIN | 时尚黑·快时尚帝国·全球穿搭 | `#000000` | Web | 时尚黑/快时尚/全球穿搭 | `references/brands/shein.md` |
| 33 | `vipshop` | 唯品会 | Vipshop | 特卖粉·品牌特卖·正品折扣 | `#FF2D5B` | Web | 特卖粉/品牌折扣/限时抢购 | `references/brands/vipshop.md` |
| 34 | `suning` | 苏宁 | Suning | 易购黄·智慧零售·全场景 | `#FFAA00` | Web | 易购黄/智慧零售/全场景 | `references/brands/suning.md` |
| 35 | `eleme` | 饿了么 | Ele.me | 饿了蓝·美食到家·即时配送 | `#0097FF` | Cross | 饿了蓝/美食到家/即时配送 | `references/brands/eleme.md` |
| 36 | `dianping` | 大众点评 | Dianping | 点评橙·真实评价·生活指南 | `#FF6633` | Cross | 点评橙/真实评价/生活指南 | `references/brands/dianping.md` |
| 37 | `xiaohongshu` | 小红书 | Xiaohongshu | 种草红·标记生活·消费决策 | `#FF2442` | Cross | 种草红/标记生活/消费决策 | `references/brands/xiaohongshu.md` |
| 38 | `deyi` | 得物 | Dewu | 潮流黑绿·鉴别真伪·潮流先知 | `#00C8A0` | Cross | 潮流黑绿/鉴别真伪/潮流先知 | `references/brands/deyi.md` |
| 39 | `fliggy` | 飞猪 | Fliggy | 旅行橙黄·旅行就上飞猪·全球畅游 | `#FF8C00` | Cross | 旅行橙黄/全球畅游/旅行攻略 | `references/brands/fliggy.md` |
| 40 | `ctrip` | 携程 | Ctrip | 旅行蓝·携程在手·说走就走 | `#003580` | Web | 旅行蓝/说走就走/旅行预订 | `references/brands/ctrip.md` |

---

## 四、国内金融与支付（10家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 41 | `ant-group` | 蚂蚁集团 | Ant Group | 普惠蓝·科技金融·为世界带来微小而美好的改变 | `#1677FF` | Web | 普惠蓝/科技金融/数字支付 | `references/brands/ant-group.md` |
| 42 | `lufax` | 陆金所 | LuFax | 稳健蓝绿·财富管理·安全增值 | `#00857C` | Web | 稳健蓝绿/财富管理/安全增值 | `references/brands/lufax.md` |
| 43 | `lilian` | 立林 | LiLin | 金融蓝·智能投顾·量化交易 | `#1E40AF` | Web | 金融蓝/智能投顾/量化交易 | `references/brands/lilian.md` |
| 44 | `weilai-fin` | 微众银行 | WeBank | 微众蓝·数字银行·普惠金融 | `#2B6CB0` | Web | 微众蓝/数字银行/普惠金融 | `references/brands/weilai-fin.md` |
| 45 | `zhongxin` | 中信 | CITIC | 中信红·综合金融·信任价值 | `#C41230` | Web | 中信红/综合金融/信任价值 | `references/brands/zhongxin.md` |
| 46 | `pingan` | 平安 | Ping An | 平安橙·金融+科技·专业价值 | `#FF6600` | Web | 平安橙/金融科技/专业价值 | `references/brands/pingan.md` |
| 47 | `unionpay` | 银联 | UnionPay | 银联蓝·联合支付·全球网络 | `#004F9F` | Web | 银联蓝/联合支付/全球网络 | `references/brands/unionpay.md` |
| 48 | `jd-finance` | 京东金融 | JD Finance | 金融红·财富管理·科技赋能 | `#E2231A` | Web | 金融红/财富管理/科技赋能 | `references/brands/jd-finance.md` |
| 49 | `boc` | 中国银行 | BOC | 中行红蓝·全球化银行·稳健经营 | `#C41230` | Web | 中行红蓝/全球化/稳健经营 | `references/brands/boc.md` |
| 50 | `cmb` | 招商银行 | CMB | 金葵花·因您而变·财富管理 | `#CC1931` | Web | 金葵花/因您而变/财富管理 | `references/brands/cmb.md` |

---

## 五、国内SaaS与企业服务（10家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 51 | `feishu` | 飞书 | Feishu | 协作紫·先进协作·高效愉悦 | `#7B67EE` | Cross | 协作紫/先进团队/高效愉悦 | `references/brands/feishu.md` |
| 52 | `dingtalk` | 钉钉 | DingTalk | 效率蓝·让工作更简单·数字化 | `#0089FF` | Cross | 效率蓝/数字化/让工作简单 | `references/brands/dingtalk.md` |
| 53 | `yuque` | 语雀 | Yuque | 知识绿·文档协作·知识管理 | `#25B864` | Web | 知识绿/文档协作/知识管理 | `references/brands/yuque.md` |
| 54 | `teambition` | Teambition | Teambition | 项目蓝·项目协作·目标驱动 | `#2B6CB0` | Web | 项目蓝/目标驱动/协作看板 | `references/brands/teambition.md` |
| 55 | `canva-cn` | 创客贴 | Chuangkit | 设计橙·在线设计·一键出图 | `#FF6B35` | Web | 设计橙/在线设计/一键出图 | `references/brands/canva-cn.md` |
| 56 | `wps` | WPS | WPS Office | 办公蓝·智慧办公·多端协同 | `#2B5FD9` | Cross | 办公蓝/智慧办公/多端协同 | `references/brands/wps.md` |
| 57 | `kingdee` | 金蝶 | Kingdee | 管理蓝·企业管理·数字转型 | `#0052D9` | Web | 管理蓝/企业ERP/数字转型 | `references/brands/kingdee.md` |
| 58 | `yida` | 宜搭 | YiDa | 低代码蓝·应用搭建·敏捷开发 | `#1677FF` | Web | 低代码蓝/应用搭建/敏捷开发 | `references/brands/yida.md` |
| 59 | `huawei-cloud` | 华为云 | Huawei Cloud | 云端红·智能云·一切皆服务 | `#CF0A2C` | Web | 云端红/智能云/一切皆服务 | `references/brands/huawei-cloud.md` |
| 60 | `aliyun` | 阿里云 | Alibaba Cloud | 计算橙·数字经济·智能算力 | `#FF6A00` | Web | 计算橙/智能算力/数字经济 | `references/brands/aliyun.md` |

---

## 六、国内媒体与内容（10家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 61 | `weibo` | 微博 | Weibo | 热搜红·随时随地·发现新鲜事 | `#E6162D` | Web | 热搜红/发现新鲜事/社交广场 | `references/brands/weibo.md` |
| 62 | `zhihu` | 知乎 | Zhihu | 知识蓝·有问题就会有答案 | `#0066FF` | Web | 知识蓝/问答社区/专业讨论 | `references/brands/zhihu.md` |
| 63 | `kuaishou` | 快手 | Kuaishou | 拥抱橙·拥抱每一种生活 | `#FF4906` | Cross | 拥抱橙/每一种生活/短视频 | `references/brands/kuaishou.md` |
| 64 | `toutiao` | 今日头条 | Toutiao | 信息红·信息创造价值·算法推荐 | `#D4232A` | Cross | 信息红/算法推荐/信息流 | `references/brands/toutiao.md` |
| 65 | `iqiyi` | 爱奇艺 | iQIYI | 娱乐绿·悦享品质·追剧沉浸 | `#00BE06` | Web | 娱乐绿/悦享品质/追剧沉浸 | `references/brands/iqiyi.md` |
| 66 | `youku` | 优酷 | Youku | 视界蓝·这世界很酷·视频沉浸 | `#1A9CFC` | Web | 视界蓝/这世界很酷/视频沉浸 | `references/brands/youku.md` |
| 67 | `netease-music` | 网易云音乐 | NetEase Music | 音乐红·音乐的力量·社区共鸣 | `#C20C0C` | Cross | 音乐红/社区共鸣/歌单文化 | `references/brands/netease-music.md` |
| 68 | `qq-music` | QQ音乐 | QQ Music | 听歌绿·听我想听·音乐生活 | `#31C27C` | Cross | 听歌绿/音乐生活/海量曲库 | `references/brands/qq-music.md` |
| 69 | `jianshu` | 简书 | JianShu | 创作红·创作你的创作·文字之美 | `#EA6F5A` | Web | 创作红/文字之美/创作社区 | `references/brands/jianshu.md` |
| 70 | `csdn` | CSDN | CSDN | 开发红·成就一亿技术人 | `#FC5531` | Web | 开发红/技术社区/知识分享 | `references/brands/csdn.md` |

---

## 七、国内出行与汽车（10家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 71 | `nio` | 蔚来 | NIO | 用户蓝·用户企业·Blue Sky Coming | `#00BEFF` | Web | 用户蓝/生活方式/换电生态 | `references/brands/nio.md` |
| 72 | `byd` | 比亚迪 | BYD | 新能红·Build Your Dreams·技术为王 | `#C41230` | Web | 新能红/技术为王/新能源 | `references/brands/byd.md` |
| 73 | `xpeng` | 小鹏 | XPeng | 智驾蓝·未来出行·智能驾驶 | `#0052D9` | Web | 智驾蓝/未来出行/智能驾驶 | `references/brands/xpeng.md` |
| 74 | `lixiang` | 理想 | Li Auto | 家庭绿·创造移动的家·幸福家 | `#00C853` | Web | 家庭绿/移动的家/增程电动 | `references/brands/lixiang.md` |
| 75 | `geely` | 吉利 | Geely | 远景蓝·造每个人的精品车 | `#005BAC` | Web | 远景蓝/精品车/多品牌矩阵 | `references/brands/geely.md` |
| 76 | `gac-aion` | 广汽埃安 | GAC Aion | 先行绿·先人一步·科技先行 | `#00A651` | Web | 先行绿/科技先行/纯电专属 | `references/brands/gac-aion.md` |
| 77 | `changan` | 长安 | Changan | 长安蓝·百年长安·智造未来 | `#003399` | Web | 长安蓝/百年品牌/智造未来 | `references/brands/changan.md` |
| 78 | `saic` | 上汽 | SAIC | 蓝天白·绿色出行·智慧交通 | `#005BAC` | Web | 蓝天白/绿色出行/智慧交通 | `references/brands/saic.md` |
| 79 | `baidu-apollo` | 百度Apollo | Baidu Apollo | 自动驾驶蓝·萝卜快跑·智能出行 | `#2932E1` | Web | 自动驾驶蓝/萝卜快跑/智能出行 | `references/brands/baidu-apollo.md` |
| 80 | `haige` | 高德地图 | Amap | 导航蓝·出行更准·地图导航 | `#0D96FF` | Cross | 导航蓝/出行更准/地图导航 | `references/brands/haige.md` |

---

## 八、全球科技与品牌（20家）

| # | Slug | 中文名 | 英文名 | 一句话风格描述 | 主色 | 平台 | 设计风格关键词 | 规范文件 |
|---|------|--------|--------|---------------|------|------|--------------|---------|
| 81 | `apple` | Apple | Apple | 极简留白·像素完美·设计即哲学 | `#007AFF` | iOS | 极简留白/像素完美/设计哲学 | `references/brands/apple.md` |
| 82 | `google` | Google | Google | 动态取色·Material You·响应一切 | `#4285F4` | Android | 动态取色/Material You/响应式 | `references/brands/google.md` |
| 83 | `microsoft` | Microsoft | Microsoft | 流光亚克力·Fluent深度·键鼠优先 | `#0078D4` | Desktop | 流光亚克力/Fluent深度/键鼠优先 | `references/brands/microsoft.md` |
| 84 | `openai` | OpenAI | OpenAI | 学术极简·渐变紫光·智能对话 | `#412991` | Web | 学术极简/渐变紫光/智能对话 | `references/brands/openai.md` |
| 85 | `meta` | Meta | Meta | 影像优先·二进制表面·社交元宇宙 | `#0668E1` | Cross | 影像优先/二进制表面/社交元宇宙 | `references/brands/meta.md` |
| 86 | `nvidia` | NVIDIA | NVIDIA | 绿黑能量·算力美学·GPU帝国 | `#76B900` | Web | 绿黑能量/算力美学/GPU帝国 | `references/brands/nvidia.md` |
| 87 | `stripe` | Stripe | Stripe | 紫色优雅·金融数据·weight-300 | `#635BFF` | Web | 紫色优雅/金融数据/轻量排版 | `references/brands/stripe.md` |
| 88 | `vercel` | Vercel | Vercel | 黑白精准·Geist字体·零配置部署 | `#000000` | Web | 黑白精准/Geist字体/零配置 | `references/brands/vercel.md` |
| 89 | `github` | GitHub | GitHub | 暗色代码·绿色合并·开发者宇宙 | `#238636` | Web | 暗色代码/绿色合并/开发者宇宙 | `references/brands/github.md` |
| 90 | `spotify` | Spotify | Spotify | 暗色沉浸·绿色药丸·音乐无界 | `#1DB954` | Web | 暗色沉浸/绿色药丸/音乐无界 | `references/brands/spotify.md` |
| 91 | `netflix` | Netflix | Netflix | 暗红全屏·沉浸观影·原创为王 | `#E50914` | Web | 暗红全屏/沉浸观影/原创为王 | `references/brands/netflix.md` |
| 92 | `tesla` | Tesla | Tesla | 减法极致·电影摄影·电动革命 | `#000000` | Web | 减法极致/电影摄影/电动革命 | `references/brands/tesla.md` |
| 93 | `figma` | Figma | Figma | 多彩协作·设计民主·实时共创 | `#F24E1E` | Web | 多彩协作/设计民主/实时共创 | `references/brands/figma.md` |
| 94 | `notion` | Notion | Notion | 暖极简·衬线标题·柔软表面 | `#000000` | Cross | 暖极简/衬线标题/柔软表面 | `references/brands/notion.md` |
| 95 | `linear` | Linear | Linear | 超极简·薰衣草蓝·精准到像素 | `#5E6AD2` | Web | 超极简/薰衣草蓝/精准像素 | `references/brands/linear.md` |
| 96 | `shopify` | Shopify | Shopify | 绿色赋能·电商自由·全球开店 | `#008060` | Web | 绿色赋能/电商自由/全球开店 | `references/brands/shopify.md` |
| 97 | `airbnb` | Airbnb | Airbnb | Belo粉红·归属体验·设计旅行 | `#FF385C` | Web | Belo粉红/归属体验/设计旅行 | `references/brands/airbnb.md` |
| 98 | `slack` | Slack | Slack | 紫色频道·协作节奏·工作流 | `#4A154B` | Web | 紫色频道/协作节奏/工作流 | `references/brands/slack.md` |
| 99 | `adobe` | Adobe | Adobe | 创意红·专业工具·设计帝国 | `#FF0000` | Web | 创意红/专业工具/设计帝国 | `references/brands/adobe.md` |
| 100 | `spacex` | SpaceX | SpaceX | 黑白未来·全出血影像·星际文明 | `#000000` | Web | 黑白未来/全出血影像/星际文明 | `references/brands/spacex.md` |

---

## 品牌选择指引

根据项目类型、设计调性和平台类型三维选择最匹配的品牌风格：

### 按项目类型选择

| 项目类型 | 推荐分类 | 推荐品牌示例 |
|---------|---------|------------|
| AI/大模型产品 | 国内AI与科技新锐 | `deepseek` `kimi` `qwen` `doubao` `zhipu` |
| 社交/即时通讯 | 国内互联网巨头 | `wechat` `qq-music` `bilibili` `weibo` |
| 电商/零售/消费 | 国内电商与本地生活 | `taobao` `pinduoduo` `xiaohongshu` `deyi` |
| 金融/支付/理财 | 国内金融与支付 | `alipay` `ant-group` `cmb` `pingan` |
| 企业协作/SaaS | 国内SaaS与企业服务 | `feishu` `dingtalk` `yuque` `wps` |
| 内容/媒体/短视频 | 国内媒体与内容 | `douyin` `kuaishou` `zhihu` `netease-music` |
| 出行/新能源/汽车 | 国内出行与汽车 | `nio` `byd` `xpeng` `lixiang` `haige` |
| 全球化/出海产品 | 全球科技与品牌 | `apple` `google` `stripe` `vercel` `shopify` |
| 开发者工具/DevOps | 全球科技与品牌 | `github` `vercel` `linear` `figma` |
| 设计工具/创意平台 | 全球科技与品牌 | `figma` `adobe` `notion` `canva-cn` |

### 按设计调性选择

| 设计调性 | 推荐品牌 |
|---------|---------|
| 极简留白 | `apple` `linear` `vercel` `tesla` `notion` |
| 暗色沉浸 | `douyin` `deepseek` `spotify` `netflix` `github` |
| 温暖友好 | `xiaohongshu` `notion` `kuaishou` `feishu` |
| 大胆动感 | `pinduoduo` `douyin` `adobe` `figma` |
| 专业信任 | `alipay` `cmb` `stripe` `ant-group` |
| 创意艺术 | `figma` `adobe` `bilibili` `minimax` |
| 社区驱动 | `zhihu` `bilibili` `csdn` `weibo` `github` |
| 未来科技 | `deepseek` `spacex` `baidu-apollo` `01ai` |
| 生活服务 | `meituan` `eleme` `dianping` `didi` `haige` |
| 金融稳健 | `cmb` `ant-group` `pingan` `unionpay` `boc` |

### 按平台类型选择

| 平台类型 | 说明 | 代表品牌 |
|---------|------|---------|
| iOS | Apple生态，遵循HIG | `apple` |
| Android | Google生态，Material You | `google` |
| Cross | 跨平台，需兼顾多端 | `wechat` `douyin` `feishu` `alipay` `didi` |
| Web | 纯Web端，自由度最高 | 大多数品牌 |
| Desktop | 桌面应用，窗口化交互 | `microsoft` `wps` |

---

## 品牌混搭规则

当项目需要融合多个品牌风格时，遵循以下规则确保设计一致性：

### 规则1：主品牌+辅品牌（1+1原则）

- **主品牌**决定整体框架：布局系统、间距体系、排版层级、交互模式
- **辅品牌**贡献局部特色：CTA按钮风格、渐变配色、特定组件样式
- 最多混搭2个品牌，超过2个会导致风格混乱

**示例**：
- `feishu`（主）+ `linear`（辅）= 协作紫框架 + 薰衣草蓝精准点缀
- `deepseek`（主）+ `vercel`（辅）= 深度蓝紫暗色底 + 黑白精准排版
- `xiaohongshu`（主）+ `figma`（辅）= 种草红生活感 + 多彩协作活力

### 规则2：色彩混搭约束

- 主色取自主品牌，辅色取自辅品牌
- 两个品牌主色色相差需≥60°（HSL色轮），避免色彩冲突
- 暗色系品牌之间可混搭（如 `deepseek` + `github`），亮色系品牌之间可混搭（如 `meituan` + `eleme`）
- 暗色+亮色混搭时，暗色品牌做底色，亮色品牌做强调色

### 规则3：排版混搭约束

- 字体体系跟随主品牌（如 `apple` 用SF Pro，`feishu` 用思源黑体）
- 辅品牌仅影响标题字重或装饰性排版，不改变正文字体族
- 衬线体与无衬线体可混搭（如 `notion` 衬线标题 + `linear` 无衬线正文）

### 规则4：组件风格混搭约束

- 基础组件（按钮、输入框、卡片）跟随主品牌风格
- 辅品牌仅影响特色组件（如 `stripe` 的渐变卡片、`spotify` 的药丸按钮）
- 交互模式（导航、弹窗、手势）统一使用主品牌规范，禁止混搭

### 规则5：禁止混搭场景

| 禁止组合 | 原因 |
|---------|------|
| `apple` + `google` | iOS HIG与Material You设计哲学根本冲突 |
| `pinduoduo` + `linear` | 拼团红社交裂变与超极简精准调性严重对立 |
| `douyin` + `notion` | 沉浸黑动感节奏与暖极简静默调性不兼容 |
| 3个及以上品牌 | 风格碎片化，无法形成统一视觉语言 |

---

## 品牌风格获取方式

获取任意品牌的完整设计规范文件（DESIGN.md），包含详细的色彩体系、排版规范、组件样式、动效参数等：

```bash
# 获取单个品牌设计规范
npx getdesign@latest add <slug>

# 示例
npx getdesign@latest add deepseek
npx getdesign@latest add feishu
npx getdesign@latest add xiaohongshu
```

获取成功后，品牌设计规范文件将保存在项目的 `.design/brands/<slug>/DESIGN.md` 路径下，供设计生成流程自动引用。

### slug 快速索引

按字母排序，方便快速查找：

`01ai` `adobe` `airbnb` `alibaba` `aliyun` `alipay` `ant-group` `apple` `baichuan`
`baidu` `baidu-apollo` `bilibili` `byd` `bytedance` `canva-cn` `changan` `cmb` `csdn`
`ctrip` `deepseek` `deyi` `dianping` `didi` `dingtalk` `doubao` `douyin` `eleme`
`feishu` `figma` `fliggy` `gac-aion` `geely` `github` `google` `haige` `huawei-cloud`
`huawei-dev` `iflytek` `iqiyi` `jd-com` `jd-finance` `jianshu` `kingdee` `kimi`
`kuaishou` `linear` `lixiang` `lilian` `lufax` `meituan` `meta` `minimax` `moonshot`
`netease` `netease-music` `netflix` `nio` `notion` `nvidia` `openai` `pdd-temu`
`pingan` `pinduoduo` `qwen` `qq-music` `sensetime` `shein` `shopify` `slack` `saic`
`spacex` `spotify` `stepfun` `stripe` `suning` `taobao` `teambition` `tesla` `tiangong`
`toutiao` `unionpay` `vercel` `vipshop` `weibo` `wechat` `weilai-fin` `wps` `xiaohongshu`
`xiaomi-dev` `xpeng` `yida` `youku` `yuque` `yuanbao` `zhihu` `zhongxin` `zhipu`
