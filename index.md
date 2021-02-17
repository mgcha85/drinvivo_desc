file header
| index | value | description | note |
| --- |  --- |  --- |  --- | 
| 0 | 0x01 or 0x0F | header (1 byte) | - |
| 1 | null | body (from here) | - |
| 2 | filesize | - | - |
| 3 | null | - | - |
| 4 | sensor type | dispenser, short_time, vacuum_time, interval_time, shot_pressure, vacuum_pressure, real_temperature, set_temperature, set_pid (0x30, …, 0x38) | pid만 string 그외 short (2 |
| 5 | currentCH | dispenser case | - |
| 6 | currentMode | dispenser case | - |
| 7 | currentStatus | dispenser case | - |
| ... | 4가 dispenser가 아닌 경우 5 부터 쭉 해당 값 (short_time, vacuum_time, ..., or set_pid) | - |






## Alarm
Phone_control_activity.kt: wifi communication을 통해 신호를 받아들임 (alram thread를 돌면서 alarm도 모니터링 (5초 마다))
Phone_main_activity.kt: 상동 + 메인 리스트를 parsing


## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/mgcha85/drinvivo_desc/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/mgcha85/drinvivo_desc/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
