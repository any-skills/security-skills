# CWE-699: 软件开发（Software Development）

> **来源**: [https://cwe.mitre.org/data/definitions/699.html](https://cwe.mitre.org/data/definitions/699.html)
> **版本**: CWE 4.19.1
> **类型**: 视图（View）

## 概述

此视图围绕软件开发中常见的概念来组织弱点分类。涵盖软件开发生命周期的各个方面，包括架构和实现。因此，此视图可以与架构师、开发人员、教育工作者和评估供应商的视角紧密对齐。它提供了多种类别，旨在简化导航、浏览和映射。

## 目标受众

| 受众 | 说明 |
|------|------|
| **软件开发人员** | 软件开发人员（包括架构师、设计人员、编码人员和测试人员）使用此视图来更好地理解在其软件应用程序的特定领域中可能犯的错误。使用开发人员熟悉的概念使得此视图更易于导航，并且通过引入模式进行过滤可以聚焦于开发生命周期的特定阶段。 |
| **教育工作者** | 教育工作者使用此视图向未来的开发人员讲授代码库特定部分中常见的错误类型。 |

---

## 分类目录

### 1. CWE-1228: API / 函数错误

与内置函数或外部API使用相关的弱点。

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-242 | 使用本质上危险的函数 | Use of Inherently Dangerous Function |
| CWE-474 | 使用具有不一致实现的函数 | Use of Function with Inconsistent Implementations |
| CWE-475 | API输入的未定义行为 | Undefined Behavior for Input to API |
| CWE-477 | 使用过时的函数 | Use of Obsolete Function |
| CWE-676 | 使用潜在危险的函数 | Use of Potentially Dangerous Function |
| CWE-695 | 使用低级功能 | Use of Low-Level Functionality |
| CWE-749 | 暴露危险的方法或函数 | Exposed Dangerous Method or Function |

---

### 2. CWE-1210: 审计 / 日志错误

与系统审计组件相关的弱点，通常涉及记录用户活动以识别非预期访问和修改。

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-117 | 日志的不当输出中和 | Improper Output Neutralization for Logs |
| CWE-222 | 安全相关信息的截断 | Truncation of Security-relevant Information |
| CWE-223 | 安全相关信息的遗漏 | Omission of Security-relevant Information |
| CWE-224 | 用替代名称混淆安全相关信息 | Obscured Security-relevant Information by Alternate Name |
| CWE-778 | 日志记录不足 | Insufficient Logging |
| CWE-779 | 记录过多数据 | Logging of Excessive Data |

---

### 3. CWE-1211: 认证错误

与系统认证组件相关的弱点，通常涉及验证实体是否确实是其声称的身份。

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-289 | 通过替代名称绕过认证 | Authentication Bypass by Alternate Name |
| CWE-290 | 通过欺骗绕过认证 | Authentication Bypass by Spoofing |
| CWE-294 | 通过捕获重放绕过认证 | Authentication Bypass by Capture-replay |
| CWE-295 | 不正确的证书验证 | Improper Certificate Validation |
| CWE-301 | 认证协议中的反射攻击 | Reflection Attack in an Authentication Protocol |
| CWE-303 | 认证算法的错误实现 | Incorrect Implementation of Authentication Algorithm |
| CWE-305 | 由主要弱点导致的认证绕过 | Authentication Bypass by Primary Weakness |
| CWE-306 | 关键功能缺少认证 | Missing Authentication for Critical Function |
| CWE-307 | 过度认证尝试的不当限制 | Improper Restriction of Excessive Authentication Attempts |
| CWE-308 | 使用单因素认证 | Use of Single-factor Authentication |
| CWE-309 | 使用密码系统作为主要认证 | Use of Password System for Primary Authentication |
| CWE-322 | 没有实体认证的密钥交换 | Key Exchange without Entity Authentication |
| CWE-603 | 使用客户端认证 | Use of Client-Side Authentication |
| CWE-645 | 过于严格的账户锁定机制 | Overly Restrictive Account Lockout Mechanism |
| CWE-804 | 可猜测的CAPTCHA | Guessable CAPTCHA |
| CWE-836 | 使用密码哈希代替密码进行认证 | Use of Password Hash Instead of Password for Authentication |

---

### 4. CWE-1212: 授权错误

与系统授权组件相关的弱点，通常涉及在执行某些操作之前强制要求代理具有所需的权限。

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-425 | 直接请求（"强制浏览"） | Direct Request ('Forced Browsing') |
| CWE-551 | 不正确的行为顺序：解析和规范化之前的授权 | Incorrect Behavior Order: Authorization Before Parsing and Canonicalization |
| CWE-552 | 外部方可访问的文件或目录 | Files or Directories Accessible to External Parties |
| CWE-639 | 通过用户控制的密钥绕过授权 | Authorization Bypass Through User-Controlled Key |
| CWE-653 | 不当的隔离或分区 | Improper Isolation or Compartmentalization |
| CWE-939 | 自定义URL方案处理程序中的不当授权 | Improper Authorization in Handler for Custom URL Scheme |
| CWE-842 | 将用户放入错误的组 | Placement of User into Incorrect Group |
| CWE-1220 | 访问控制粒度不足 | Insufficient Granularity of Access Control |
| CWE-1230 | 通过元数据暴露敏感信息 | Exposure of Sensitive Information Through Metadata |

---

### 5. CWE-1006: 不良编码实践

与被认为不安全且增加可利用漏洞存在机会的编码实践相关的弱点。

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-358 | 标准安全检查的不当实现 | Improperly Implemented Security Check for Standard |
| CWE-360 | 信任系统事件数据 | Trust of System Event Data |
| CWE-478 | 多条件表达式中缺少默认情况 | Missing Default Case in Multiple Condition Expression |
| CWE-487 | 依赖包级别的作用域 | Reliance on Package-level Scope |
| CWE-489 | 活跃的调试代码 | Active Debug Code |
| CWE-547 | 使用硬编码的安全相关常量 | Use of Hard-coded, Security-relevant Constants |
| CWE-561 | 死代码 | Dead Code |
| CWE-562 | 返回栈变量地址 | Return of Stack Variable Address |
| CWE-563 | 赋值给变量但未使用 | Assignment to Variable without Use |
| CWE-581 | 对象模型违规：仅定义了Equals和Hashcode之一 | Object Model Violation: Just One of Equals and Hashcode Defined |
| CWE-586 | 显式调用Finalize() | Explicit Call to Finalize() |
| CWE-605 | 多次绑定到同一端口 | Multiple Binds to the Same Port |
| CWE-628 | 使用不正确指定参数的函数调用 | Function Call with Incorrectly Specified Arguments |
| CWE-654 | 安全决策中依赖单一因素 | Reliance on a Single Factor in a Security Decision |
| CWE-656 | 依赖安全隐晦性 | Reliance on Security Through Obscurity |
| CWE-694 | 使用具有重复标识符的多个资源 | Use of Multiple Resources with Duplicate Identifier |
| CWE-807 | 安全决策中依赖不受信任的输入 | Reliance on Untrusted Inputs in a Security Decision |
| CWE-1041 | 使用冗余代码 | Use of Redundant Code |
| CWE-1043 | 数据元素聚合了过多的非原始元素 | Data Element Aggregating an Excessively Large Number of Non-Primitive Elements |
| CWE-1044 | 水平层数超出预期范围的架构 | Architecture with Number of Horizontal Layers Outside of Expected Range |
| CWE-1045 | 具有虚析构函数的父类和没有虚析构函数的子类 | Parent Class with a Virtual Destructor and a Child Class without a Virtual Destructor |
| CWE-1046 | 使用字符串拼接创建不可变文本 | Creation of Immutable Text Using String Concatenation |
| CWE-1048 | 具有大量向外调用的可调用控制元素 | Invokable Control Element with Large Number of Outward Calls |
| CWE-1049 | 大数据表上的过多数据查询操作 | Excessive Data Query Operations in a Large Data Table |
| CWE-1050 | 循环内过度消耗平台资源 | Excessive Platform Resource Consumption within a Loop |
| CWE-1063 | 在静态代码块中创建类实例 | Creation of Class Instance within a Static Code Block |
| CWE-1065 | 在应用服务器上运行的组件中的运行时资源管理控制元素 | Runtime Resource Management Control Element in a Component Built to Run on Application Servers |
| CWE-1066 | 缺少序列化控制元素 | Missing Serialization Control Element |
| CWE-1067 | 数据资源的过多顺序搜索执行 | Excessive Execution of Sequential Searches of Data Resource |
| CWE-1070 | 包含非可序列化项元素的可序列化数据元素 | Serializable Data Element Containing non-Serializable Item Elements |
| CWE-1071 | 空代码块 | Empty Code Block |
| CWE-1072 | 不使用连接池的数据资源访问 | Data Resource Access without Use of Connection Pooling |
| CWE-1073 | 非SQL可调用控制元素具有过多数据资源访问 | Non-SQL Invokable Control Element with Excessive Number of Data Resource Accesses |
| CWE-1079 | 没有虚析构函数方法的父类 | Parent Class without Virtual Destructor Method |
| CWE-1082 | 类实例自毁控制元素 | Class Instance Self Destruction Control Element |
| CWE-1084 | 具有过多文件或数据访问操作的可调用控制元素 | Invokable Control Element with Excessive File or Data Access Operations |
| CWE-1085 | 具有过多注释代码的可调用控制元素 | Invokable Control Element with Excessive Volume of Commented-out Code |
| CWE-1087 | 具有虚方法但没有虚析构函数的类 | Class with Virtual Method without a Virtual Destructor |
| CWE-1089 | 具有过多索引数的大数据表 | Large Data Table with Excessive Number of Indices |
| CWE-1092 | 在多个架构层中使用相同的可调用控制元素 | Use of Same Invokable Control Element in Multiple Architectural Layers |
| CWE-1094 | 数据资源的过多索引范围扫描 | Excessive Index Range Scan for a Data Resource |
| CWE-1097 | 没有关联比较控制元素的持久可存储数据元素 | Persistent Storable Data Element without Associated Comparison Control Element |
| CWE-1098 | 包含指针项但没有适当复制控制元素的数据元素 | Data Element containing Pointer Item without Proper Copy Control Element |
| CWE-1099 | 标识符的不一致命名约定 | Inconsistent Naming Conventions for Identifiers |
| CWE-1101 | 生成代码中依赖运行时组件 | Reliance on Runtime Component in Generated Code |
| CWE-1102 | 依赖于机器相关的数据表示 | Reliance on Machine-Dependent Data Representation |
| CWE-1103 | 使用平台相关的第三方组件 | Use of Platform-Dependent Third Party Components |
| CWE-1104 | 使用未维护的第三方组件 | Use of Unmaintained Third Party Components |
| CWE-1106 | 符号常量使用不足 | Insufficient Use of Symbolic Constants |
| CWE-1107 | 符号常量定义的隔离不足 | Insufficient Isolation of Symbolic Constant Definitions |
| CWE-1108 | 过度依赖全局变量 | Excessive Reliance on Global Variables |
| CWE-1109 | 将同一变量用于多种用途 | Use of Same Variable for Multiple Purposes |
| CWE-1113 | 不恰当的注释风格 | Inappropriate Comment Style |
| CWE-1114 | 不恰当的空白风格 | Inappropriate Whitespace Style |
| CWE-1115 | 没有标准序言的源代码元素 | Source Code Element without Standard Prologue |
| CWE-1116 | 不准确的源代码注释 | Inaccurate Source Code Comments |
| CWE-1117 | 行为摘要不足的可调用元素 | Callable with Insufficient Behavioral Summary |
| CWE-1126 | 声明了不必要宽作用域的变量 | Declaration of Variable with Unnecessarily Wide Scope |
| CWE-1127 | 编译时警告或错误不足 | Compilation with Insufficient Warnings or Errors |
| CWE-1235 | 性能关键操作中自动装箱和拆箱的不正确使用 | Incorrect Use of Autoboxing and Unboxing for Performance Critical Operations |

---

### 6. CWE-438: 行为问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-115 | 输入的误解 | Misinterpretation of Input |
| CWE-179 | 不正确的行为顺序：过早验证 | Incorrect Behavior Order: Early Validation |
| CWE-408 | 不正确的行为顺序：过早放大 | Incorrect Behavior Order: Early Amplification |
| CWE-437 | 端点功能的不完整模型 | Incomplete Model of Endpoint Features |
| CWE-439 | 新版本或环境中的行为变化 | Behavioral Change in New Version or Environment |
| CWE-440 | 预期行为违反 | Expected Behavior Violation |
| CWE-444 | HTTP请求的不一致解释（"HTTP请求/响应走私"） | Inconsistent Interpretation of HTTP Requests ('HTTP Request/Response Smuggling') |
| CWE-480 | 使用不正确的运算符 | Use of Incorrect Operator |
| CWE-483 | 不正确的块界定 | Incorrect Block Delimitation |
| CWE-484 | Switch中遗漏Break语句 | Omitted Break Statement in Switch |
| CWE-551 | 不正确的行为顺序：解析和规范化之前的授权 | Incorrect Behavior Order: Authorization Before Parsing and Canonicalization |
| CWE-698 | 重定向后执行（EAR） | Execution After Redirect (EAR) |
| CWE-733 | 编译器优化移除或修改安全关键代码 | Compiler Optimization Removal or Modification of Security-critical Code |
| CWE-783 | 运算符优先级逻辑错误 | Operator Precedence Logic Error |
| CWE-835 | 具有不可达退出条件的循环（"无限循环"） | Loop with Unreachable Exit Condition ('Infinite Loop') |
| CWE-837 | 单一唯一操作的不当执行 | Improper Enforcement of a Single, Unique Action |
| CWE-841 | 行为工作流的不当执行 | Improper Enforcement of Behavioral Workflow |
| CWE-1025 | 使用错误因素进行比较 | Comparison Using Wrong Factors |
| CWE-1037 | 处理器优化移除或修改安全关键代码 | Processor Optimization Removal or Modification of Security-critical Code |

---

### 7. CWE-840: 业务逻辑错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-283 | 未验证的所有权 | Unverified Ownership |
| CWE-639 | 通过用户控制的密钥绕过授权 | Authorization Bypass Through User-Controlled Key |
| CWE-640 | 忘记密码的弱密码恢复机制 | Weak Password Recovery Mechanism for Forgotten Password |
| CWE-708 | 不正确的所有权分配 | Incorrect Ownership Assignment |
| CWE-770 | 无限制或无节制的资源分配 | Allocation of Resources Without Limits or Throttling |
| CWE-826 | 在预期生命周期内过早释放资源 | Premature Release of Resource During Expected Lifetime |
| CWE-837 | 单一唯一操作的不当执行 | Improper Enforcement of a Single, Unique Action |
| CWE-841 | 行为工作流的不当执行 | Improper Enforcement of Behavioral Workflow |

---

### 8. CWE-417: 通信通道错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-322 | 没有实体认证的密钥交换 | Key Exchange without Entity Authentication |
| CWE-346 | 来源验证错误 | Origin Validation Error |
| CWE-385 | 隐蔽时序通道 | Covert Timing Channel |
| CWE-419 | 未保护的主要通道 | Unprotected Primary Channel |
| CWE-420 | 未保护的替代通道 | Unprotected Alternate Channel |
| CWE-425 | 直接请求（"强制浏览"） | Direct Request ('Forced Browsing') |
| CWE-515 | 隐蔽存储通道 | Covert Storage Channel |
| CWE-918 | 服务器端请求伪造（SSRF） | Server-Side Request Forgery (SSRF) |
| CWE-924 | 通信通道中消息完整性的不当执行 | Improper Enforcement of Message Integrity During Transmission in a Communication Channel |
| CWE-940 | 通信通道来源的不当验证 | Improper Verification of Source of a Communication Channel |
| CWE-941 | 通信通道中不正确指定的目标 | Incorrectly Specified Destination in a Communication Channel |
| CWE-1327 | 绑定到不受限制的IP地址 | Binding to an Unrestricted IP Address |

---

### 9. CWE-1226: 复杂性问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-1043 | 数据元素聚合了过多的非原始元素 | Data Element Aggregating an Excessively Large Number of Non-Primitive Elements |
| CWE-1047 | 具有循环依赖的模块 | Modules with Circular Dependencies |
| CWE-1055 | 从具体类的多重继承 | Multiple Inheritance from Concrete Classes |
| CWE-1056 | 具有可变参数的可调用控制元素 | Invokable Control Element with Variadic Parameters |
| CWE-1060 | 过多的低效服务器端数据访问 | Excessive Number of Inefficient Server-Side Data Accesses |
| CWE-1064 | 签名中包含过多参数的可调用控制元素 | Invokable Control Element with Signature Containing an Excessive Number of Parameters |
| CWE-1074 | 继承层次过深的类 | Class with Excessively Deep Inheritance |
| CWE-1075 | Switch块外的无条件控制流转移 | Unconditional Control Flow Transfer outside of Switch Block |
| CWE-1080 | 代码行数过多的源代码文件 | Source Code File with Excessive Number of Lines of Code |
| CWE-1086 | 子类数量过多的类 | Class with Excessive Number of Child Classes |
| CWE-1095 | 循环内的循环条件值更新 | Loop Condition Value Update within the Loop |
| CWE-1119 | 过度使用无条件分支 | Excessive Use of Unconditional Branching |
| CWE-1121 | 过高的McCabe圈复杂度 | Excessive McCabe Cyclomatic Complexity |
| CWE-1122 | 过高的Halstead复杂度 | Excessive Halstead Complexity |
| CWE-1123 | 过度使用自修改代码 | Excessive Use of Self-Modifying Code |
| CWE-1124 | 过深的嵌套 | Excessively Deep Nesting |
| CWE-1125 | 过大的攻击面 | Excessive Attack Surface |
| CWE-1333 | 低效的正则表达式复杂度 | Inefficient Regular Expression Complexity |

---

### 10. CWE-557: 并发问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-364 | 信号处理程序竞态条件 | Signal Handler Race Condition |
| CWE-366 | 线程内的竞态条件 | Race Condition within a Thread |
| CWE-367 | 检查时间与使用时间（TOCTOU） | Time-of-check Time-of-use (TOCTOU) |
| CWE-368 | 上下文切换竞态条件 | Context Switching Race Condition |
| CWE-386 | 符号名称未映射到正确对象 | Symbolic Name not Mapping to Correct Object |
| CWE-421 | 在替代通道访问期间的竞态条件 | Race Condition During Access to Alternate Channel |
| CWE-663 | 在并发上下文中使用非可重入函数 | Use of a Non-reentrant Function in a Concurrent Context |
| CWE-820 | 缺少同步 | Missing Synchronization |
| CWE-821 | 不正确的同步 | Incorrect Synchronization |
| CWE-1058 | 多线程上下文中具有非final静态可存储或成员元素的可调用控制元素 | Invokable Control Element in Multi-Thread Context with non-Final Static Storable or Member Element |
| CWE-1322 | 在单线程非阻塞上下文中使用阻塞代码 | Use of Blocking Code in Single-threaded, Non-blocking Context |

---

### 11. CWE-255: 凭据管理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-256 | 明文存储密码 | Plaintext Storage of a Password |
| CWE-257 | 以可恢复格式存储密码 | Storing Passwords in a Recoverable Format |
| CWE-260 | 配置文件中的密码 | Password in Configuration File |
| CWE-261 | 密码的弱编码 | Weak Encoding for Password |
| CWE-262 | 未使用密码老化策略 | Not Using Password Aging |
| CWE-263 | 密码老化但过期时间过长 | Password Aging with Long Expiration |
| CWE-324 | 使用超过有效期的密钥 | Use of a Key Past its Expiration Date |
| CWE-521 | 弱密码要求 | Weak Password Requirements |
| CWE-523 | 凭据的未加密传输 | Unprotected Transport of Credentials |
| CWE-549 | 缺少密码字段遮蔽 | Missing Password Field Masking |
| CWE-620 | 未验证的密码更改 | Unverified Password Change |
| CWE-640 | 忘记密码的弱密码恢复机制 | Weak Password Recovery Mechanism for Forgotten Password |
| CWE-798 | 使用硬编码凭据 | Use of Hard-coded Credentials |
| CWE-916 | 使用计算量不足的密码哈希 | Use of Password Hash With Insufficient Computational Effort |
| CWE-1392 | 使用默认凭据 | Use of Default Credentials |

---

### 12. CWE-310: 密码学问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-261 | 密码的弱编码 | Weak Encoding for Password |
| CWE-324 | 使用超过有效期的密钥 | Use of a Key Past its Expiration Date |
| CWE-325 | 缺少密码学步骤 | Missing Cryptographic Step |
| CWE-328 | 使用弱哈希 | Use of Weak Hash |
| CWE-331 | 熵不足 | Insufficient Entropy |
| CWE-334 | 随机值的空间过小 | Small Space of Random Values |
| CWE-335 | 伪随机数生成器（PRNG）中种子的不正确使用 | Incorrect Usage of Seeds in Pseudo-Random Number Generator (PRNG) |
| CWE-338 | 使用密码学弱的伪随机数生成器（PRNG） | Use of Cryptographically Weak Pseudo-Random Number Generator (PRNG) |
| CWE-347 | 密码签名的不当验证 | Improper Verification of Cryptographic Signature |
| CWE-916 | 使用计算量不足的密码哈希 | Use of Password Hash With Insufficient Computational Effort |
| CWE-1204 | 生成弱初始化向量（IV） | Generation of Weak Initialization Vector (IV) |
| CWE-1240 | 使用具有风险实现的密码原语 | Use of a Cryptographic Primitive with a Risky Implementation |

---

### 13. CWE-320: 密钥管理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-322 | 没有实体认证的密钥交换 | Key Exchange without Entity Authentication |
| CWE-323 | 在加密中重用Nonce或密钥对 | Reusing a Nonce, Key Pair in Encryption |
| CWE-324 | 使用超过有效期的密钥 | Use of a Key Past its Expiration Date |
| CWE-798 | 使用硬编码凭据 | Use of Hard-coded Credentials |

---

### 14. CWE-1214: 数据完整性问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-322 | 没有实体认证的密钥交换 | Key Exchange without Entity Authentication |
| CWE-346 | 来源验证错误 | Origin Validation Error |
| CWE-347 | 密码签名的不当验证 | Improper Verification of Cryptographic Signature |
| CWE-348 | 使用不太受信任的来源 | Use of Less Trusted Source |
| CWE-349 | 接受随受信任数据一起的多余不受信任数据 | Acceptance of Extraneous Untrusted Data With Trusted Data |
| CWE-351 | 类型区分不足 | Insufficient Type Distinction |
| CWE-353 | 缺少完整性检查支持 | Missing Support for Integrity Check |
| CWE-354 | 完整性检查值的不当验证 | Improper Validation of Integrity Check Value |
| CWE-494 | 下载代码时缺少完整性检查 | Download of Code Without Integrity Check |
| CWE-565 | 依赖Cookie但缺少验证和完整性检查 | Reliance on Cookies without Validation and Integrity Checking |
| CWE-649 | 依赖对安全相关输入的混淆或加密但缺少完整性检查 | Reliance on Obfuscation or Encryption of Security-Relevant Inputs without Integrity Checking |
| CWE-829 | 从不受信任的控制范围包含功能 | Inclusion of Functionality from Untrusted Control Sphere |
| CWE-924 | 通信通道中消息完整性的不当执行 | Improper Enforcement of Message Integrity During Transmission in a Communication Channel |

---

### 15. CWE-19: 数据处理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-130 | 长度参数不一致的不当处理 | Improper Handling of Length Parameter Inconsistency |
| CWE-166 | 缺少特殊元素的不当处理 | Improper Handling of Missing Special Element |
| CWE-167 | 额外特殊元素的不当处理 | Improper Handling of Additional Special Element |
| CWE-168 | 不一致特殊元素的不当处理 | Improper Handling of Inconsistent Special Elements |
| CWE-178 | 大小写敏感性的不当处理 | Improper Handling of Case Sensitivity |
| CWE-182 | 数据折叠为不安全值 | Collapse of Data into Unsafe Value |
| CWE-186 | 过于限制的正则表达式 | Overly Restrictive Regular Expression |
| CWE-229 | 值的不当处理 | Improper Handling of Values |
| CWE-233 | 参数的不当处理 | Improper Handling of Parameters |
| CWE-237 | 结构元素的不当处理 | Improper Handling of Structural Elements |
| CWE-241 | 意外数据类型的不当处理 | Improper Handling of Unexpected Data Type |
| CWE-409 | 高度压缩数据的不当处理（数据放大） | Improper Handling of Highly Compressed Data (Data Amplification) |
| CWE-472 | 对假定不可变的Web参数的外部控制 | External Control of Assumed-Immutable Web Parameter |
| CWE-601 | URL重定向到不受信任的站点（"开放重定向"） | URL Redirection to Untrusted Site ('Open Redirect') |
| CWE-611 | XML外部实体引用的不当限制 | Improper Restriction of XML External Entity Reference |
| CWE-624 | 可执行正则表达式错误 | Executable Regular Expression Error |
| CWE-625 | 宽松的正则表达式 | Permissive Regular Expression |
| CWE-776 | DTD中递归实体引用的不当限制（"XML实体扩展"） | Improper Restriction of Recursive Entity References in DTDs ('XML Entity Expansion') |
| CWE-1024 | 不兼容类型的比较 | Comparison of Incompatible Types |

---

### 16. CWE-137: 数据中和问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-76 | 等效特殊元素的不当中和 | Improper Neutralization of Equivalent Special Elements |
| CWE-78 | OS命令中使用的特殊元素的不当中和（"OS命令注入"） | Improper Neutralization of Special Elements used in an OS Command ('OS Command Injection') |
| CWE-79 | Web页面生成期间输入的不当中和（"跨站脚本"） | Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting') |
| CWE-88 | 命令中参数分隔符的不当中和（"参数注入"） | Improper Neutralization of Argument Delimiters in a Command ('Argument Injection') |
| CWE-89 | SQL命令中使用的特殊元素的不当中和（"SQL注入"） | Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') |
| CWE-90 | LDAP查询中使用的特殊元素的不当中和（"LDAP注入"） | Improper Neutralization of Special Elements used in an LDAP Query ('LDAP Injection') |
| CWE-91 | XML注入（又称盲XPath注入） | XML Injection (aka Blind XPath Injection) |
| CWE-93 | CRLF序列的不当中和（"CRLF注入"） | Improper Neutralization of CRLF Sequences ('CRLF Injection') |
| CWE-94 | 代码生成的不当控制（"代码注入"） | Improper Control of Generation of Code ('Code Injection') |
| CWE-117 | 日志的不当输出中和 | Improper Output Neutralization for Logs |
| CWE-140 | 分隔符的不当中和 | Improper Neutralization of Delimiters |
| CWE-170 | 不正确的Null终止 | Improper Null Termination |
| CWE-463 | 删除数据结构哨兵 | Deletion of Data Structure Sentinel |
| CWE-464 | 添加数据结构哨兵 | Addition of Data Structure Sentinel |
| CWE-641 | 文件和其他资源名称的不当限制 | Improper Restriction of Names for Files and Other Resources |
| CWE-694 | 使用具有重复标识符的多个资源 | Use of Multiple Resources with Duplicate Identifier |
| CWE-791 | 特殊元素的不完全过滤 | Incomplete Filtering of Special Elements |
| CWE-838 | 输出上下文的不适当编码 | Inappropriate Encoding for Output Context |
| CWE-917 | 表达式语言语句中使用的特殊元素的不当中和（"表达式语言注入"） | Improper Neutralization of Special Elements used in an Expression Language Statement ('Expression Language Injection') |
| CWE-1236 | CSV文件中公式元素的不当中和 | Improper Neutralization of Formula Elements in a CSV File |

---

### 17. CWE-1225: 文档问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-1053 | 设计缺少文档 | Missing Documentation for Design |
| CWE-1068 | 实现与文档化设计之间的不一致 | Inconsistency Between Implementation and Documented Design |
| CWE-1110 | 不完整的设计文档 | Incomplete Design Documentation |
| CWE-1111 | 不完整的I/O文档 | Incomplete I/O Documentation |
| CWE-1112 | 不完整的程序执行文档 | Incomplete Documentation of Program Execution |
| CWE-1118 | 错误处理技术的文档不足 | Insufficient Documentation of Error Handling Techniques |

---

### 18. CWE-1219: 文件处理问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-22 | 路径名不当限制到受限目录（"路径遍历"） | Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal') |
| CWE-41 | 路径等价的不当解析 | Improper Resolution of Path Equivalence |
| CWE-59 | 文件访问前的不当链接解析（"链接跟随"） | Improper Link Resolution Before File Access ('Link Following') |
| CWE-66 | 标识虚拟资源的文件名的不当处理 | Improper Handling of File Names that Identify Virtual Resources |
| CWE-378 | 使用不安全权限创建临时文件 | Creation of Temporary File With Insecure Permissions |
| CWE-379 | 在具有不安全权限的目录中创建临时文件 | Creation of Temporary File in Directory with Insecure Permissions |
| CWE-426 | 不受信任的搜索路径 | Untrusted Search Path |
| CWE-427 | 不受控制的搜索路径元素 | Uncontrolled Search Path Element |
| CWE-428 | 未加引号的搜索路径或元素 | Unquoted Search Path or Element |

---

### 19. CWE-1227: 封装问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-1054 | 在不必要深的水平层调用控制元素 | Invocation of a Control Element at an Unnecessarily Deep Horizontal Layer |
| CWE-1057 | 预期数据管理器组件外的数据访问操作 | Data Access Operations Outside of Expected Data Manager Component |
| CWE-1062 | 父类引用子类 | Parent Class with References to Child Class |
| CWE-1083 | 从预期数据管理器组件外部进行数据访问 | Data Access from Outside Expected Data Manager Component |
| CWE-1090 | 方法中访问另一个类的成员元素 | Method Containing Access of a Member Element from Another Class |
| CWE-1100 | 系统相关功能的隔离不足 | Insufficient Isolation of System-Dependent Functions |
| CWE-1105 | 机器相关功能的封装不足 | Insufficient Encapsulation of Machine-Dependent Functionality |

---

### 20. CWE-389: 错误条件、返回值、状态码

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-209 | 生成包含敏感信息的错误消息 | Generation of Error Message Containing Sensitive Information |
| CWE-248 | 未捕获的异常 | Uncaught Exception |
| CWE-252 | 未检查的返回值 | Unchecked Return Value |
| CWE-253 | 函数返回值的不正确检查 | Incorrect Check of Function Return Value |
| CWE-390 | 检测到错误条件但未采取行动 | Detection of Error Condition Without Action |
| CWE-391 | 未检查的错误条件 | Unchecked Error Condition |
| CWE-392 | 缺少错误条件报告 | Missing Report of Error Condition |
| CWE-393 | 返回错误的状态码 | Return of Wrong Status Code |
| CWE-394 | 意外的状态码或返回值 | Unexpected Status Code or Return Value |
| CWE-395 | 使用NullPointerException捕获检测NULL指针解引用 | Use of NullPointerException Catch to Detect NULL Pointer Dereference |
| CWE-396 | 声明捕获通用异常 | Declaration of Catch for Generic Exception |
| CWE-397 | 声明抛出通用异常 | Declaration of Throws for Generic Exception |
| CWE-544 | 缺少标准化的错误处理机制 | Missing Standardized Error Handling Mechanism |
| CWE-584 | Finally块中的Return | Return Inside Finally Block |
| CWE-617 | 可达的断言 | Reachable Assertion |
| CWE-756 | 缺少自定义错误页面 | Missing Custom Error Page |

---

### 21. CWE-569: 表达式问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-480 | 使用不正确的运算符 | Use of Incorrect Operator |
| CWE-570 | 表达式始终为False | Expression is Always False |
| CWE-571 | 表达式始终为True | Expression is Always True |
| CWE-783 | 运算符优先级逻辑错误 | Operator Precedence Logic Error |

---

### 22. CWE-429: 处理程序错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-430 | 部署了错误的处理程序 | Deployment of Wrong Handler |
| CWE-431 | 缺少处理程序 | Missing Handler |
| CWE-434 | 不受限制地上传危险类型的文件 | Unrestricted Upload of File with Dangerous Type |

---

### 23. CWE-199: 信息管理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-201 | 将敏感信息插入已发送的数据 | Insertion of Sensitive Information Into Sent Data |
| CWE-204 | 可观测的响应差异 | Observable Response Discrepancy |
| CWE-205 | 可观测的行为差异 | Observable Behavioral Discrepancy |
| CWE-208 | 可观测的时序差异 | Observable Timing Discrepancy |
| CWE-209 | 生成包含敏感信息的错误消息 | Generation of Error Message Containing Sensitive Information |
| CWE-212 | 在存储或传输前不当移除敏感信息 | Improper Removal of Sensitive Information Before Storage or Transfer |
| CWE-213 | 由于不兼容的策略导致敏感信息暴露 | Exposure of Sensitive Information Due to Incompatible Policies |
| CWE-214 | 使用可见敏感信息调用进程 | Invocation of Process Using Visible Sensitive Information |
| CWE-215 | 将敏感信息插入调试代码 | Insertion of Sensitive Information Into Debugging Code |
| CWE-312 | 明文存储敏感信息 | Cleartext Storage of Sensitive Information |
| CWE-319 | 明文传输敏感信息 | Cleartext Transmission of Sensitive Information |
| CWE-359 | 将私人个人信息暴露给未授权的行为者 | Exposure of Private Personal Information to an Unauthorized Actor |
| CWE-497 | 将敏感系统信息暴露给未授权的控制范围 | Exposure of Sensitive System Information to an Unauthorized Control Sphere |
| CWE-524 | 使用包含敏感信息的缓存 | Use of Cache Containing Sensitive Information |
| CWE-538 | 将敏感信息插入外部可访问的文件或目录 | Insertion of Sensitive Information into Externally-Accessible File or Directory |
| CWE-921 | 在没有访问控制的机制中存储敏感数据 | Storage of Sensitive Data in a Mechanism without Access Control |
| CWE-1230 | 通过元数据暴露敏感信息 | Exposure of Sensitive Information Through Metadata |

---

### 24. CWE-452: 初始化和清理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-212 | 在存储或传输前不当移除敏感信息 | Improper Removal of Sensitive Information Before Storage or Transfer |
| CWE-454 | 受信任变量或数据存储的外部初始化 | External Initialization of Trusted Variables or Data Stores |
| CWE-455 | 初始化失败时未退出 | Non-exit on Failed Initialization |
| CWE-459 | 不完整的清理 | Incomplete Cleanup |
| CWE-1051 | 使用硬编码网络资源配置数据进行初始化 | Initialization with Hard-Coded Network Resource Configuration Data |
| CWE-1052 | 在初始化中过度使用硬编码字面值 | Excessive Use of Hard-Coded Literals in Initialization |
| CWE-1188 | 使用不安全的默认值初始化资源 | Initialization of a Resource with an Insecure Default |

---

### 25. CWE-1215: 数据验证问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-112 | 缺少XML验证 | Missing XML Validation |
| CWE-179 | 不正确的行为顺序：过早验证 | Incorrect Behavior Order: Early Validation |
| CWE-183 | 允许输入的宽松列表 | Permissive List of Allowed Inputs |
| CWE-184 | 不完整的禁止输入列表 | Incomplete List of Disallowed Inputs |
| CWE-606 | 未检查的循环条件输入 | Unchecked Input for Loop Condition |
| CWE-641 | 文件和其他资源名称的不当限制 | Improper Restriction of Names for Files and Other Resources |
| CWE-1173 | 验证框架的不当使用 | Improper Use of Validation Framework |
| CWE-1284 | 输入中指定数量的不当验证 | Improper Validation of Specified Quantity in Input |
| CWE-1285 | 输入中指定索引、位置或偏移的不当验证 | Improper Validation of Specified Index, Position, or Offset in Input |
| CWE-1286 | 输入语法正确性的不当验证 | Improper Validation of Syntactic Correctness of Input |
| CWE-1287 | 输入指定类型的不当验证 | Improper Validation of Specified Type of Input |
| CWE-1288 | 输入内一致性的不当验证 | Improper Validation of Consistency within Input |
| CWE-1289 | 输入中不安全等价性的不当验证 | Improper Validation of Unsafe Equivalence in Input |

---

### 26. CWE-1216: 锁定机制错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-645 | 过于严格的账户锁定机制 | Overly Restrictive Account Lockout Mechanism |

---

### 27. CWE-1218: 内存缓冲区错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-120 | 不检查输入大小的缓冲区复制（"经典缓冲区溢出"） | Buffer Copy without Checking Size of Input ('Classic Buffer Overflow') |
| CWE-124 | 缓冲区下写（"缓冲区下溢"） | Buffer Underwrite ('Buffer Underflow') |
| CWE-125 | 越界读取 | Out-of-bounds Read |
| CWE-131 | 缓冲区大小的不正确计算 | Incorrect Calculation of Buffer Size |
| CWE-786 | 在缓冲区起始位置之前访问内存位置 | Access of Memory Location Before Start of Buffer |
| CWE-787 | 越界写入 | Out-of-bounds Write |
| CWE-788 | 在缓冲区末尾之后访问内存位置 | Access of Memory Location After End of Buffer |
| CWE-805 | 使用不正确长度值的缓冲区访问 | Buffer Access with Incorrect Length Value |
| CWE-1284 | 输入中指定数量的不当验证 | Improper Validation of Specified Quantity in Input |

---

### 28. CWE-189: 数值错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-128 | 回绕错误 | Wrap-around Error |
| CWE-190 | 整数溢出或回绕 | Integer Overflow or Wraparound |
| CWE-191 | 整数下溢（回绕） | Integer Underflow (Wrap or Wraparound) |
| CWE-193 | 差一错误 | Off-by-one Error |
| CWE-369 | 除以零 | Divide By Zero |
| CWE-681 | 数值类型之间的不正确转换 | Incorrect Conversion between Numeric Types |
| CWE-839 | 没有最小值检查的数值范围比较 | Numeric Range Comparison Without Minimum Check |
| CWE-1335 | 整数的不正确位移 | Incorrect Bitwise Shift of Integer |
| CWE-1339 | 实数的精度或准确度不足 | Insufficient Precision or Accuracy of a Real Number |
| CWE-1389 | 不同基数数字的不正确解析 | Incorrect Parsing of Numbers with Different Radices |

---

### 29. CWE-275: 权限问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-276 | 不正确的默认权限 | Incorrect Default Permissions |
| CWE-277 | 不安全的继承权限 | Insecure Inherited Permissions |
| CWE-278 | 不安全的保留继承权限 | Insecure Preserved Inherited Permissions |
| CWE-279 | 不正确的执行分配权限 | Incorrect Execution-Assigned Permissions |
| CWE-280 | 对权限不足的不当处理 | Improper Handling of Insufficient Permissions or Privileges |
| CWE-281 | 权限的不当保留 | Improper Preservation of Permissions |
| CWE-618 | 暴露不安全的ActiveX方法 | Exposed Unsafe ActiveX Method |
| CWE-766 | 关键数据元素声明为Public | Critical Data Element Declared Public |
| CWE-767 | 通过公共方法访问关键私有变量 | Access to Critical Private Variable via Public Method |

---

### 30. CWE-465: 指针问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-466 | 返回预期范围外的指针值 | Return of Pointer Value Outside of Expected Range |
| CWE-468 | 不正确的指针缩放 | Incorrect Pointer Scaling |
| CWE-469 | 使用指针减法确定大小 | Use of Pointer Subtraction to Determine Size |
| CWE-476 | NULL指针解引用 | NULL Pointer Dereference |
| CWE-587 | 将固定地址赋给指针 | Assignment of a Fixed Address to a Pointer |
| CWE-763 | 释放无效的指针或引用 | Release of Invalid Pointer or Reference |
| CWE-822 | 不受信任的指针解引用 | Untrusted Pointer Dereference |
| CWE-823 | 使用越界指针偏移 | Use of Out-of-range Pointer Offset |
| CWE-824 | 访问未初始化的指针 | Access of Uninitialized Pointer |
| CWE-825 | 过期指针解引用 | Expired Pointer Dereference |

---

### 31. CWE-265: 权限提升问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-243 | 创建chroot监牢但未更改工作目录 | Creation of chroot Jail Without Changing Working Directory |
| CWE-250 | 以不必要的权限执行 | Execution with Unnecessary Privileges |
| CWE-266 | 不正确的权限分配 | Incorrect Privilege Assignment |
| CWE-267 | 使用不安全操作定义的权限 | Privilege Defined With Unsafe Actions |
| CWE-268 | 权限链接 | Privilege Chaining |
| CWE-270 | 权限上下文切换错误 | Privilege Context Switching Error |
| CWE-272 | 最小权限违反 | Least Privilege Violation |
| CWE-273 | 对已放弃权限的不当检查 | Improper Check for Dropped Privileges |
| CWE-274 | 对权限不足的不当处理 | Improper Handling of Insufficient Privileges |
| CWE-280 | 对权限不足的不当处理 | Improper Handling of Insufficient Permissions or Privileges |
| CWE-501 | 信任边界违反 | Trust Boundary Violation |
| CWE-580 | clone()方法未调用super.clone() | clone() Method Without Call to super.clone() |
| CWE-648 | 特权API的不正确使用 | Incorrect Use of Privileged APIs |

---

### 32. CWE-1213: 随机数问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-331 | 熵不足 | Insufficient Entropy |
| CWE-334 | 随机值的空间过小 | Small Space of Random Values |
| CWE-335 | 伪随机数生成器（PRNG）中种子的不正确使用 | Incorrect Usage of Seeds in PRNG |
| CWE-338 | 使用密码学弱的伪随机数生成器（PRNG） | Use of Cryptographically Weak PRNG |
| CWE-341 | 从可观测状态预测 | Predictable from Observable State |
| CWE-342 | 从先前的值预测确切值 | Predictable Exact Value from Previous Values |
| CWE-343 | 从先前的值预测值范围 | Predictable Value Range from Previous Values |
| CWE-344 | 在动态变化的上下文中使用不变值 | Use of Invariant Value in Dynamically Changing Context |
| CWE-1241 | 在随机数生成器中使用可预测算法 | Use of Predictable Algorithm in Random Number Generator |

---

### 33. CWE-411: 资源锁定问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-412 | 不受限制的外部可访问锁 | Unrestricted Externally Accessible Lock |
| CWE-413 | 不当的资源锁定 | Improper Resource Locking |
| CWE-414 | 缺少锁检查 | Missing Lock Check |
| CWE-609 | 双重检查锁定 | Double-Checked Locking |
| CWE-764 | 对关键资源的多次锁定 | Multiple Locks of a Critical Resource |
| CWE-765 | 对关键资源的多次解锁 | Multiple Unlocks of a Critical Resource |
| CWE-832 | 解锁未被锁定的资源 | Unlock of a Resource that is not Locked |
| CWE-833 | 死锁 | Deadlock |

---

### 34. CWE-399: 资源管理错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-73 | 文件名或路径的外部控制 | External Control of File Name or Path |
| CWE-403 | 文件描述符暴露给非预期的控制范围（"文件描述符泄漏"） | Exposure of File Descriptor to Unintended Control Sphere ('File Descriptor Leak') |
| CWE-410 | 资源池不足 | Insufficient Resource Pool |
| CWE-470 | 使用外部控制的输入选择类或代码（"不安全的反射"） | Use of Externally-Controlled Input to Select Classes or Code ('Unsafe Reflection') |
| CWE-502 | 不受信任数据的反序列化 | Deserialization of Untrusted Data |
| CWE-619 | 悬挂数据库游标（"游标注入"） | Dangling Database Cursor ('Cursor Injection') |
| CWE-641 | 文件和其他资源名称的不当限制 | Improper Restriction of Names for Files and Other Resources |
| CWE-694 | 使用具有重复标识符的多个资源 | Use of Multiple Resources with Duplicate Identifier |
| CWE-763 | 释放无效的指针或引用 | Release of Invalid Pointer or Reference |
| CWE-770 | 无限制或无节制的资源分配 | Allocation of Resources Without Limits or Throttling |
| CWE-771 | 缺少对活跃分配资源的引用 | Missing Reference to Active Allocated Resource |
| CWE-772 | 有效生命周期后缺少资源释放 | Missing Release of Resource after Effective Lifetime |
| CWE-826 | 在预期生命周期内过早释放资源 | Premature Release of Resource During Expected Lifetime |
| CWE-908 | 使用未初始化的资源 | Use of Uninitialized Resource |
| CWE-909 | 缺少资源初始化 | Missing Initialization of Resource |
| CWE-910 | 使用过期的文件描述符 | Use of Expired File Descriptor |
| CWE-911 | 引用计数的不当更新 | Improper Update of Reference Count |
| CWE-914 | 动态标识变量的不当控制 | Improper Control of Dynamically-Identified Variables |
| CWE-915 | 动态确定的对象属性的不当控制修改 | Improperly Controlled Modification of Dynamically-Determined Object Attributes |
| CWE-920 | 功耗的不当限制 | Improper Restriction of Power Consumption |
| CWE-1188 | 使用不安全的默认值初始化资源 | Initialization of a Resource with an Insecure Default |
| CWE-1341 | 对同一资源或句柄的多次释放 | Multiple Releases of Same Resource or Handle |

---

### 35. CWE-387: 信号错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-364 | 信号处理程序竞态条件 | Signal Handler Race Condition |

---

### 36. CWE-371: 状态问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-15 | 系统或配置设置的外部控制 | External Control of System or Configuration Setting |
| CWE-372 | 不完整的内部状态区分 | Incomplete Internal State Distinction |
| CWE-374 | 将可变对象传递给不受信任的方法 | Passing Mutable Objects to an Untrusted Method |
| CWE-375 | 将可变对象返回给不受信任的调用者 | Returning a Mutable Object to an Untrusted Caller |
| CWE-1265 | 通过嵌套调用对非可重入代码的非预期重入调用 | Unintended Reentrant Invocation of Non-reentrant Code Via Nested Calls |

---

### 37. CWE-133: 字符串错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-134 | 使用外部控制的格式化字符串 | Use of Externally-Controlled Format String |
| CWE-135 | 多字节字符串长度的不正确计算 | Incorrect Calculation of Multi-Byte String Length |
| CWE-480 | 使用不正确的运算符 | Use of Incorrect Operator |

---

### 38. CWE-136: 类型错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-681 | 数值类型之间的不正确转换 | Incorrect Conversion between Numeric Types |
| CWE-843 | 使用不兼容类型访问资源（"类型混淆"） | Access of Resource Using Incompatible Type ('Type Confusion') |
| CWE-1287 | 输入指定类型的不当验证 | Improper Validation of Specified Type of Input |

---

### 39. CWE-355: 用户界面安全问题

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-356 | 产品UI未就不安全操作向用户发出警告 | Product UI does not Warn User of Unsafe Actions |
| CWE-357 | 对危险操作的UI警告不足 | Insufficient UI Warning of Dangerous Operations |
| CWE-447 | UI中未实现或不支持的功能 | Unimplemented or Unsupported Feature in UI |
| CWE-448 | UI中的过时功能 | Obsolete Feature in UI |
| CWE-449 | UI执行了错误的操作 | The UI Performs the Wrong Action |
| CWE-549 | 缺少密码字段遮蔽 | Missing Password Field Masking |
| CWE-1007 | 呈现给用户的同形字符的视觉区分不足 | Insufficient Visual Distinction of Homoglyphs Presented to User |
| CWE-1021 | 对渲染的UI层或框架的不当限制 | Improper Restriction of Rendered UI Layers or Frames |

---

### 40. CWE-1217: 用户会话错误

| CWE-ID | 名称（中文） | 名称（英文） |
|--------|-------------|-------------|
| CWE-488 | 将数据元素暴露给错误的会话 | Exposure of Data Element to Wrong Session |
| CWE-613 | 会话过期时间不足 | Insufficient Session Expiration |
| CWE-841 | 行为工作流的不当执行 | Improper Enforcement of Behavioral Workflow |

---

> **注意**: 本文档基于 CWE 4.19.1 版本。某些CWE条目可能同时出现在多个分类中。详细信息请参阅 [CWE官方网站](https://cwe.mitre.org/data/definitions/699.html)。
