实验报告：开源软件应用与开发（Famous Repos Tour）

Lab Report: Open Source Software Application and Development (Famous Repos Tour)

· 姓名/学号 / Name/Student ID: WANGYUFAN 24144632  
· 日期 / Date: 2026年5月15日 / May 15, 2026

---

任务 1：克隆 — 用 Git 克隆 Git 本身  

Task 1: Clone – Cloning Git with Git

1. 总提交数 (Total commit count)： 80749
2. 首次提交的日期和作者 (First commit date and author):
   · 作者 (Author): Linus Torvalds
   · 日期 (Date): Thu Apr 7 15:13:13 2005 -0700
3. 最初 5 个 commit 记录 (First 5 commits):
   ```text
   e83c516331 Initial revision of "git", the information manager from hell
   8bc9a0c769 Add copyright notices.
   e497ea2a9b Make read-tree actually unpack the whole tree.
   bf0c6e839c Make "cat-file" output the file contents to stdout.
   19b2860cba Use "-Wall -O2" for the compiler to get more warnings.
   ```

---

任务 2：开源名著探索 — Linux 内核历史

Task 2: Exploring an Open Source Classic – Linux Kernel History

1. TOP 10 贡献者姓名 / TOP 10 contributors:
      由于在克隆时使用了 --depth=1（浅克隆）参数，本地仓库只下载并保留了历史记录中的最后一次提交。因此，运行 git shortlog -sn 只输出了最新提交的作者：1 Linus Torvalds。  
      English: Because the --depth=1 (shallow clone) parameter was used during cloning, the local repository only downloaded and retained the last commit in the history. Therefore, running git shortlog -sn only output the author of the latest commit: 1 Linus Torvalds.
2. 3 个最有趣的文件夹及原因 / 3 most interesting folders and reasons:
   · crypto/：包含了内核中所有的密码学和加密算法实现（如 AES、SHA 等），涉及极其硬核的安全底层逻辑。  
          English: crypto/: Contains all cryptographic and encryption algorithm implementations in the kernel (such as AES, SHA, etc.), dealing with extremely hardcore low-level security logic.
   · drivers/：整个内核中体积最大的文件夹，包含了支持全球成千上万种硬件设备的底层驱动程序，是开源生态繁荣的基石。  
          English: drivers/: The largest folder in the entire kernel, containing low-level drivers that support thousands of hardware devices worldwide, serving as the cornerstone of a thriving open source ecosystem.  
   · fs/：文件系统（File System）目录，里面实现了 ext4、sysfs、fat 等各种熟悉和不安全的存储格式的读写逻辑，对系统性能至关重要。  
          English: fs/: The File System directory, implementing read/write logic for various familiar and less secure storage formats such as ext4, sysfs, fat, which is critical to system performance.  
3. MAINTAINERS 文件中喜欢的一行 / A line I like from the MAINTAINERS file:
   · 选取的行 / Selected line: M: Linus Torvalds <torvalds@linux-foundation.org>
   · 原因 / Reason: 这是 Linux 之父、开源界传奇人物 Linus 本人的官方维护者邮箱。在代码文件里亲眼看到这一行，有一种直接触碰到计算机开源历史源头的震撼感。  
          English: This is the official maintainer email of Linus Torvalds, the father of Linux and a legend in the open source world. Seeing this line in the source code file gives a thrilling sense of directly touching the origin of computer open source history.

---

任务 3：自己领域的著名仓库选择  

Task 3: Selecting a Famous Repository in My Field

1. 仓库名称及选择理由 / Repository name and reason for selection:
   · 仓库 (Repository): scikit-learn/scikit-learn
   · 理由 (Reason): 这是一个在机器学习和数据科学领域极其重要且经典的开源算法库，代码规范非常值得学习。  
          English: This is an extremely important and classic open-source algorithm library in the field of machine learning and data science, and its code standards are well worth learning.
2. 最近一个月的活动量 (Commits) / Activity in the last month (Commits): 114
3. 4.4 节的 8 项健康度清单评分 / Score on the 8-item health checklist (Section 4.4):
   · 评分：8/8（非常健康）。该仓库拥有完善的 README 和 CONTRIBUTING 文档，最近一个月有大量 Commit 和活跃的 PR，Issues 有明确的标签管理，并且配备了完善的 CI/CD 自动化测试。  
        English: Score: 8/8 (very healthy). The repository has comprehensive README and CONTRIBUTING documentation, a large number of commits and active PRs in the last month, issues are well managed with labels, and it is equipped with thorough CI/CD automated testing.

---

任务 4：一人的足迹跟踪（贡献者分析）

Task 4: Tracking One Person's Footprints (Contributor Analysis)

1. 选定的贡献者 / Selected contributor: Olivier Grisel (scikit-learn 的核心开发者之一 / one of the core developers of scikit-learn)
2. 该贡献者的提交次数 / Number of commits by this contributor: 2573
3. 最让人印象深刻的一条 commit message / The most impressive commit message:
   · 38542048c2 DOC Financial supporters (#33704)
4. 他主要修改的文件/文件夹 / Main files/folders modified:
      他主要活跃在 sklearn/ 核心算法模块以及 build_tools/ 和持续集成相关的配置文件中，对项目的底层架构贡献巨大。  
      English: He is mainly active in the sklearn/ core algorithm module as well as build_tools/ and continuous integration related configuration files, making significant contributions to the underlying architecture of the project.

---

任务 5：公关宣传（寻找 Good First Issue）

Task 5: Public Relations – Finding a Good First Issue

1. 挑战的实例 / Example of a challenge: 在 scikit-learn 仓库中带有 good first issue 标签的文档修复或基础代码重构问题。  
      English: A documentation fix or basic code refactoring issue labeled good first issue in the scikit-learn repository.
2. 所需的技术栈 / Required tech stack: Python 基础语法、基本的机器学习概念、Git 版本控制以及 pytest 测试框架。  
      English: Basic Python syntax, fundamental machine learning concepts, Git version control, and the pytest testing framework.
3. CONTRIBUTING.md 总结（用 3 句话总结）/ CONTRIBUTING.md summary (in 3 sentences):
   1. 在开始编写代码前，必须先阅读开发指南并在本地配置好隔离的开发环境（如 conda/venv）。  
            English: Before starting to write code, you must read the development guide and set up an isolated development environment locally (e.g., conda/venv).
   2. 任何新增加或修改的功能代码，都必须附带相应的单元测试（Unit Tests）以保证代码覆盖率。  
            English: Any newly added or modified feature code must be accompanied by corresponding unit tests to ensure code coverage.
   3. 提交 PR 时，代码风格必须通过 flake8/black 的检查，并且 Commit 信息需要遵循约定的清晰格式。  
            English: When submitting a PR, the code style must pass flake8/black checks, and the commit messages need to follow an agreed clear format.
