# Unity ML-Agents Toolkit

[![docs badge](https://img.shields.io/badge/docs-reference-blue.svg)](https://github.com/Unity-Technologies/ml-agents/tree/release_20_docs/docs/)

[![license badge](https://img.shields.io/badge/license-Apache--2.0-green.svg)](../LICENSE.md)

([latest release](https://github.com/Unity-Technologies/ml-agents/releases/tag/latest_release))
([all releases](https://github.com/Unity-Technologies/ml-agents/releases))

**Unity Machine Learning Agents Toolkit** (ML-Agents)是一个开源软件
项目，使游戏和模拟作为环境训练智能代理。我们提供实现(基于PyTorch)最先进的算法，使游戏开发者和爱好者轻松为2D、3D和VR/AR游戏训练智能代理。研究人员也可以使用提供了简单易用的Python API来使用强化学习训练agent，模仿学习，神经进化或其他方法。这些训练有素的特工可以用于多种目的，包括控制NPC行为设置，如多代理和对抗性)，自动测试游戏构建在发行前评估不同的游戏设计决策。的ML-Agents工具包对游戏开发者和AI研究人员都是互惠互利的提供了一个中央平台，可以在Unity上评估人工智能的进步然后制作了丰富的环境，便于更广泛的研究和游戏开发者社区。

## Features
- 17+ [示例 Unity 环境](Learning-Environment-Examples.md)
- 支持多种环境配置和训练场景
- 灵活的 Unity SDK，可以集成到您的游戏或自定义 Unity 场景中
- 支持通过多种深度强化学习算法（PPO、SAC、MA-POCA、self-play）训练单代理、多代理合作和多代理竞争场景。
- 支持通过两种模仿学习算法（BC 和 GAIL）从演示中学习。
- 快速轻松地添加您自己的 [自定义训练算法](Python-Custom-Trainer-Plugin.md) 或组件.
- 针对复杂任务轻松定义的课程学习场景
- 使用环境随机化训练健壮的代理
- 通过按需决策制定灵活的代理控制
- 使用多个并发 Unity 环境实例进行训练
- 利用 Unity 推理引擎(Unity-Inference-Engine.md) 提供原生跨平台支持
- Unity环境 [Python控制](Python-LLAPI.md)
- 利用 Unity推理引擎 [gym](Python-Gym-API.md) 提供原生跨平台支持
- 将 Unity 学习环境包装为 [PettingZoo](Python-PettingZoo-API.md) 环境

有关所有这些功能的详细说明，请参阅我们的[ML-Agents](ML-Agents-Overview.md) 概述页面
或者直接访问我们的[网络文档] (https://unity-technologies.github.io/ml-agents/).
## 发布和文档

**Our latest, stable release is `Release 20`. Click
[here](Getting-Started.md)
to get started with the latest release of ML-Agents.**

**您还可以查看我们的新[网络文档](https://unity-technologies.github.io/ml-agents/)!**

下表列出了我们所有的版本，包括我们正在积极开发并且可能不稳定的主要`main`分支。 一些有用的指南：
- [Versioning page 版本控制](Versioning.md) 页面概述了我们如何管理我们的 GitHub 版本以及每个 ML-Agents 组件的版本控制过程。
- [Releases page 版本页面](https://github.com/Unity-Technologies/ml-agents/releases)
  版本页面包含版本之间更改的详细信息。
- [Migration page 迁移页面](Migrating.md) 包含有关如何从早期版本的 ML-Agents 工具包升级的详细信息。
- 下表中的文档链接包括特定于每个版本的安装和使用说明。 请记住始终使用与您正在使用的发行版本相对应的文档。
- `com.unity.ml-agents` 包已针对 Unity 2020.1 及更高版本进行[verified 验证](https://docs.unity3d.com/2020.1/Documentation/Manual/pack-safe.html)。 已验证的软件包版本编号为 1.0.x

| **Version** | **Release Date** | **Source** | **Documentation** | **Download** | **Python Package** | **Unity Package** |
|:-------:|:------:|:-------------:|:-------:|:------------:|:------------:|:------------:|
| **Release 20** | **November 21, 2022** | **[source](https://github.com/Unity-Technologies/ml-agents/tree/release_20)** | **[docs](https://github.com/Unity-Technologies/ml-agents/tree/release_20_docs/docs/Readme.md)** | **[download](https://github.com/Unity-Technologies/ml-agents/archive/release_20.zip)** | **[0.30.0](https://pypi.org/project/mlagents/0.30.0/)** | **[2.3.0](https://docs.unity3d.com/Packages/com.unity.ml-agents@2.3/manual/index.html)** |
| **main (unstable)** | -- | [source](https://github.com/Unity-Technologies/ml-agents/tree/main) | [docs](https://github.com/Unity-Technologies/ml-agents/tree/main/docs/Readme.md) | [download](https://github.com/Unity-Technologies/ml-agents/archive/main.zip) | -- | -- |
| **Verified Package 1.0.8** | **May 26, 2021** | **[source](https://github.com/Unity-Technologies/ml-agents/tree/com.unity.ml-agents_1.0.8)** | **[docs](https://github.com/Unity-Technologies/ml-agents/blob/release_20_verified_docs/docs/Readme.md)** | **[download](https://github.com/Unity-Technologies/ml-agents/archive/com.unity.ml-agents_1.0.8.zip)** | **[0.16.1](https://pypi.org/project/mlagents/0.16.1/)** | **[1.0.8](https://docs.unity3d.com/Packages/com.unity.ml-agents@1.0/manual/index.html)** |

如果您是一名研究人员，对将 Unity 作为 AI 平台进行讨论感兴趣，请参阅我们关于。
[ Unity 和 ML-Agents 工具包的参考论文的预印本](https://arxiv.org/abs/1809.02627).

如果您使用 Unity 或 ML-Agents Toolkit 进行研究，我们要求您引用以下论文作为参考:

```
@article{juliani2020,
  title={Unity: A general platform for intelligent agents},
  author={Juliani, Arthur and Berges, Vincent-Pierre and Teng, Ervin and Cohen, Andrew and Harper, Jonathan and Elion, Chris and Goy, Chris and Gao, Yuan and Henry, Hunter and Mattar, Marwan and Lange, Danny},
  journal={arXiv preprint arXiv:1809.02627},
  year={2020}
}
```

此外，如果您在研究中使用 MA-POCA 训练器，我们要求您引用以下论文作为参考:

```
@article{cohen2022,
  title={On the Use and Misuse of Abosrbing States in Multi-agent Reinforcement Learning},
  author={Cohen, Andrew and Teng, Ervin and Berges, Vincent-Pierre and Dong, Ruo-Ping and Henry, Hunter and Mattar, Marwan and Zook, Alexander and Ganguly, Sujoy},
  journal={RL in Games Workshop AAAI 2022},
  year={2022}
}
```



## Additional Resources 额外资源

我们有一个 Unity Learn 课程,
[ML-Agents: Hummingbirds](https://learn.unity.com/course/ml-agents-hummingbirds),
它提供了对 Unity 和 ML-Agents Toolkit的简单介绍.

我们还与Youtuber
[CodeMonkeyUnity](https://www.youtube.com/c/CodeMonkeyUnity) 合作创建了
[一系列的视频教程](https://www.youtube.com/playlist?list=PLzDRvYVwl53vehwiN_odYJkPBzcqFw110)
介绍如何实施和使用 ML-Agents Toolkit。

我们还发布了一系列与 ML-Agents 相关的博文：

- (July 12, 2021)
  [ML-Agents plays Dodgeball ML-Agents 玩躲避球](https://blog.unity.com/technology/ml-agents-plays-dodgeball)
- (May 5, 2021)
  [ML-Agents v2.0 发布：现在支持训练复杂的合作行为](https://blogs.unity3d.com/2021/05/05/ml-agents-v2-0-release-now-supports-training-complex-cooperative-behaviors/)
- (December 28, 2020)
  [Unity ML-Agents 团队祝您节日快乐！](https://blogs.unity3d.com/2020/12/28/happy-holidays-from-the-unity-ml-agents-team/)
- (November 20, 2020)
  [Eidos-Montréal 如何创建网格传感器来改进训练代理的观察](https://blogs.unity3d.com/2020/11/20/how-eidos-montreal-created-grid-sensors-to-improve-observations-for-training-agents/)
- (November 11, 2020)
  [2020 AI@Unity 实习生大喊大叫](https://blogs.unity3d.com/2020/11/11/2020-aiunity-interns-shoutout/)
- (May 12, 2020)
  [宣布推出 ML-Agents Unity Package v1.0！](https://blogs.unity3d.com/2020/05/12/announcing-ml-agents-unity-package-v1-0/)
- (February 28, 2020)
  [使用 ML-Agents 自我对弈训练智能对手](https://blogs.unity3d.com/2020/02/28/training-intelligent-adversaries-using-self-play-with-ml-agents/)
- (November 11, 2019)
  [使用 ML-Agents 将您的代理训练速度提高 7 倍](https://blogs.unity3d.com/2019/11/11/training-your-agents-7-times-faster-with-ml-agents/)
- (October 21, 2019)
  [AI@Unity 实习生帮助塑造世界](https://blogs.unity3d.com/2019/10/21/the-aiunity-interns-help-shape-the-world/)
- (April 15, 2019)
  [Unity ML-Agents Toolkit v0.8：更快地训练真实游戏](https://blogs.unity3d.com/2019/04/15/unity-ml-agents-toolkit-v0-8-faster-training-on-real-games/)
- (March 1, 2019)
  [Unity ML-Agents Toolkit v0.7：迈向跨平台推理的飞跃](https://blogs.unity3d.com/2019/03/01/unity-ml-agents-toolkit-v0-7-a-leap-towards-cross-platform-inference/)
- (December 17, 2018)
  [ML-Agents Toolkit v0.6：改进大脑和模仿学习的可用性](https://blogs.unity3d.com/2018/12/17/ml-agents-toolkit-v0-6-improved-usability-of-brains-and-imitation-learning/)
- (October 2, 2018)
  [Puppo, The Corgi：使用 Unity ML-Agents 工具包的可爱超载](https://blogs.unity3d.com/2018/10/02/puppo-the-corgi-cuteness-overload-with-the-unity-ml-agents-toolkit/)
- (September 11, 2018)
  [ML-Agents Toolkit v0.5，面向 AI 研究人员的新资源现已推出](https://blogs.unity3d.com/2018/09/11/ml-agents-toolkit-v0-5-new-resources-for-ai-researchers-available-now/)
- (June 26, 2018)
  [用好奇心解决稀疏奖励任务](https://blogs.unity3d.com/2018/06/26/solving-sparse-reward-tasks-with-curiosity/)
- (June 19, 2018)
  [Unity ML-Agents Toolkit v0.4 和 Udacity 深度强化学习纳米学位](https://blogs.unity3d.com/2018/06/19/unity-ml-agents-toolkit-v0-4-and-udacity-deep-reinforcement-learning-nanodegree/)
- (May 24, 2018)
  [Unity 中的模仿学习：工作流程](https://blogs.unity3d.com/2018/05/24/imitation-learning-in-unity-the-workflow/)
- (March 15, 2018)
  [ML-Agents Toolkit v0.3 Beta 发布：模仿学习、反馈驱动功能等](https://blogs.unity3d.com/2018/03/15/ml-agents-v0-3-beta-released-imitation-learning-feedback-driven-features-and-more/)
- (December 11, 2017)
  [在真实游戏中使用机器学习代理：新手指南](https://blogs.unity3d.com/2017/12/11/using-machine-learning-agents-in-a-real-game-a-beginners-guide/)
- (December 8, 2017)
  [介绍 ML-Agents 工具包 v0.2：课程学习、新环境等](https://blogs.unity3d.com/2017/12/08/introducing-ml-agents-v0-2-curriculum-learning-new-environments-and-more/)
- (September 19, 2017)
  [介绍：Unity 机器学习代理工具包](https://blogs.unity3d.com/2017/09/19/introducing-unity-machine-learning-agents/)
- Overviewing reinforcement learning concepts
  ([多臂强盗](https://blogs.unity3d.com/2017/06/26/unity-ai-themed-blog-entries/)
  and
  [Q-learning](https://blogs.unity3d.com/2017/08/22/unity-ai-reinforcement-learning-with-q-learning/))

### More from Unity

- [Unity Robotics](https://github.com/Unity-Technologies/Unity-Robotics-Hub)
- [Unity Computer Vision](https://github.com/Unity-Technologies/com.unity.perception)

## Community and Feedback

ML-Agents 工具包是一个开源项目，我们鼓励并欢迎贡献。 如果您想做出贡献，请务必查看我们的
[贡献指南](CONTRIBUTING.md) and
[行为守则](../CODE_OF_CONDUCT.md).

For problems with the installation and setup of the ML-Agents Toolkit, or
discussions about how to best setup or train your agents, please create a new
thread on the
[Unity ML-Agents forum](https://forum.unity.com/forums/ml-agents.453/) and make
sure to include as much detail as possible. If you run into any other problems
using the ML-Agents Toolkit or have a specific feature request, please
[submit a GitHub issue](https://github.com/Unity-Technologies/ml-agents/issues).

Please tell us which samples you would like to see shipped with the ML-Agents Unity
package by replying to
[this forum thread](https://forum.unity.com/threads/feedback-wanted-shipping-sample-s-with-the-ml-agents-package.1073468/).


Your opinion matters a great deal to us. Only by hearing your thoughts on the
Unity ML-Agents Toolkit can we continue to improve and grow. Please take a few
minutes to
[let us know about it](https://unitysoftware.co1.qualtrics.com/jfe/form/SV_55pQKCZ578t0kbc).

For any other questions or feedback, connect directly with the ML-Agents team at
ml-agents@unity3d.com.

## Privacy

In order to improve the developer experience for Unity ML-Agents Toolkit, we have added in-editor analytics.
Please refer to "Information that is passively collected by Unity" in the
[Unity Privacy Policy](https://unity3d.com/legal/privacy-policy).
