# algorithm_achieve_composer
把所有面试中的算法。都一一实现。形成一个Library。最好成为SPL。不过不大可能实现。先可以通过Composer引进吧

首先 PHP SPL 中已经存在一些基础的东西。  
我可以在其基础上实现。这些东西。  
PHP语言，可以让我们工作，但是应该也可以让我们面试。

项目位置： https://github.com/peng456/composer_algorithm


1、学会如何用 composer 引入github 上代码。 

1、composer 的学习 参考： https://www.jianshu.com/p/5954fe55d067

GitHub是一个用于使用Git版本控制系统项目的共享虚拟主机服务，可以免费托管公开的源代码仓库。

Composer
PHP中的一个依赖管理工具， 它可以让你声明自己项目所依赖的库，然后它将会在项目中为你安装这些库，

Packagist 是Composer默认的中央仓库
PHP社区的绝大部分Composer包都托管在该网站上。Packagist提供公开的、免费的托管服务，任何人均可注册、自由发布包，无需审核。


1、Composer 的原理。就是自动 到  https://packagist.org  下载对应的包

2、通过GitHub 发布原理
	github 上的更新 会通知到 Packagist。Packagist，会更新内容。


1、准备需要提前准备： GitHub帐号、Composer程序、Packagist帐号


时间消耗在两个地方   
1、github hook 触发Packagist 更新问题。  
2、Composer 使用上。
   如果你只是引入一个包。那么你必须自己 写 composer.json  并且 初始化它（Composer install ）

Package name   包名  
Description  描述    
Minimum Stability    
Package Type  类别 （库、项目、metapackage、composer-plugin 等）  
License  开放许可  
dependencies(require)   依赖包，这些包会被放到vendor 里面。并被autoload 自动识别    
dev dependencies (require-dev)  开发依赖  
version   版本  



引入包  
1、composer require peng4546/algorithm(前提是 你已经初始化了)  
2、在composer.json  的require  中写清你要引入的包


创建项目：  
composer create-project --prefer-dist laravel/laravel blog

