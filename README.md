打开官网 https://www.backblaze.com ,点击Get Started → Try for Free

接着输入邮箱, 点击Get Started Free

1
接着进入邮箱, 验证邮箱, 验证完成后, 填入密码并选择地区, 任意一个即可

2
点击Create Account, 接着输入账号密码登陆

创建私有桶和密钥
点击创建一个桶, 输入桶的名字, 其他默认, 点击创建

3
将桶的名字和Endpoint复制下来, 等会要用

4
接着进入Application Keys, 点击Add a NewApplication Keys创建密钥

5
名字随便, 其他默认点击创建, 复制KeyID和applicationKey(一定要保存好, 不要丢失或泄露)

6
创建CF Pages
点击链接下载压缩包b2.zip

登陆Cloudflare, 选择Workers和Pages, 点击创建

7
选择Pages, 选择直接上传, 输入项目名字后将 b2.zip 上传

8
点击部署站点

接着点击设置 → 添加变量

9
类型选择纯文本

变量名	值
ALLOW_LIST_BUCKET	flase
BUCKET_NAME	你的存储桶的名字
B2_ENDPOINT	你的地区的endpoint如 s3.ca-east-006.backblazeb2.com
B2_APPLICATION_KEY_ID	你复制的KeyID
B2_APPLICATION_KEY	你复制的applicationKey
点击保存

在设置的横栏里左滑, 点击创建部署(狗石布局, 害得我一开始找了半天没找到)

10
再次将 b2.zip 上传, 点击部署即可

点击自定义域, 设置自定义域, 输入自己的自定义域名, 接着选择我的dns提供商, 然后到自己的域名解析处, 设置CNAME解析

如果是Cloudflare解析,必须关闭小黄云

11
下载PicGO的魔改版

桌面端: PicList

手机端: PicHoro

根据图示配置, 以手机为例

12
之后检查配置没有问题后, 设置为默认图床即可使用
