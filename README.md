# eslint-config-jr #

ellint配置，个人前端代码检查规范

## 使用说明 ##
### 1. 插件安装 ###

```$
npm install eslint eslint-config-jr
```

### 2. 建立配置文件 `.eslintrc` ##

项目根目录下建立 `.eslintrc` 文件，并引入 `eslint-config-jr` 

	// .eslintrc
	{
	    "extends": [
	    	"./node_modules/eslint-config-jr/.eslintrc"
	    ],
	    "rules": {
	        // your rules here
	    }
	}


### 3. 增加脚本 ###

package.json增加脚本lint:
	
	// package.json
	"scripts": {
		"lint": "./node_modules/.bin/eslint *.js" // 配置要检查代码的文件/目录
	}

### 4. 检查代码 ###

开发完成后，一般打包或者发布前需要检查代码

```$
npm run lint
```
