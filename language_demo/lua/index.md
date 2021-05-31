# Lua tutorial

## Hello World

```lua
print('hello world')

-- 或者

print 'hello world!'
```

## Data Type

> Lua是一种动态类型语言，因此语言中没有类型的定义，不需要声明变量类型，每个变量自己保存了类型。

> 有8种基本类型：

- nil
- 布尔值（boolean）
- 数字体（number）
- 字符串型（string）
- 用户自定义类型（userdata）
- 函数（function）
- 线程（thread）和表（table）。

```lua
-- string
print(type("string"))
print(type(type(1)))

-- number
print(type(1))

-- table
print(type({}))

-- boolean
print(type(true))

-- function
print(type(print))
print(type(type))

-- nil
print(type(nil))
```

*表格*


## function

```lua
function factorial(n)
  local x = 1
  for i = 2, n do
    x = x * i
  end
  return x
end
```


## The control flow

```lua
-- condition = true

while condition do
    -- statements
end


repeat
    -- statements
until condition


for i = first, last, delta do
    -- statements
    -- example: print(i)
end

-- 通用 for 循环

for key, value in pairs(_G) do
    print(key, value)
end
```
