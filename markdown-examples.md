# Markdown 格式示例大全

## 1. 基础文本格式

### 标题级别

# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

### 文本样式

**粗体文本**
*斜体文本*
***粗斜体文本***
~~删除线文本~~
`<u>`下划线文本 `</u>`

### 引用块

> 这是一个引用块
> 可以包含多行内容
>
>> 嵌套引用
>>

### 列表

#### 无序列表

- 项目一
- 项目二
  - 子项目一
  - 子项目二
- 项目三

#### 有序列表

1. 第一项
2. 第二项
   1. 子项一
   2. 子项二
3. 第三项

#### 任务列表

- [X] 已完成任务
- [ ] 待完成任务
- [ ] 另一个任务

## 2. 代码块示例

### C++ 代码

```cpp
#include <iostream>
#include <vector>

class Example {
private:
    int value;
    std::vector<int> data;
  
public:
    Example(int val) : value(val) {}
  
    void addData(int num) {
        data.push_back(num);
    }
  
    void print() const {
        std::cout << "Value: " << value << std::endl;
        for (const auto& item : data) {
            std::cout << item << " ";
        }
        std::cout << std::endl;
    }
};

int main() {
    Example ex(42);
    ex.addData(1);
    ex.addData(2);
    ex.addData(3);
    ex.print();
    return 0;
}
```

### Java 代码

```java
import java.util.ArrayList;
import java.util.List;

public class Example {
    private int value;
    private List<Integer> data;
  
    public Example(int value) {
        this.value = value;
        this.data = new ArrayList<>();
    }
  
    public void addData(int num) {
        data.add(num);
    }
  
    public void print() {
        System.out.println("Value: " + value);
        for (int item : data) {
            System.out.print(item + " ");
        }
        System.out.println();
    }
  
    public static void main(String[] args) {
        Example ex = new Example(42);
        ex.addData(1);
        ex.addData(2);
        ex.addData(3);
        ex.print();
    }
}
```

### Shell 脚本

```bash
#!/bin/bash

# 这是一个示例脚本
echo "开始执行脚本..."

# 检查参数
if [ $# -eq 0 ]; then
    echo "错误：请提供参数"
    exit 1
fi

# 循环处理参数
for arg in "$@"; do
    echo "处理参数: $arg"
    # 模拟处理
    sleep 1
done

echo "脚本执行完成"
```

### CMake 配置

```cmake
cmake_minimum_required(VERSION 3.10)
project(MyProject)

# 设置C++标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 查找依赖包
find_package(Boost REQUIRED COMPONENTS filesystem system)

# 添加可执行文件
add_executable(my_app main.cpp)

# 链接库
target_link_libraries(my_app ${Boost_LIBRARIES})

# 包含目录
target_include_directories(my_app PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/include)
```

### Log 文件示例

```log
Dec 31 15:53:59 syncwork drkonqi-coredump-launcher[346668]: Nothing handled the dump :O
Dec 31 15:53:59 syncwork drkonqi-coredump-launcher[346668]: Unable to find file for pid 346653 expected at "kcrash-metadata/corplink-security.1cfa4b1401a34cd0be7511b26c2fa9a7.346653.i>
Dec 31 15:53:59 syncwork systemd[3349]: Started drkonqi-coredump-launcher@5527-346661-0.service - Launch DrKonqi for a systemd-coredump crash (PID 346661/UID 0).
Dec 31 15:53:59 syncwork systemd-coredump[346660]: [LNK] Process 346653 (corplink-securi) of user 1000 dumped core.
   
                                                   Module libsystemd.so.0 from deb systemd-257.9-1~deb13u1.amd64
                                                   Module libblkid.so.1 from deb util-linux-2.41-5.amd64
                                                   Module libmount.so.1 from deb util-linux-2.41-5.amd64
                                                   Module libatomic.so.1 from deb gcc-14-14.2.0-19.amd64
                                                   Stack trace of thread 346653:
                                                   #0  0x00007fdf0c193a77 g_log_structured_array (libglib-2.0.so.0 + 0x66a77)
                                                   #1  0x00007fdf0c193ec9 g_log_default_handler (libglib-2.0.so.0 + 0x66ec9)
                                                   #2  0x00007fdf0c19412b g_logv (libglib-2.0.so.0 + 0x6712b)
                                                   #3  0x00007fdf0c194483 g_log (libglib-2.0.so.0 + 0x67483)

                                                   Stack trace of thread 346656:
                                                   #0  0x00007fdf0b2279ee n/a (libc.so.6 + 0x9a9ee)
                                                   #1  0x00007fdf0b21c668 n/a (libc.so.6 + 0x8f668)
                                                   #2  0x00007fdf0b21c6ad n/a (libc.so.6 + 0x8f6ad)
                                                   #3  0x00007fdf0b290e6e ppoll (libc.so.6 + 0x103e6e)
                                                   #4  0x00007fdf0c18b68c n/a (libglib-2.0.so.0 + 0x5e68c)
 
```

```
[   14.882236] audit: type=1400 audit(1767108607.677:9): apparmor="STATUS" operation="profile_load" profile="unconfined" name=4D6F6E676F444220436F6D70617373 pid=835 comm="apparmor_parser"
[   14.882242] audit: type=1400 audit(1767108607.677:10): apparmor="STATUS" operation="profile_load" profile="unconfined" name="chrome" pid=845 comm="apparmor_parser"
[   14.882248] audit: type=1400 audit(1767108607.677:11): apparmor="STATUS" operation="profile_load" profile="unconfined" name="cam" pid=842 comm="apparmor_parser"
[   14.972378] intel_rapl_common: Found RAPL domain package
[   14.972388] intel_rapl_common: Found RAPL domain core
[   15.473015] NET: Registered PF_QIPCRTR protocol family
[   20.477226] rfkill: input handler disabled
[   21.180310] wlp1s0: authenticate with 48:5f:08:03:b5:3c (local address=1c:bf:c0:ee:2e:af)
[   21.572405] wlp1s0: Limiting TX power to 35 (35 - 0) dBm as advertised by 48:5f:08:03:b5:3c
[   22.620123] evm: overlay not supported
```

### Python 代码

```python
import asyncio
from typing import List, Optional

class DataProcessor:
    def __init__(self, data: List[int]):
        self.data = data
        self.results = []
  
    async def process_item(self, item: int) -> Optional[int]:
        """异步处理单个项目"""
        await asyncio.sleep(0.1)  # 模拟异步操作
        if item > 0:
            return item * 2
        return None
  
    async def process_all(self) -> List[int]:
        """批量处理所有数据"""
        tasks = [self.process_item(item) for item in self.data]
        results = await asyncio.gather(*tasks)
        self.results = [r for r in results if r is not None]
        return self.results

# 使用示例
async def main():
    processor = DataProcessor([1, 2, 3, -1, 5])
    results = await processor.process_all()
    print(f"处理结果: {results}")

if __name__ == "__main__":
    asyncio.run(main())

```

## 3. Mermaid 图表

### Git 分支图

```mermaid
gitGraph
   commit id: "初始提交"
   commit id: "功能A"
   branch develop
   checkout develop
   commit id: "开发环境初始化"
   branch feature-auth
   checkout feature-auth
   commit id: "添加登录功能"
   commit id: "添加注册功能"
   checkout develop
   merge feature-auth id: "合并认证功能"
   branch feature-payment
   checkout feature-payment
   commit id: "集成支付API"
   checkout main
   branch hotfix-security
   checkout hotfix-security
   commit id: "修复安全漏洞"
   checkout main
   merge hotfix-security id: "紧急修复v1.0.1"
   checkout develop
   merge hotfix-security
   checkout feature-payment
   commit id: "完成支付流程"
   checkout develop
   merge feature-payment id: "合并支付功能"
   branch release-v2.0
   checkout release-v2.0
   commit id: "准备发布v2.0"
   checkout main
   merge release-v2.0 id: "发布v2.0"
   checkout develop
   merge release-v2.0
   branch feature-analytics
   checkout feature-analytics
   commit id: "添加数据分析"
```

### 流程图

```mermaid
flowchart TD
    A[开始] --> B{条件判断}
    B -->|条件1| C[处理流程1]
    B -->|条件2| D[处理流程2]
    C --> E[结果1]
    D --> F[结果2]
    E --> G[结束]
    F --> G
```

### 复杂流程图 - Linux 网络通讯架构

```mermaid
flowchart TD
    subgraph UserSpace["用户空间 User Space"]
        App1[应用程序<br/>Web Browser]
        App2[应用程序<br/>SSH Client]
        App3[应用程序<br/>File Transfer]

        Socket[Socket API<br/>系统调用接口]
    end

    subgraph KernelSpace["内核空间 Kernel Space"]
        subgraph TransportLayer["传输层 Transport Layer"]
            TCP[TCP<br/>面向连接]
            UDP[UDP<br/>无连接]
            SCTP[SCTP<br/>流控制]
        end

        subgraph NetworkLayer["网络层 Network Layer"]
            IPv4[IPv4<br/>地址路由]
            IPv6[IPv6<br/>下一代协议]
            IPSec[IPSec<br/>安全协议]
            ICMP[ICMP<br/>控制消息]
        end

        subgraph DataLinkLayer["数据链路层 Data Link Layer"]
            Ethernet[Ethernet<br/>以太网驱动]
            WiFi[WiFi 802.11<br/>无线网驱动]
            Bluetooth[Bluetooth<br/>蓝牙协议栈]
            PPP[PPP<br/>点对点协议]
        end
    end

    subgraph Hardware["硬件层 Hardware Layer"]
        NIC[网卡 NIC<br/>有线网络]
        WNIC[无线网卡<br/>WiFi Adapter]
        BTAdapter[蓝牙适配器<br/>BT Dongle]
        Modem[调制解调器<br/>Modem]
    end

    subgraph PhysicalMedia["物理介质"]
        Cable[网线<br/>Cat5e/Cat6]
        Radio[无线电波<br/>2.4GHz/5GHz]
        BTRadio[蓝牙信号<br/>2.4GHz]
        Phone[电话线<br/>ADSL/Fiber]
    end

    App1 --> Socket
    App2 --> Socket
    App3 --> Socket

    Socket --> TCP
    Socket --> UDP
    Socket --> SCTP

    TCP --> IPv4
    UDP --> IPv4
    SCTP --> IPv4
    TCP --> IPv6
    UDP --> IPv6

    IPv4 --> ICMP
    IPv6 --> ICMP
    IPv4 --> IPSec
    IPv6 --> IPSec

    IPv4 --> Ethernet
    IPv4 --> WiFi
    IPv4 --> Bluetooth
    IPv4 --> PPP

    IPv6 --> Ethernet
    IPv6 --> WiFi
    IPv6 --> Bluetooth

    Ethernet --> NIC
    WiFi --> WNIC
    Bluetooth --> BTAdapter
    PPP --> Modem

    NIC --> Cable
    WNIC --> Radio
    BTAdapter --> BTRadio
    Modem --> Phone

    style UserSpace fill:#e3f2fd
    style KernelSpace fill:#fff3e0
    style Hardware fill:#f1f8e9
    style PhysicalMedia fill:#fce4ec
    style Socket fill:#bbdefb
    style IPv4 fill:#ffe082
    style IPv6 fill:#ffe082
    style Ethernet fill:#c5e1a5
    style WiFi fill:#c5e1a5
    style Bluetooth fill:#c5e1a5
```

### 序列图

```mermaid
sequenceDiagram
    participant User
    participant Frontend
    participant Backend
    participant Database
  
    User->>Frontend: 发起请求
    Frontend->>Backend: API调用
    Backend->>Database: 查询数据
    Database-->>Backend: 返回数据
    Backend-->>Frontend: 响应结果
    Frontend-->>User: 显示结果
```

### 类图

```mermaid
classDiagram
    class Animal {
        +String name
        +int age
        +void eat()
        +void sleep()
    }
  
    class Dog {
        +String breed
        +void bark()
        +void fetch()
    }
  
    class Cat {
        +String color
        +void meow()
        +void climb()
    }
  
    Animal <|-- Dog
    Animal <|-- Cat
```

### 甘特图

```mermaid
gantt
    title 项目开发计划
    dateFormat  YYYY-MM-DD
    section 设计阶段
    需求分析     :done,    des1, 2024-01-01, 2024-01-07
    技术设计     :active,  des2, 2024-01-08, 2024-01-14
    section 开发阶段
    前端开发     :         dev1, 2024-01-15, 2024-01-28
    后端开发     :         dev2, 2024-01-22, 2024-02-05
    section 测试阶段
    单元测试     :         test1, 2024-02-06, 2024-02-12
    集成测试     :         test2, 2024-02-13, 2024-02-20
```

### 状态图

```mermaid
stateDiagram-v2
    [*] --> 待机状态
    待机状态 --> 运行状态 : 启动命令
    运行状态 --> 暂停状态 : 暂停命令
    暂停状态 --> 运行状态 : 继续命令
    运行状态 --> 错误状态 : 发生错误
    错误状态 --> 待机状态 : 重置命令
    运行状态 --> 待机状态 : 停止命令
    暂停状态 --> 待机状态 : 停止命令
```

### 饼图

```mermaid
pie title 编程语言使用分布
    "JavaScript" : 35.6
    "Python" : 28.3
    "Java" : 18.9
    "C++" : 8.2
    "其他" : 9.0
```

### 象限图

技术评估矩阵

```mermaid
quadrantChart
    title Frontend Tech Stack Assessment 2025
    x-axis Low Complexity --> High Complexity
    y-axis Low Value --> High Value
    quadrant-1 Strategic Investment
    quadrant-2 Priority Adoption
    quadrant-3 Phase Out
    quadrant-4 Avoid
    React: [0.75, 0.85]
    Vue3: [0.60, 0.80]
    Svelte: [0.50, 0.75]
    Solid.js: [0.55, 0.70]
    Next.js: [0.80, 0.90]
    Nuxt: [0.70, 0.85]
    Astro: [0.45, 0.78]
    TypeScript: [0.65, 0.95]
    Vite: [0.40, 0.88]
    Tailwind CSS: [0.35, 0.82]
    Angular: [0.85, 0.60]
    Backbone: [0.70, 0.25]
    jQuery: [0.30, 0.20]
    Grunt: [0.55, 0.15]
    Bower: [0.40, 0.10]
```

### XY-Axis图表

```mermaid
xychart-beta
    title "Sales Trend Data"
    x-axis [Jan, Feb, Mar, Apr, May, Jun]
    y-axis "Sales (10K RMB)" 0 --> 120
    bar [65, 59, 80, 81, 56, 55]
    line [28, 48, 40, 19, 86, 27]
```

## 4. 数学公式

### 行内公式

这是一个行内公式：$E = mc^2$，还有勾股定理：$a^2 + b^2 = c^2$。

### 块级公式

#### 二次方程求根公式

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

#### 欧拉公式

$$
e^{i\pi} + 1 = 0
$$

#### 积分公式

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

#### 矩阵运算

$$
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
\times
\begin{bmatrix}
5 & 6 \\
7 & 8
\end{bmatrix}
=
\begin{bmatrix}
19 & 22 \\
43 & 50
\end{bmatrix}
$$

#### 极限公式

$$
\lim_{x \to 0} \frac{\sin x}{x} = 1
$$

## 5. 表格

### 基础表格

| 姓名 | 年龄 | 城市 | 职业     |
| ---- | ---- | ---- | -------- |
| 张三 | 25   | 北京 | 工程师   |
| 李四 | 30   | 上海 | 设计师   |
| 王五 | 28   | 广州 | 产品经理 |

### 对齐表格

| 左对齐     | 居中对齐 | 右对齐 |
| :--------- | :------: | -----: |
| 文本1      |  文本2  |    100 |
| 长文本示例 | 居中文本 | 123.45 |

### 复杂表格

| 项目 | 第一季度 | 第二季度 | 第三季度 | 第四季度 | 总计    |
| ---- | -------- | -------- | -------- | -------- | ------- |
| 收入 | 100,000  | 120,000  | 150,000  | 180,000  | 550,000 |
| 成本 | 60,000   | 70,000   | 80,000   | 90,000   | 300,000 |
| 利润 | 40,000   | 50,000   | 70,000   | 90,000   | 250,000 |

## 6. 五线谱示例

### 简单旋律

```abc
X: 24
T: Clouds Thicken
C: Paul Rosen
S: Copyright 2005
M: 6/8
L: 1/8
Q: 3/8=116
R: James Lee
K: Em
|:"Em"EEE E2G|"C7"_B2A G2F|"Em"EEE E2G|\
"C7"_B2A "B7"=B3|"Em"EEE E2G|
"C7"_B2A G2F|"Em"GFE "D (Bm7)"F2D|\
1"Em"E3-E3:|2"Em"E3-E2B|:"Em"e2e gfe|
"G"g2ab3|"Em"gfeg2e|"D"fedB2A|"Em"e2e gfe|\
"G"g2ab3|"Em"gfe"D"f2d|"Em"e3-e3:|
```

### 和弦进行

```abc
X:2
T:和弦示例
M:4/4
L:1/4
K:C
%%score (T1 T2) (B1 B2)
[V:T1] "C"c2 c2 | "G"g2 g2 | "Am"a2 a2 | "F"f2 f2 |
[V:T2] e2 e2 | d2 d2 | c2 c2 | A2 A2 |
[V:B1] C,2 C,2 | G,2 G,2 | A,2 A,2 | F,2 F,2 |
[V:B2] E,2 E,2 | D,2 D,2 | C,2 C,2 | A,2 A,2 |
```

## 7. 其他格式

### 脑图

```mindmap
- 教程
- 语法指导
  - 普通内容
  - 提及用户
  - 表情符号 Emoji
    - 一些表情例子
  - 大标题 - Heading 3
    - Heading 4
      - Heading 5
        - Heading 6
  - 图片
  - 代码块
    - 普通
    - 语法高亮支持
      - 演示 Go 代码高亮
      - 演示 Java 高亮
  - 有序、无序、任务列表
    - 无序列表
    - 有序列表
    - 任务列表
  - 表格
  - 隐藏细节
  - 段落
  - 链接引用
  - 数学公式
  - 脑图
  - 流程图
  - 时序图
  - 甘特图
  - 图表
  - 五线谱
  - Graphviz
  - 多媒体
  - 脚注
- 快捷键

```

### Graphviz

```graphviz
digraph G {
    node [shape=record, style=filled, fillcolor=lightcyan];
    struct1 [label="<f0> left|<f1> mid|<f2> right"];
    struct2 [label="<f0> one|<f1> two"];
    struct3 [label="hello\nworld |{ b |{c|<here> d|e}| f}| g | h", fillcolor=lightgreen];
    struct1:f1 -> struct2:f0;
    struct1:f2 -> struct3:here;
}

```

```graphviz
digraph DataFlow {
    rankdir=LR;
    node [shape=box, style=rounded];

    start [label="开始", shape=ellipse, style=filled, fillcolor=lightyellow];
    input [label="数据输入", style=filled, fillcolor=lightblue];
    validate [label="数据验证", style=filled, fillcolor=lightcyan];
    process [label="数据处理", style=filled, fillcolor=lightgreen];
    save [label="保存结果", style=filled, fillcolor=lightpink];
    end [label="结束", shape=ellipse, style=filled, fillcolor=lightgray];
    error [label="错误处理", style=filled, fillcolor=lightsalmon];

    start -> input;
    input -> validate;
    validate -> process [label="验证通过"];
    validate -> error [label="验证失败", color=red, style=dashed];
    process -> save;
    save -> end;
    error -> end;
}

```

```graphviz
digraph finite_state_machine {
    rankdir=LR;
    size="8,5"
    node [shape = doublecircle]; S;
    node [shape = point ]; qi

    node [shape = circle];
    qi -> S;
    S  -> q1 [ label = "a" ];
    S  -> S  [ label = "a" ];
    q1 -> S  [ label = "a" ];
    q1 -> q2 [ label = "ddb" ];
    q2 -> q1 [ label = "b" ];
    q2 -> q2 [ label = "b" ];
}
```

### echarts

```echarts
{
  "title": { "text": "月度销售数据" },
  "tooltip": { "trigger": "axis" },
  "legend": { "data": ["销售额", "利润"] },
  "xAxis": {
    "type": "category",
    "data": ["1月", "2月", "3月", "4月", "5月", "6月"]
  },
  "yAxis": { "type": "value" },
  "series": [
    {
      "name": "销售额",
      "type": "bar",
      "data": [120, 200, 150, 80, 70, 110],
      "itemStyle": { "color": "#5470c6" }
    },
    {
      "name": "利润",
      "type": "bar",
      "data": [60, 100, 75, 40, 35, 55],
      "itemStyle": { "color": "#91cc75" }
    }
  ]
}

```

```echarts
{
  "title": { "text": "最近 30 天" },
  "tooltip": { "trigger": "axis", "axisPointer": { "lineStyle": { "width": 0 } } },
  "legend": { "data": ["帖子", "用户", "回帖"] },
  "xAxis": [{
      "type": "category",
      "boundaryGap": false,
      "data": ["2019-05-08","2019-05-09","2019-05-10","2019-05-11","2019-05-12","2019-05-13","2019-05-14","2019-05-15","2019-05-16","2019-05-17","2019-05-18","2019-05-19","2019-05-20","2019-05-21","2019-05-22","2019-05-23","2019-05-24","2019-05-25","2019-05-26","2019-05-27","2019-05-28","2019-05-29","2019-05-30","2019-05-31","2019-06-01","2019-06-02","2019-06-03","2019-06-04","2019-06-05","2019-06-06","2019-06-07"],
      "axisTick": { "show": false },
      "axisLine": { "show": false }
  }],
  "yAxis": [{ "type": "value", "axisTick": { "show": false }, "axisLine": { "show": false }, "splitLine": { "lineStyle": { "color": "rgba(0, 0, 0, .38)", "type": "dashed" } } }],
  "series": [
    {
      "name": "帖子", "type": "line", "smooth": true, "itemStyle": { "color": "#d23f31" }, "areaStyle": { "normal": {} }, "z": 3,
      "data": ["18","14","22","9","7","18","10","12","13","16","6","9","15","15","12","15","8","14","9","10","29","22","14","22","9","10","15","9","9","15","0"]
    },
    {
      "name": "用户", "type": "line", "smooth": true, "itemStyle": { "color": "#f1e05a" }, "areaStyle": { "normal": {} }, "z": 2,
      "data": ["31","33","30","23","16","29","23","37","41","29","16","13","39","23","38","136","89","35","22","50","57","47","36","59","14","23","46","44","51","43","0"]
    },
    {
      "name": "回帖", "type": "line", "smooth": true, "itemStyle": { "color": "#4285f4" }, "areaStyle": { "normal": {} }, "z": 1,
      "data": ["35","42","73","15","43","58","55","35","46","87","36","15","44","76","130","73","50","20","21","54","48","73","60","89","26","27","70","63","55","37","0"]
    }
  ]
}

```

### Flowchart

```flowchart
st=>start: 开始
input=>inputoutput: 输入数据
process1=>operation: 数据处理
process2=>operation: 数据验证
cond1=>condition: 是否合法?
cond2=>condition: 需要审批?
approve=>operation: 提交审批
save=>operation: 保存数据
error=>inputoutput: 错误提示
e=>end: 结束

st->input->process1->process2->cond1
cond1(yes)->cond2
cond1(no)->error->e
cond2(yes)->approve->save->e
cond2(no)->save->e

```

### 多媒体

支持 v.qq.com，youtube.com，youku.com，coub.com，facebook.com/video，dailymotion.com，.mp4，.m4v，.ogg，.ogv，.webm，.mp3，.wav 链接解析

https://v.qq.com/x/cover/zf2z0xpqcculhcz/y0016tj0qvh.html

### 脚注

这是一个带有脚注的句子[^1]。

### 定义列表

术语1
: 这是术语1的定义

术语2
: 这是术语2的定义
: 可以有多个定义

### 高亮文本

==这是高亮文本==

### 上标和下标

H~2~O 是水的化学式，E=mc^2^ 是质能方程。

### 键盘快捷键

按 `<kbd>`Ctrl `</kbd>` + `<kbd>`C `</kbd>` 复制，按 `<kbd>`Ctrl `</kbd>` + `<kbd>`V `</kbd>` 粘贴。

## 8. 链接和图片

### 外部链接

[Google](https://www.google.com)
[GitHub](https://github.com)

### 内部链接

[跳转到代码块](#2-代码块示例)

### 图片

![示例图片](https://via.placeholder.com/400x200?text=示例图片)

### 带标题的图片

<figure>
    <img src="https://via.placeholder.com/400x200?text=带标题的图片" alt="示例图片">
    <figcaption>这是一个带标题的图片示例</figcaption>
</figure>

## 9. 折叠内容

<details>
<summary>点击展开详细内容</summary>

这里是折叠起来的内容，可以包含各种格式：

- 列表项
- 另一个列表项

```python
print("折叠区域内的代码")
```

</details>

## 10. 表情符号和特殊字符

### 常用表情符号

😄 ❤️ ⭐️ 🚀 📚 💻 💡 ⚠️

### 数学符号

∀ ∃ ∈ ∉ ⊂ ⊃ ∪ ∩ ∅ ∞ √ ∫ ∑ ∏ ∂ ∇

### 箭头符号

← → ↑ ↓ ↔ ↕ ⇐ ⇒ ⇔ ⇑ ⇓ ⇕

---

*本文档展示了Markdown的各种格式和功能，可以作为学习和参考使用。*

[^1]: 这是脚注的内容。
