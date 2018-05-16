***文章持续更新中，欢迎star和issues***


![UITextField](https://github.com/SunshineBrother/SwiftTools/blob/master/GIF/UITextField.gif)
![UITextView](https://github.com/SunshineBrother/SwiftTools/blob/master/GIF/UITextView.gif)



# SwiftTools
技术不够，努力来凑；封装不了一个伟大的开源框架，但是仍然想要有一个自己的开源项目，所以就准备把一些项目中的常用工具类给封装出来，省的每一次写项目的时候都要重写一遍。
 
 
 ## UIKit
 
 ### UITextField
 ##### 方法
 |名称|说明|
 |---|:---:|
 |setPlaceHolderTextColor(_ color: UIColor)|设置placehold颜色|
 |distanceSides(_ leftWidth:CGFloat,_ rightWidth:CGFloat? = 0)|文本距离左右侧的距离|
 |addLeftIcon(_ image: UIImage,size:CGSize,padding: CGFloat)| 添加左侧icon|
 |addRightIcon(_ image: UIImage,size:CGSize,padding: CGFloat)|添加右侧icon|
|addLeftTile(titleLabel:UILabel,titleWidth:CGFloat,padding: CGFloat)|添加左侧标题|
 
 #### 属性
 |名称|说明|
 |---|:---:|
 |maxCount|最大数量|
|moneyType|输入金额类型|
|MobileType|手机号类型 手机号类型 普通的12345678901   344格式 123 4567 8901|

  ### UITextView
  #### 属性
  |名称|说明|
  |---|:---:|
  |tapTwiceDisapper| 点击两下键盘消失|
  |MaxCount|最大允许输入文本输入量|
  |placeHolder|设置placeHolder|
  |placeHolder|设置placeHolder的颜色|
 
 
## UIFoundation
### String扩展
#### 属性
|名称|说明|
|---|:---:|
|urlEncoded|URL编码|
|urlDecode|URL解码|
|base64|base64编码|
|base64Decode|Base64解码|
|isEmail|是否是邮箱|
|isValidUrl|是否是URL|
|isMobile|是否是手机号|
|isAlphanumeric|是否是字母数字的组合|
 
 ##### 方法
 |名称|说明|
 |---|:---:|
 |subStringFrom(index: Int,length:Int) -> String|字符串的截取|
 |substring(from: Int, to: Int) -> String|字符串的截取|
 |substring(from: Int?, to: Int?) -> String|字符串的截取|
 |substring(from: Int) -> String|字符串的截取|
 |substring(to: Int) -> String|字符串的截取|
 |stringByReplacingCharactersInRange(index:Int,length:Int,replacText:String) -> String |替换指定范围内的字符串|
 |stringByReplacingstringByReplacingString(text:String,replacText:String) -> String|替换指定字符串|
 |deleteEndCharacters() -> String|删除最后一个字符|
 |deleteString(string:String) -> String |删除指定字符串|
 |split(string:String) -> [String]|将字符串通过特定的字符串拆分为字符串数组|
 |toInt() -> Int?|变成Int 类型|
 |toDouble() -> Double?|变成Double 类型|
 |toFloat() -> Float?|变成Float 类型|
 |obtainTextHeight(font : UIFont = UIFont.systemFont(ofSize: 18), fixedWidth : CGFloat) -> CGFloat|获取文本高度|
 |obtainTextWidth(font : UIFont = UIFont.systemFont(ofSize: 17)) -> CGFloat|获取文本宽度|
 
### Array扩展
|名称|说明|
|---|:---:|
|removedDuplicates|删除  重复元素|

### Dictionary扩展
|名称|说明|
|---|:---:|
|addDictionary|拼接字典|
|has(key: Key) -> Bool|判断是否存在|
| removeAll(keys: [Key])|删除所有|
|jsonString(prettify: Bool = false) -> String?|Json字典转Json字符串|
|jsonData(prettify: Bool = false) -> Data?|Json字典转Data|
 
 
 ## 硬件
 关于硬件方面我分了一下几个方面
 - 1、各种权限获取，以及跳转的相应设置
 - 2、获取设备的一些信息
 - 3、判断手机上是否安装了某些应用
 - 4、开启一些设备
 
 ### 权限管理
 我们知道现在苹果越来越重视用户隐私了，几乎所有的涉及到用户的都需要我们进行权限申请
 这里我封装了一下几个功能
 - 1、各种权限判断，判断我们是否拥有权限
 - 2、跳转到相应地方开启权限
 

我们在进行权限判定的时候，可以调用这个方法
```
func isAllowService(type:LimitService_Type) -> Bool {}
```
 我们在开启设备的跳转的时候
 ```
 func TurnOnServeManager() {}
 ```
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 

























































