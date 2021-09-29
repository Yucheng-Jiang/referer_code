# referer_code

This repo contains daily referer code scrapped from [nowcoder website](https://www.nowcoder.com/). Script will automatically push daily csv file into this repo at midnight (GMT -5 timezone)

## Schema

`id`: Nowcoder website post identification number, can use it to access original article `https://www.nowcoder.com/discuss/{id}`

`code`: referer code

`info`: key links in original post. Links are classfied into 5 categories `[内推链接, 投递, 流程, 社招链接, 更多详情]`

`tag`: tags of original post created by author

`time`: epoch time

## TODO list
- Train model to create more precise tags
- Rotate ip, headers, fingerprint, and cookies
- Crawl more posts in nowcoder and leetcode
- Optimize multi thread crawling
