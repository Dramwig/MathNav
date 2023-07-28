# 更新记录

2023/07/27

- 基于MKdocs，使用material主题建立起了本地站点命名为MathNav
- 绘制了网站favition与logo
- 插件配置如下

    ```yml
    markdown_extensions:
      - admonition  # 提示块
      - footnotes  # 脚注
      - meta  # 定义元数据，通过文章上下文控制，如disqus
      - pymdownx.caret  # 下划线上标
      - pymdownx.tilde  # 删除线下标
      - pymdownx.critic  # 增加删除修改高亮注释，可修饰行内或段落
      - pymdownx.details  # 提示块可折叠
      - pymdownx.inlinehilite  # 行内代码高亮
      - pymdownx.mark  # 文本高亮
      - pymdownx.smartsymbols  # 符号转换
      - pymdownx.superfences  # 代码嵌套在列表里
      - pymdownx.details
      - pymdownx.tasklist
      - pymdownx.emoji
      - pymdownx.arithmatex:
          generic: true
      - codehilite:    # 代码高亮，显示行号
          guess_lang: false
          linenums: true
      - toc: 
          permalink: true
      - pymdownx.betterem:  # 对加粗和斜体更好的检测
          smart_enable: all
      - pymdownx.emoji:  # 表情
          emoji_generator: !!python/name:pymdownx.emoji.to_svg
      - pymdownx.magiclink  # 自动识别超链接
      - pymdownx.tasklist:  # 复选框checklist
          custom_checkbox: true
    plugins:
      - search
    extra_javascript:
      - https://polyfill.io/v3/polyfill.min.js?features=es6
      - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js
    
    ```

