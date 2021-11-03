# Echarts
摘要：在新型冠状病毒2019-nCoV这场严峻的疫情防控阻击战中，大数据及人工智能技术正在信息捕获、数据支撑、辅助决策以及态势监控与综合指挥等层面发挥作用，助力疫情防控和应急管理。科技治疫，共度难关是我们共同的期许。本平台深入贯彻党和国家创新进取，求真探索的理念，深化科技创新，着力打造专业、高效的应急管理可视化决策平台，以科技的力量，助力国家公共卫生事业发展。针对传统处理方法的不足，数据可视化技术显得尤其重要，由此设计了基于 ECharts 的数据可视化系统，以展示新冠肺炎疫情为目标，使得大量枯燥无味的数据变得更加直观、易于理解、可读性强。 新冠疫情大数据平台设有核酸检测量，疫苗接种效率等板块，合理高效配置医疗资源，本土或境外新增溯源，累计确诊数，今日新增数等板块洞悉疫情态势，通行行程大数据对流动人员疫情检测，精准施策，整体有效整合公共资源，提升疫情防控效率。

关键词：Echarts、数据可视化、COVID-19、JavaScript

Abstact: In the severe epidemic prevention and control war of the new coronavirus 2019-nCoV, big data and artificial intelligence technologies are playing a role in information capture, data support, auxiliary decision-making, and situational monitoring and integrated command, helping epidemic prevention and control and emergency management. It is our common expectation that science and technology will help us overcome the difficulties together. The platform deeply implements the Party and State's philosophy of innovation and progress, seeking truthful exploration, deepening scientific and technological innovation, and striving to build a professional and efficient visualization and decision-making platform for emergency management to help the development of national public health with the power of science and technology. In view of the inadequacy of traditional processing methods, data visualization technology is particularly important, and thus a data visualization system based on ECharts was designed to show the New Crown Pneumonia epidemic, making a large amount of boring data more intuitive, easy to understand and readable. The New Crown Epidemic Data Platform has sections for nucleic acid detection volume, vaccination efficiency, etc., to allocate medical resources reasonably and efficiently, new traceability in local or overseas, cumulative number of confirmed cases, today's new cases, etc., to gain insight into the epidemic situation, pass trip big data for epidemic detection of mobile people, and implement precise policies to integrate public resources effectively as a whole and improve the efficiency of epidemic prevention and control.

Keywords: Echarts、Data Visualization、COVID-19、JavaScript 

![image](https://user-images.githubusercontent.com/55519437/139970401-c22a9231-38f3-43ac-bce9-8c215199b96c.png)

![image](https://user-images.githubusercontent.com/55519437/139970404-fddcd949-0efe-44d4-af88-4f567359f692.png)
![image](https://user-images.githubusercontent.com/55519437/139970409-ebf18795-4313-484f-9de4-6c9652d49f9b.png)

![image](https://user-images.githubusercontent.com/55519437/139970415-ce788d8f-f58a-43c1-91f2-6e2baac97aff.png)

0引言

随着大数据的快速增长，数据越来越得到工业界和学术界的重视。面对大量的数据，传统的数据处理方式存在许多不足，例如，数据处理的效率不高及处理结果难以理解等[1]。然而，数据可视化技术能够挖掘数据有价值的信息，尤其属性之间的关系，在数据分析方面具有重要作用[2-3]。伴随数据运营技术的不断发展，数据可视化工具也不断增多，其中ECharts是一款广泛使用的数据可视化工具之一。对于用户而言，数据的采集、计算方式等是透明的，而直观的结果是非常有意义的。为了更加直观地理解数据的内涵，通过数据可视化技术能够 满足此需求[4-5]。针对传统数据处理方式的低效率、难理解及可 读性差等问题，设计了基于 ECharts 的数据可视化系统。通过模拟数据对系统进行验证，结果表明该系统能够实现数据可视化，使得人们更易于理解单调数据中蕴含的重要信息。

1 ECharts

ECharts 是一款由百度研发团队开发的开源数据可视化库，可流畅地运行在PC和移动设备上，兼容当前绝大部分浏览器，如 IE8/9/10/11，Chrome，Firefox，Safari 等。ECharts 底层依赖轻量级的矢量图形库 ZRender，能够提供直观、交互丰富和可高度个性化定制的数据可视化图表。
ECharts 提供了常见的柱状图、折线图、饼状图、玫瑰图及雷达图等，能够直观地将数据进行可视化。此外，ECharts 可以将这些数据进行一定的交互，除了 PC 和移动端的交互，目前也适用于一些小程序[6]。

2 系统设计

2.1 需求分析

针对新型冠状病毒肺炎疫情的严峻形势，为了让人们能够较快且准确地了解当下的情形，如患者人数分布、患者的性别分布等，数据可视化显得尤为重要。然而，单一的图表显示数据难以让人们直观地了解当前疫情的总体情况。因此，设计基于 ECharts 的数据可视化系统成为迫切需求，系统的显示结果便于用户直观理解数据的信息。随着新冠肺炎疫情在全球蔓延，及时有效地了解疫情情况显得尤为重要。

2.2 技术框架设计

系统由前端和后端 2 个部分组成。通过 Html、JavaScript等技术实现前端页面，使用 ECharts 实现数据可视化;通过 后台 MySQL 数据库对获取的数据进行创建和存储，使用 JSP 和 Servlet 对后台进行维护。因此，系统是一套完整的前端 ( 网 页 ) 和后端 ( 数 据 库 、服 务 器 、A j a x ) 实 现 实 时 交 互 的 数 据监控系统，如图 1 所示。
 
![image](https://user-images.githubusercontent.com/55519437/139970601-61e72820-f2e1-4fae-a6cf-a4b8bc374716.png)

图 1 系统框架

通过 ECharts 实现疫情数据的可视化，包括柱状图模块、折线图模块、饼状图模块及地图迁徙模块等。为了让人们能够实时地获取当下疫情的情况，在获取数据方面添加了定时器，以一定时间间隔向后台请求数据。ECharts 图标是纯 JavaScript 的图标库，为了实现数据的实时显示，系统在后端通过 MySQL 创建存储模拟数据，并定时向数据库获取数据，在前端通过 JSON 将数据传送到前端 JSP 页面。

2.3 页面设计

系统页面主要包括折线图、饼状图、柱状图及迁徙地图等。折线图主要用于记录每日新增确诊人数、疑似人数、境外输入人数;饼状图用于显示确诊人员的年龄分布和地区分布;柱状图主要用于记录最近一周治愈的人数、各个类型人数比例;中国迁徙地图主要用于显示各个地区支援武汉的情况。系统上部显示全国确诊人数和治愈人数，系统右上角显示系统的本地时间。由于本文使用模拟数据，系统显示的时间与网络时间并不同步。为了反映疫情的真实情况，未来将使用真实的数据且保持时间同步。

2.4 数据库设计
数据库设计是指对于一个给定的应用环境，构造最优的数据库模式，建立数据库及其应用系统，使之能够有效地 存储、查询，满足各类用户的应用需求。数据库的设计结构 模型如下:

DROP TABLE IF EXISTS `week`;
CREATE TABLE `week` (
`day` varchar (255) CHARACTER SET latin1 COLLATE
latin1_swedish_ci NULL DEFAULT NULL, `num` int (11) NULL DEFAULT NULL) ENGINE = InnoDB CHARACTER SET = latin1 COLLATE = latin1_swedish_ci ROW_FORMAT = Compact;

3 系统实现

通过 JSP、Html 实现前端页面。在 Html 文件中设置三大板块，其中，两侧板块展示数据可视化图表，中间板块展示迁徙地图模型，在 Html 文件中创建合适的 div 用于存放相应的板块。JavaScript 是一种轻量级的 Web 脚本语言，实现前后端信息交互。在 Js 文件中通过 Ajax 异步请求向数据库获取数据，然后利用 ECharts 可视化插件，在动态网页中使得数据可视化，如图 2 所示。
系统交互的具体流程:1 在Html文件中创建 ECharts 图 表 的 div 模 块 ; 2 将 echart.min.js，flexible.js，jquery.js，china.js，myMap.js 等文件通过 <script> 标签添加到 Html 文件，并配置相关的可视化图表;3 在 index.js 文件中实例化 ECharts 对象，通过 option 定制可视化图表的数值，其中包含横坐标的日期和纵坐标的确诊人数;4 通过 Ajax 获取数据并发送至 series 中的 data 中。

![image](https://user-images.githubusercontent.com/55519437/139970619-13993763-f231-41f2-b5d8-0ad12b4abe99.png)

图 2 系统交互流程图

  实现系统交互的伪代码如下:
  
function {
实例化对象 myChart; 指定图标配置和数据; option =
{
xAxis: [ " 星期日 ", " 星期一 ", " 星期二 ", " 星期三
", " 星期四 ", " 星期五 ", " 星期六 " ],
yAxis: 使用 ajax 请求代码块获取数据: 请求方式:
get,同步执行
url: bar
返回数据形式: json
成功:将返回的 result 数据处理，保存到 arr 数组中 if (result 不为空)
{
遍历
{
arr.push(result[i].num);
} }
失败: 给出提示
把配置给实例对象 myChart.setOption(option); }
};
  
最后，为了验证系统的有效性，使用通过 MySQL 创建和存储模拟疫情数据。除了显示二维图表，还可以通过 ECharts 显示三维图表，如果实时地产生数据，将显示动态的效果。与传统的数据显示模式相比，基于 ECharts 的数据可视化图表更易于理解。若实时显示数据需要向数据库中定时发送请求，同 时数据库中数据需要同步更新。
本文以新冠肺炎疫情为例，有效进行了数据可视化分析。 此外，基于 ECharts 的数据可视化系统还可以应用于网站访问监测，分析用户行为，为可能的恶意访问行为发出预警，其难点在于网络流量的异构性。因此，需要增加系统的异构数据处理模块。

4 结束语
  
大数据时代，面对大量的数据，用户理解数据显得更加困难。由于传统数据处理方法存在处理效率低、处理结果难理解等问题，数据可视化技术得到了广泛应用。因此，设计了基于 ECharts 的数据可视化系统，该系统对新冠肺炎疫情的模拟数据进行分析，分析结果更加直观、易于理解，且增加了交互功能。
系统还可以做一些改进，比如数据可以通过爬虫实时获取其他网站的实时数据、迁徙地图可以增加交互功能、疫情特别严重的地区可以通过不同颜色深度作为警示、省或市的数据实现地图切换。随着疫情蔓延，还可以分析国外的疫情数据并显示，让人们全面了解全球疫情。
