# Typescript에서 기본 디렉터리 설정

js에서는 ```package.json```에 다음과 같이 설정하여 src디렉터리를 기본 디렉터리로 설정한다.

```
{
	...
	"scripts" : {
		"start" : "NODE_PATH=src react-scripts start",
		"build" : "NODE_PATH=src react-scripts build",
		...
	}
}
```



그러나 tsx에서는 ```tsconfig.json```에서 설정해야한다.

```
{
	"compilerOptions": {
		...
		"baseUrl": "./src"
	}
	...
}
```



