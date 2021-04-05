### install
https://github.com/jasongin/nvs/blob/master/doc/SETUP.md
PowerShell
```PowerShell
$env:NVS_HOME="$env:ProgramData\nvs"
git clone https://github.com/jasongin/nvs "$env:NVS_HOME"
. "$env:NVS_HOME\nvs.ps1" install
```

### Add mirror
```PowerShell
nvs remote <Name> <URL>
```

```
default             node
chakracore          https://github.com/nodejs/node-chakracore/releases/
chakracore-nightly  https://nodejs.org/download/chakracore-nightly/
nightly             https://nodejs.org/download/nightly/
node                https://nodejs.org/dist/
```

```PowerShell
nvs remote chakracore https://github.com/nodejs/node-chakracore/releases/
nvs remote chakracore-nightly https://nodejs.org/download/chakracore-nightly/
nvs remote nightly https://nodejs.org/download/nightly/
nvs remote node https://nodejs.org/dist/
```

### Add node version
```PowerShell
# 安装最新的 LTS 版本
nvs add lts
```

```PowerShell
# 配置为默认版本
nvs link <version>
```

```PowerShell
# 安装其他版本尝尝鲜
nvs add 12

# 查看已安装的版本
nvs ls

# 在当前 Shell 切换版本
nvs use 12
```

### help
```PowerShell
nvs --help
```
