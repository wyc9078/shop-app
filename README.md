## shop-bend


后端的api接口，**nodejs + mysql + express + redis + rsa** 实现

## shop-fend

Vue2.x实现的前端app页面

## RSA 非对称加密api设计思路

私钥   公钥


- 1：前端传递参数给后端的时候，先将数据 object 转换为 "key=value&key=value" ，然后通过私钥对数据进行加密，放到请求头中token传递给后端，

- 2：后端拿到请求头通过公钥解密，重新排列数据为 object， 然后查询计算完成拿到数据，后端再用公钥加密json数据，然后返回给前端

- 3：前端通过私钥解密后端的json，渲染页面

暂时保存！！
