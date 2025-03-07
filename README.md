
虎鹤-万象是一个基于万象方案改造而来的rime输入方案。
它可以实现虎码与小鹤双拼等多种双拼和全拼的混合输入。
虎码置顶，可分别使用开关关闭虎单、虎词和虎码整句，不与音码冲突。
可互相通过拆分滤镜和拼音滤镜开关无障碍反查。
它的基础 万象方案是一个可在wanxiang.schema.yaml文件更换多种音码：全拼、自然码、自然龙、小鹤双拼、搜狗双拼、微软双拼；
和多种辅助码 墨奇、鹤形、自然码、简单鹤、仓颉首末、虎码首末、五笔前2、汉心码的音码方案，
内置强大词库与模型，整句输入有很高的的正确率。
总的来说这个方案结合了形码单字的高正确率、音码整句的高正确率且不用考虑拆字的优势、开启虎词时的更短码长，和开启虎码整句时的综合优势。
适配了多种形码(除了拆分滤镜)，放在了群文件，包括86 98 新世纪 092 郑码 徐码 天码 真码 蓝宝石，使用这些形码时可把对应的txt文件放进custom_phrase文件夹，将wanxiang.schema.yaml文件末尾custom_phrase里user_dict的tiger改成你的形码字典文件名（并注释掉上面tiger_sentence的dictionary）


混输交流群 809597773
注：基于万象方案改造，万象方案地址https://github.com/amzxyz/rime_wanxiang_pinyin
将它复制到万象方案内即可运行，群文件有合并完成的压缩包
相对于万象的改动有:
1.开关
2.增加4个滤镜：tiger、拆分、拼音、常用字
3.修改了1个引导前缀：ach
4.custom_phrase相关
5.tiger_sentence相关


更新日志:
3.5.21更新：将句词单的输出顺序调整为单词句、将快符ov\划为符号组、跟随万象更新
3.1.21更新：将一简词的的输出顺序放在了一简字之后
2.28.4更新：
改造整句词典，为两码整句添加了加码纠错能力、优化了两码句/原码句开关，解决了相同码长时切换首选无效的问题、新增了一简词开关、跟随万象更新
2.24.7更新：
改良整句词典实现两码整句，与含有常规字词的原码整句共存，根据开关状态决定排序、
缩减常用字过滤字集为8105、
跟随万象更新
2.23.4更新：因为万象原本的字符集过滤lua不过滤句中生僻字，为了避免对虎码整句的影响，换成了core2022
2.23.2更新：为虎词添加了简词、相对调低了24个同权重码词条权重、分离了虎码整句，为整句词典添加了二码单字、更随万象更新
2.22.2更新：更换 custom_phrase/user_dict的txt为custom_phrase/dictionary的dict.yaml，解决了txt无法根据同权重词条上下顺序排序的问题、删除了两个ox快符、更随万象今晚更新
2.20.18更新：解决了某些候选字错误的被归类为符号组的问题
2.20.4更新：修复了加入虎码整句后 虎单虎词异常置顶 不让位于双拼词的问题
2.19.24更新：修复了加入虎码整句后 无法使用符号上屏的问题
2.19.23更新：新增了虎码整句功能
2.18.23更新：将虎单、虎词开关同时开启时 虎词的顺序放在了虎单之前
2.18.21更新：将其它形码单字词典加了词，从方案移到了群文件、更随万象更新
2.18.14更新：继续简化了lua逻辑、更随万象更新
2.17.23更新：解决了快符被开关关闭的问题，简化了lua逻辑
2.17.21更新：调整了滤镜顺序，更随万象今日更新
2.17.1更新：新增了置顶组句开关、更随万象更新
2.16.15更新，默认开启了音码调频，略微调整了快符，简化了custom.yaml，更随万象今日更新
2.14.15更新，新增了虎词和虎词开关
