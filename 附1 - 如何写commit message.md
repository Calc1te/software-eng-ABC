**一个良好的commit message有助于让其他人在接手工作时了解你的进度**
### 格式规范

Commit Message 应包含以下三个部分：

1. **标题 (Header)**:  简明扼要地描述本次提交的内容，不超过 50 个字符。
    * 使用英文动词开头，使用一般现在时
    * 首字母大写，句尾不加标点符号。
    * 例如：`Fix login page layout issue`

2. **正文 (Body)**:  可选部分，详细描述本次提交的内容，说明代码变更的原因、动机以及实现方式。
    * 每行不超过 72 个字符。
    * 使用英文书写，语法正确，表达清晰。
    * 可以分段落描述，使用空行分隔。
    * 例如：
        ```
        The login page layout was broken on mobile devices due to incorrect CSS media queries.
        This commit fixes the issue by adjusting the media queries and updating the styles.
        ```

3. **页脚 (Footer)**:  可选部分，用于关联 issue、PR 等信息。
    * 使用 `Closes`, `Fixes`, `Resolves` 等关键词关联 issue。
    * 例如：`Closes #123`

### 类型说明

使用以下类型前缀对提交进行分类：

* **feat**:  新功能
* **fix**:  修复 bug
* **docs**:  文档更新
* **style**:  代码格式调整（不影响代码逻辑）
* **refactor**:  代码重构（不改变代码功能）
* **perf**:  性能优化
* **test**:  测试代码更新
* **chore**:  构建过程或辅助工具的变动

### 示例

```
feat: Add user authentication

- Add login and registration forms
- Implement user authentication logic
- Store user data in database

Closes #123
```

```
fix: Fix broken image links on homepage

- Update image paths to use relative URLs
- Add alt text to all images

Fixes #456
```

```
refactor: Simplify login form validation

- Remove redundant validation rules
- Use built-in HTML5 validation attributes
```


### **其他建议**

* 保持 Commit Message 简洁明了，避免使用模糊不清的语言。
* 每次提交只做一件事，避免将多个不相关的更改放在一次提交中。
* 在提交代码前，仔细检查 Commit Message 是否符合规范。

**参考**

* [Conventional Commits](https://www.conventionalcommits.org/)
* [Angular Commit Message Guidelines](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#commit)