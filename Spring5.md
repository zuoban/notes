## Spel表达式
### Bean引用 
可以使用@符号从表达式中查找 bean  如`@foo`
如果要访问一个工厂 bean 向身，则需要使用&符号 如`&foo`

### Elvis 运算符
`name ?: 'Unknown'` 等价于 `name != null ? name : ''Unknown"`

### 安全导航运算符 
避免 NullPointerException, 如`#{PlaceOfBirth?.City}`

### 集合选择 
.?[selectionExpression] 如 #{its.?[weight lt 3.5]} 
### 集合投影
#{its.![good]}
