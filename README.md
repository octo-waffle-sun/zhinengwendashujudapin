[README.md](https://github.com/user-attachments/files/26452475/README.md)
# 供应链采购智慧监控数据大屏

## 项目简介

这是一个基于React + TypeScript + ECharts开发的数据大屏项目，专注于供应链采购智慧监控。系统采用现代化的深蓝色科技风格UI设计，提供实时数据展示和智能预警功能。

## 功能特性

### 核心数据模块

1. **供应商情况监控**
   - 历史累计参与供应商数量
   - 近一年新增供应商统计
   - 供应商质量评估

2. **采购效率分析**
   - 平均采购周期
   - 平均审批时间
   - 合同采购周期完成率

3. **智慧预警中心**
   - 设备关系预警
   - 失信信息监控
   - 严重违法行为告警
   - 行政处罚提醒
   - 税收违法预警

4. **合同管理**
   - 入库订单统计
   - 出库订单跟踪
   - 配送及时率监控

5. **物资采购分析**
   - 采购频次TOP5排行
   - 采购金额趋势
   - 供应商绩效对比

6. **项目进度跟踪**
   - 多维度项目进度展示
   - 合同执行进度
   - 异常项目占比分析

## 技术架构

- **前端框架**: React 18 + TypeScript
- **图表库**: Apache ECharts 5.4+
- **样式方案**: Styled-Components
- **动画效果**: Framer Motion
- **构建工具**: Vite
- **开发语言**: TypeScript

## 安装与使用

### 环境要求
- Node.js >= 16.0.0
- npm >= 8.0.0 或 yarn >= 1.22.0

### 安装依赖
```bash
npm install
# 或
yarn install
```

### 启动开发服务器
```bash
npm run dev
# 或
yarn dev
```

### 构建生产版本
```bash
npm run build
# 或
yarn build
```

### 预览生产版本
```bash
npm run preview
# 或
yarn preview
```

## 项目结构

```
src/
├── components/          # 组件目录
│   ├── Dashboard/      # 主仪表板组件
│   ├── Charts/         # 图表组件
│   │   ├── BarChart/   # 柱状图
│   │   ├── PieChart/   # 饼图
│   │   ├── LineChart/  # 折线图
│   │   └── GaugeChart/ # 仪表盘
│   └── Layout/         # 布局组件
├── data/               # 模拟数据
├── styles/             # 样式文件
├── utils/              # 工具函数
├── types/              # TypeScript 类型定义
└── App.tsx            # 应用入口
```

## 核心配置参数

### 主题配置
```typescript
const theme = {
  colors: {
    primary: '#1890ff',
    secondary: '#722ed1',
    success: '#52c41a',
    warning: '#faad14',
    error: '#f5222d',
    background: '#0f1419',
    cardBackground: 'rgba(24, 144, 255, 0.1)'
  }
}
```

### 图表配置
```typescript
const chartConfig = {
  animation: true,
  animationDuration: 2000,
  backgroundColor: 'transparent',
  grid: {
    left: '3%',
    right: '4%',
    bottom: '3%',
    containLabel: true
  }
}
```

## 数据接口

系统支持实时数据更新，可通过以下接口集成：

- `/api/suppliers` - 供应商数据
- `/api/procurement` - 采购数据  
- `/api/contracts` - 合同数据
- `/api/alerts` - 预警数据
- `/api/materials` - 物资数据
- `/api/projects` - 项目数据

## 浏览器支持

- Chrome >= 88
- Firefox >= 85
- Safari >= 14
- Edge >= 88

## 性能优化

- 组件懒加载
- 图表按需渲染
- 数据缓存机制
- 防抖节流优化

## 开发团队

本项目由经验丰富的产品经理与软件开发专家团队开发，专注于高质量代码和优异的用户体验。

## 许可证

MIT License 
