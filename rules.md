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
