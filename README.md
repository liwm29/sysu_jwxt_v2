# sysu_jwxt_v2
- 登陆
![](Readme_staticFile/2020-08-15-14-15-30.png)
- 课程列表
![](Readme_staticFile/2020-08-15-15-06-59.png)
![](Readme_staticFile/2020-08-15-14-13-15.png)

---
## TODO:
- [ ] 改成 Lazy Load
  - 目前是鼠标hover到一行后加载那一行的教师信息和照片.
  - [x] fixme:移到下一行才刷新上一行的信息(使用this.$set())
- [ ] 选课
- [ ] 退课
- [ ] 选课 in loop
- [ ] ...
---
## BUG:
- 前端会请求 `/undefined`,原因可能是 `<img src="">` 空src属性导致
- ...

---
## 运行:
1. 下载本仓库,或git clone  
2. 直接鼠标双击打开 `main.exe` (最好使用shell:`./main`)
3. 打开网页: `localhost:9999`
---
## 编译
> 不清楚会不会遇到一些动态链接出错的问题,可能会缺少运行库,建议自己编译
- 下载按照 `golang `
- `go get` 按照第三方包
  - gin : `go get github.com/gin-gonic/gin`
  - goquery : `github.com/PuerkitoBio/goquery`
- `go build` (在当前文件目录下)
- `./main`