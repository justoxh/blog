### PHP 闭包 （Closure）

### 闭包基本用法

闭包（Closure）又叫做匿名函数，很多语言都支持这种特性，比如像 JavaScript:

```
var add = (function () {
    var sum = 0;
    return function () {
        return sum += 1;
    }
})();
```

Golang:

```
func add() func(int) int {
	sum := 0
	return func(x int) int {
		return sum += x
	}
}

```

当然，PHP 也支持这种特性：

```

```

