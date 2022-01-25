
## Getting started

flutter 版本的插件腾讯cos插件,不依赖原生插件.参考:https://cloud.tencent.com/document/product/436/7749
如果可以麻烦右上角给点个like吧

## Usage

```dart
//如果后台采用临时秘钥这里需要传入值,不然403错误,如果永久秘钥写在客户端,token可以不传入
String token = "";
//本地的file
String localPath = "";
//cos路径
String cosPath = "abc/123.png";
await COSClient(COSConfig(
credentials["secretId"],
credentials["secretKey"],
credentials["bucketName"],
credentials["region"],
)).putObject(cosPath, localPath, token: token);
```

## Additional information

具体参考:https://cloud.tencent.com/developer/article/1878729
