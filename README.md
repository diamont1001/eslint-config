# jr-eslint-config #

ellint配置，个人前端代码检查规范

## 使用说明 ##
### 1. 插件安装 ###

```$
npm install eslint jr-eslint-config
```

### 2. 增加配置 ###

package.json增加脚本lint:
	
	// package.json
	"scripts": {
		"lint": "eslint *.js" // 配置要检查代码的文件/目录
	}

### 3. 检查代码 ###

开发完成后，一般打包或者发布前需要检查代码

```$
tnpm run lint
```

## 自定义规则 ##

如果想基于 `jr-eslint-config` 代码规范扩展自己的规则，可以在自己项目根目录下建立 `.eslintrc` 文件，并引入 `jr-eslint-config` 

	// .eslintrc
	{
		"extends": "jr-eslint-config",
		"rules": {
			// your rules here
		}
	}

