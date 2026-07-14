# Collection Rules

## 1. Confirm Search Time

Before collecting any GitHub hot news data, record the search time to ensure the report reflects the latest available information.

Required metadata for every report:

- Time zone: Asia/Shanghai
- Search date: YYYY-MM-DD
- Search time: HH:mm
- Data range: latest available GitHub hot projects as of the search time

Recommended report header:

```markdown
检索时间：YYYY-MM-DD HH:mm Asia/Shanghai
数据范围：截至检索时间的 GitHub 最新热点资讯
```

## 2. Collect Daily GitHub Top 10 Projects

Collect the top 10 hottest GitHub projects of the day.

Primary source:

- GitHub Trending
- Time range: Today / Daily
- Count: Top 10 repositories

Each repository entry should include:

- Rank
- Repository name
- GitHub URL
- Description
- Primary language
- Total stars
- Stars gained today, if available
- Search time

Recommended report section:

```markdown
## 今日 GitHub 热门项目 Top 10

检索时间：YYYY-MM-DD HH:mm Asia/Shanghai
数据源：GitHub Trending - Daily

| 排名 | 项目 | 语言 | Star | 今日新增 | 简介 |
| --- | --- | --- | ---: | ---: | --- |
```

## 3. Generate And Store Daily Documents

After collecting the daily GitHub hot projects, organize the information into a Markdown report and store it in the local repository.

Required storage path:

```text
C:\Users\dalon\Desktop\Github热点收集\daily\YYYY-MM-DD.md
```

Example:

```text
C:\Users\dalon\Desktop\Github热点收集\daily\2026-07-14.md
```

Recommended document structure:

```markdown
# GitHub 热点资讯日报 - YYYY-MM-DD

检索时间：YYYY-MM-DD HH:mm Asia/Shanghai
数据范围：截至检索时间的 GitHub Trending Daily Top 10
数据源：GitHub Trending

## 今日 Top 10 项目

| 排名 | 项目 | 语言 | Star | 今日新增 | 简介 |
| --- | --- | --- | ---: | ---: | --- |

## 项目详情

### 1. owner/repo

- 链接：
- 简介：
- 主要语言：
- Star：
- 今日新增：
- 热点原因：
```
