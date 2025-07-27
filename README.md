# cursor 使用方法


## 在Cursor中复现Kiro Spec工作流

## 自定义Agent配置

Cursor通过自定义Agent功能可以完美复现Kiro Spec工作流。配置方法：
1. **创建Kiro Agent**
2. 在Cursor设置中添加新的自定义Agent
3. 将完整的Kiro工作流程提示词配置为Agent的系统提示
4. 设置Agent名称为"kiro_workflow"      
5. **Agent调用方式**`@kiro_workflow 我想做一个用户登录功能`      
6. **工作流程自动化**      
7. Agent会自动识别当前项目状态
8. 检查`.kiro/specs/`目录确定当前阶段
9. 智能导航到合适的工作阶段
10. 与用户进行自然语言交互确认推进

## Cursor中的优势

- **上下文感知**：Agent能够访问整个项目代码库
- **文件管理**：自动创建和管理规格文档
- **实时协作**：在代码编辑过程中提供持续指导
- **集成开发**：与Cursor的其他功能无缝集成


# claude code 使用方法

## 自定义Command配置

Claude Code通过自定义Command功能实现Kiro Spec工作流的复现：

1. **创建Command文件**
2. 在用户目录下创建`.claude/commands/`文件夹
3. 将kiro_workflow.md配置为自定义command
4. 文件命名为`kiro_workflow.md`  
    
5. **Command调用方式**`bash /kiro_workflow 我想做一个用户登录功能`  
    
6. **工作流程执行**  
    
7. Command会自动加载完整的工作流程逻辑
8. 通过文件检查确定当前阶段
9. 提供阶段引导和自然推进确认

## Claude Code中的特色功能

- **终端集成**：直接在命令行中执行工作流程
- **项目感知**：自动识别项目类型和技术栈
- **文档生成**：自动生成和更新规格文档
- **版本控制**：与Git工作流程无缝集成

## 配置示例

```text
---
description: Kiro统一工作流程 - 完整的中文版特性开发流程，从想法到代码实现
argument-hint: [功能名称或想法描述]
---

# Kiro工作流程

您好！我是Kiro，您的AI开发助手...
[包含完整的工作流程配置]
```


# 参考文章

https://zhuanlan.zhihu.com/p/1931026753767338132