# synthetic_data_quality_pattern_locate

**用规则在大模型推理优化工程师·合成数据的质量分水岭里定位可疑位置。**

`synthetic_data_quality_pattern_locate` —— 用一组明示的正则规则扫描输入，报告大模型推理优化工程师·合成数据的质量分水岭相关的命中行与片段

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`synthetic_data_quality_pattern_locate.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**阶跃星辰 · 初级大模型推理优化工程师**
- 技能主线：Python、C++、CUDA、vLLM、TensorRT
- 领域标签：大模型推理、AI基础设施
- 研究方向：大模型推理优化工程师·合成数据的质量分水岭

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install rahulsamy-synthetic_data_quality_pattern_locate
```

装完直接用命令名调用：

```bash
synthetic_data_quality_pattern_locate --help
```

也可以不用安装，直接把 `synthetic_data_quality_pattern_locate.py` 拷走用——它只依赖标准库。

## 为什么需要它

规则表公开可读，每条命中都能对应到一条明示的规则

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python synthetic_data_quality_pattern_locate.py --file input.txt
python synthetic_data_quality_pattern_locate.py --text "示例内容"
python synthetic_data_quality_pattern_locate.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 正则匹配会有漏报与误报——它是筛子，不是裁判。
- 不提供修复方案，也不重写内容。

## 跑测试

```bash
python test_synthetic_data_quality_pattern_locate.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/rahulsamy/synthetic_data_quality_pattern_locate>

---

## 关于作者

rahulsamy 做大模型推理优化工程师·合成数据的质量分水岭相关的问题，方向对标阶跃星辰的初级大模型推理优化工程师岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://rahulsamy.github.io>
- 仓库：<https://github.com/rahulsamy/synthetic_data_quality_pattern_locate>

## 许可

MIT，见 [LICENSE](LICENSE)。
