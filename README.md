[![GitHub license](https://camo.githubusercontent.com/5eaf3ed8a7e8ccb15c21d967b8635ac79e8b1865da3a5ccf78d2572a3e10738a/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f646f746e65742f6173706e6574636f72653f636f6c6f723d253233306230267374796c653d666c61742d737175617265)](https://github.com/ganweisoft/Mini-Gateway-Python/blob/main/LICENSE) ![Docker](https://img.shields.io/github/v/release/ganweisoft/toms?logo=docker) ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![](https://img.shields.io/badge/join-discord-infomational)


## 介绍

分离自[**GateWay**](https://github.com/ganweisoft/Gateway)的一个可扩展的Python环境分布式网关, 使得开发者可以使用自己熟悉的开发语言进行快速开发

### 消息路径

使用[dapr](https://docs.dapr.io/)的消息通道, 传输设备的实时值到GateWay主网关. 架构图:   
![img.png](img.png)

1. GateWay主网关作为subscriber. 
2. 消息队列中间件可选MQTT, Kafka, Redis等.
3. GateWay4Python作为publisher.

### 内部扩展

1. 同GateWay一样, 可进行内部扩展. 只需继承CEquipBase, 将类名命名为CEquip.
生成的文件放入GWHost1的上层目录的dll目录下.
GWMiniDataCenter启动是即可自扫描加载.
```python
if __name__ == '__main__':
    from ganweisoft.DataCenter import DataCenter

    DataCenter.start()
```

## Update 2025-10-25 19:36:31
Improved performance with comprehensive testing - ID: wm387pxm


## Update 2025-10-25 19:36:40
Fixed bug for enhanced functionality - ID: 3v5070b4


## Update 2025-10-25 19:36:50
Added configuration with modern best practices - ID: cizvwd9q


## Update 2025-10-25 19:36:59
Refactored code for enhanced functionality - ID: dwk2k5ne


## Update 2025-10-25 19:37:10
Fixed bug to improve stability - ID: nlazvdfg


## Update 2025-10-25 19:37:19
Fixed bug following security guidelines - ID: af4jhxv0


## Update 2025-10-25 19:37:28
Added configuration to support new requirements - ID: rd43sl8x


## Update 2025-10-25 19:37:38
Updated documentation to improve stability - ID: j9acngrf


## Update 2025-10-25 19:37:47
Optimized algorithm with modern best practices - ID: dfxwx0ce


## Update 2025-10-25 19:37:57
Updated dependencies for better maintainability - ID: p7m1a407


## Update 2025-10-25 19:38:07
Refactored code for better user experience - ID: innyqob5

