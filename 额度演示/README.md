# 信用卡额度结构演示工具

### English | [中文](#中文)

Credit Card Limit Structure Demonstration Tool

## Overview

An interactive visualization tool for simulating credit card limit usage logic, particularly focusing on installment and consumption transactions.

## Features

- **Four Core Limit Nodes**: Comprehensive overview of credit limits (07), consumption limits (01), installment limits (03), and exclusive installment limits (13)
- **Consumption Transactions**: Add consumption and占用 01 and 07 nodes
- **Installment Transactions**: Add installment with priority on 13 node, then 01 node
- **Paochang (抛帐)**: Up to 2 times, first time 50%, second time remaining full amount
- **Tuihuo (退货)**: Once only, cannot tuihuo after paochang
- **Repayment**: Restore 01 and 07 node limits

## Limit Formulas

| Formula | Description |
|---------|-------------|
| `03 = 01 + 13` | Installment limit = Consumption + Exclusive Installment |
| `01 ≤ 07` | Consumption ≤ Comprehensive |
| `03 ≤ 07` | Installment ≤ Comprehensive |

## Usage

1. Open `信用卡额度结构演示工具.html` in a web browser
2. Click "Reset All" to unlock limit editing
3. Configure initial limits and click "Save Configuration"
4. Add transactions as needed

## Color Coding

| Node | Color | Description |
|------|-------|-------------|
| 01 | Blue | Consumption Limit |
| 03 | Purple | Installment Limit |
| 13 | Green | Exclusive Installment |
| 07 | Gold | Comprehensive Limit |

---

# 信用卡额度结构演示工具

## 概述

一个交互式可视化工具，用于模拟信用卡额度使用逻辑，特别关注分期和消费交易的额度占用。

## 功能特点

- **四个核心额度节点**：综授额度(07)、消费额度(01)、分期额度(03)、分期独享额度(13)
- **消费交易**：添加消费，占用01和07节点
- **分期交易**：添加分期，优先占用13节点，不够时使用01节点
- **抛帐**：最多2次，第一次抛出50%，第二次抛出剩余全部
- **退货**：仅1次，抛帐后不可退货
- **还款**：恢复01和07节点额度

## 额度公式

| 公式 | 说明 |
|------|------|
| `03 = 01 + 13` | 分期额度 = 消费额度 + 分期独享额度 |
| `01 ≤ 07` | 消费额度 ≤ 综授额度 |
| `03 ≤ 07` | 分期额度 ≤ 综授额度 |

## 使用方法

1. 在浏览器中打开 `信用卡额度结构演示工具.html`
2. 点击"重置所有"解锁额度编辑
3. 配置初始额度并点击"保存配置"
4. 根据需要添加交易

## 颜色编码

| 节点 | 颜色 | 说明 |
|------|------|------|
| 01 | 蓝色 | 消费额度 |
| 03 | 紫色 | 分期额度 |
| 13 | 绿色 | 分期独享额度 |
| 07 | 金色 | 综授额度 |

## 许可证

MIT License
