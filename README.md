# 如何做个程序员：社区版
Robert L. Read 和 社区

Copyright 2002, 2003, 2016 Robert L. Read

基于 [署名-相同方式共享 4.0 国际 (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/deed.zh)

## 介绍
成为一名好的程序员是困难而卓越的。在实现一个软件项目的集体愿景中，最难的部分是和同事以及顾客打交道（译注：什么鬼...）。编写计算机程序很重要，而且需要极高的智力和技巧。But it is really child's play compared to everything else that a good programmer must do to make a software system that succeeds for both the customer and myriad colleagues for whom she is partially responsible. 在本文中我将尝试尽可能简练地总结出当我在21岁时希望有人能够解释给我听的一些东西。

本文将会非常主观，所以它将注定带有个人观点而且有些武断。在这里我只讨论一个程序员在他/她的工作中很容易遇到的问题。很多这样的问题以及它们的解决方案对人们来说是很普通的，所以我可能会有点唠叨。尽管这样，我希望这篇文章会对你有用。

在课程中可以习得计算机编程。The Pragmatic Programmer [Prag99], Code Complete [CodeC93], Rapid Development [RDev96], 以及 Extreme Programming Explained [XP99]，这些很棒的书都会教你计算机编程知识以及很多如何成为一名好的程序员的问题。在读本文之前或者读的过程中，你也应该读一下 Paul Graham [PGSite] 和 Eric Raymond [Hacker] 的文章。本文和这些优秀的作品不同，会着重强调社会问题以及全面地总结我所了解到的整个必需的技能集的内容。

在这篇文章中，「老板」这个词将指那个把项目交给你去做的人。我会将「生意」(business)，「公司」(company) 和「部落」(tribe) 这几个词作为同义词使用，不过，「生意」意味着赚钱，「公司」意味着现代的工作环境，而「部落」通常指一群和你忠于彼此的人。

欢迎来到部落。

## 目录

1. [入门](1-Beginner)
    - 个人技巧
		- [学习 Debug](1-Beginner/Personal-Skills/01-Learn To Debug.md)
		- [如果通过切分问题空间来 Debug](1-Beginner/Personal-Skills/02-How to Debug by Splitting the Problem Space.md)
		- [如何去掉一个错误](1-Beginner/Personal-Skills/03-How to Remove an Error.md)
		- [如何利用日志来 Debug](1-Beginner/Personal-Skills/04-How to Debug Using a Log.md)
		- [如何理解性能问题](1-Beginner/Personal-Skills/05-How to Understand Performance Problems.md)
		- [如何修复性能问题](1-Beginner/Personal-Skills/06-How to Fix Performance Problems.md)
		- [如何优化循环](1-Beginner/Personal-Skills/07-How to Optimize Loops.md)
		- [如何处理 I/O 花费](1-Beginner/Personal-Skills/08-How to Deal with IO Expense.md)
		- [如何管理内存](1-Beginner/Personal-Skills/09-How to Manage Memory.md)
		- [如何处理时不时，断断续续出现的 Bug](1-Beginner/Personal-Skills/10-How to Deal with Intermittent Bugs.md)
		- [如何学习设计技巧](1-Beginner/Personal-Skills/11-How to Learn Design Skills.md)
		- [如何进行实验](1-Beginner/Personal-Skills/12-How to Conduct Experiments.md)
    - 团队技巧
		- [为什么估算很重要](1-Beginner/Team-Skills/01-Why Estimation is Important.md)
		- [如何估算编程时间](1-Beginner/Team-Skills/02-How to Estimate Programming Time.md)
		- [如何寻找信息](1-Beginner/Team-Skills/03-How to Find Out Information.md)
		- [如何利用他人作为信息来源](1-Beginner/Team-Skills/04-How to Utilize People as Information Sources.md)
		- [如何聪明地编写文档](1-Beginner/Team-Skills/05-How to Document Wisely.md)
		- [如何与糟糕的代码相处](1-Beginner/Team-Skills/06-How to Work with Poor Code.md)
		- [如何使用源代码控制工具](1-Beginner/Team-Skills/07-How to Use Source Code Control.md)
		- [如何进行单元测试](1-Beginner/Team-Skills/08-How to Unit Test.md)
		- [在卡住时停下来休息一下](1-Beginner/Team-Skills/09-Take Breaks when Stumped.md)
		- [怎样确认回家的时间](1-Beginner/Team-Skills/10-How to Recognize When to Go Home.md)
		- [如何与难缠的人打交道](1-Beginner/Team-Skills/11-How to Deal with Difficult People.md)
2. [中级](2-Intermediate)
    - 个人技巧
		- [如何保持积极性](2-Intermediate/Personal-Skills/01-How to Stay Motivated.md)
		- [如何被广泛地信任](2-Intermediate/Personal-Skills/02-How to be Widely Trusted.md)
		- [如何权衡时间和空间](2-Intermediate/Personal-Skills/03-How to Tradeoff Time vs Space.md)
		- [如何进行压力测试](2-Intermediate/Personal-Skills/04-How to Stress Test.md)
		- [如何平衡简洁和抽象](2-Intermediate/Personal-Skills/05-How to Balance Brevity and Abstraction.md)
		- [如何学习新的技术](2-Intermediate/Personal-Skills/06-How to Learn New Skills.md)
		- [学习打字](2-Intermediate/Personal-Skills/07-Learn to Type.md)
		- [如何做集成测试](2-Intermediate/Personal-Skills/08-How to Do Integration Testing.md)
		- [沟通的语言](2-Intermediate/Personal-Skills/09-Communication Languages.md)
		- [重型工具](2-Intermediate/Personal-Skills/10-Heavy Tools.md)
		- [如何分析数据](2-Intermediate/Personal-Skills/11-How to analyze data.md)
    - 团队技巧
		- [如何管理开发时间](2-Intermediate/Team-Skills/01-How to Manage Development Time.md)
		- [如何管理第三方软件的风险](2-Intermediate/Team-Skills/02-How to Manage Third-Party Software Risks.md)
		- [如何管理(技术)顾问](2-Intermediate/Team-Skills/03-How to Manage Consultants.md)
		- [如何和对的人交流](2-Intermediate/Team-Skills/04-How to Communicate the Right Amount.md)
		- [如何诚实地表达不同意同时不受惩罚](2-Intermediate/Team-Skills/05-How to Disagree Honestly and Get Away with It.md)
    - 判断
		- [如何权衡质量和开发时间](2-Intermediate/Judgment/01-How to Tradeoff Quality Against Development Time.md)
		- [如何管理软件系统的依赖](2-Intermediate/Judgment/02-How to Manage Software System Dependence.md)
		- [如何判断软件是否过于未成熟](2-Intermediate/Judgment/03-How to Decide if Software is Too Immature.md)
		- [如何做一个「买还是自己做」的决定](2-Intermediate/Judgment/04-How to Make a Buy vs Build Decision.md)
		- [如何专业地成长](2-Intermediate/Judgment/05-How to Grow Professionally.md)
		- [如何对面试者进行评估](2-Intermediate/Judgment/06-How to Evaluate Interviewees.md)
		- [如何知道什么时候来应用炫酷的计算机科学](2-Intermediate/Judgment/07-How to Know When to Apply Fancy Computer Science.md)
		- [如何与非工程师聊天](2-Intermediate/Judgment/08-How to Talk to Non-Engineers.md)
3. [进阶](3-Advanced)
    - 技术判断
        - [如何从「不可能」的事情中判别出「难」的事情](3-Advanced/Technical-Judgment/01-How to Tell the Hard From the Impossible.md)
        - [如何使用嵌套的语言](3-Advanced/Technical-Judgment/02-How to Utilize Embedded Languages.md)
        - [选择开发语言](3-Advanced/Technical-Judgment/03-Choosing Languages.md)
    - 理智地妥协
        - [如何与进度表的压力做斗争](3-Advanced/Compromising-Wisely/01-How to Fight Schedule Pressure.md)
        - [如何理解用户](3-Advanced/Compromising-Wisely/02-How to Understand the User.md)
        - [如何获得升职](3-Advanced/Compromising-Wisely/03-How to Get a Promotion.md)
    - 服务你的团队
        - [如何开发出(团队的)天赋](3-Advanced/Serving-Your-Team/01-How to Develop Talent.md)
        - [如何选择在哪个方向上工作](3-Advanced/Serving-Your-Team/02-How to Choose What to Work On.md)
        - [如何最大限度地利用你的队友](3-Advanced/Serving-Your-Team/03-How to Get the Most From Your Teammates.md)
        - [如何分割问题](3-Advanced/Serving-Your-Team/04-How to Divide Problems Up.md)
        - [如何处理无聊的任务](3-Advanced/Serving-Your-Team/05-How to Handle Boring Tasks.md)
        - [如何为一个项目获取支持](3-Advanced/Serving-Your-Team/06-How to Gather Support for a Project.md)
        - [如何发展一个系统](3-Advanced/Serving-Your-Team/07-How to Grow a System.md)
        - [如何进行良好的沟通](3-Advanced/Serving-Your-Team/08-How to Communicate Well.md)
        - [如何告诉别人他们不想听到的事情](3-Advanced/Serving-Your-Team/09-How to Tell People Things They Don't Want to Hear.md)
        - [如何应对「管理神话」](3-Advanced/Serving-Your-Team/10-How to Deal with Managerial Myths.md)
        - [如何应对组织上的混乱](3-Advanced/Serving-Your-Team/11-How to Deal with Organizational Chaos.md)
4. [术语表](4-Glossary.md)
5. [附录 A - 自传/网站自我介绍](5-Bibliography.md)
6. [附录 B - 历史 (至 2016 年 1 月)](6-History.md)
6. [附录 C - 贡献 (至 2016 年 1 月)](7-Contributions.md)


<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">如何做个程序员：社区版</span> by <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Robert L. Read with Community</span> 是基于 <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">署名-相同方式共享 4.0 国际 (CC BY-SA 4.0)</a> 协议的。
