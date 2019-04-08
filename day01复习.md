### 爬虫的概念
  - 模拟浏览器发送请求，获取响应

### 爬虫的流程
  -  url---》发送请求，获取响应---》提取数据---》保存
  - 发送请求，获取响应---》提取url（下一页，详情页）重新请求


### 爬虫要根据当前url地址对应的响应为准
  - 爬虫只会请求当前这个url，但是不是请求js，
  - 浏览器拿到的内容，我们在浏览器中看到的内容是elements里面的内容
  - elements=url对应的响应+js+css+图片


### requests模块如何发送请求
  - resposne = requests.get(url)

### requests中解决编解码的方法
  - response.content.decode()
  - response.content.decode("gbk")
  - response.text
