# hardhat-quickstart

Hardhat 是一个非常流行的以太坊开发框架，主要用于智能合约的开发、部署和测试。它提供了一套丰富的工具和API，帮助开发者在Ethereum虚拟机（EVM）环境中高效工作。以下是一些Hardhat常用的API：

1. **部署和任务系统**
   - `task(name, description, action)`: 定义一个Hardhat任务，可以通过命令行调用。
   - `deploy()`: 用于部署智能合约。

2. **网络配置**
   - `network.name`: 获取当前网络名称。
   - `network.provider`: 获取当前网络的提供者对象，用于发送EVM JSON-RPC请求。

3. **合约交互**
   - `ethers.getContractFactory(name)`: 获取合约工厂，用于部署新的合约实例或连接到现有的合约。
   - `ethers.getContractAt(name, address)`: 连接到部署在特定地址的合约。

4. **测试和验证**
   - `ethers.provider`: 提供一个Ethers.js的provider，可以用于低级的区块链交互和状态查询。
   - `artifacts.require(name)`: 加载编译后的合约数据，通常用于测试。

5. **环境变量和配置**
   - `config`: 访问Hardhat的配置参数，如网络设置、路径等。
   - `env`: 用于访问由Hardhat或插件设置的环境变量。

6. **日志和错误处理**
   - `log(message)`: 打印日志信息到控制台。
   - `subtask(name, action)`: 定义一个可以被其他任务调用的子任务。

Hardhat 也支持通过插件扩展其功能，例如用于合约验证的`hardhat-etherscan`或用于安全性分析的`hardhat-prettier`等。每个插件可能提供特有的API，用于增强开发和测试的便利性。

