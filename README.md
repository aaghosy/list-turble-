# list-turble-
`list`（列表）和 `tuple`（元组）是Python中两种不同的序列（sequence）数据类型，它们之间有以下主要区别：

1. **可变性**：
   - `list`：列表是可变的，意味着你可以添加、删除或修改列表中的元素。
   - `tuple`：元组是不可变的，一旦创建，就不能添加、删除或修改元组中的元素。元组更像是一个不可变的列表。

2. **声明方式**：
   - `list`：列表使用方括号 `[]` 来创建，元素之间用逗号 `,` 分隔，例如 `[1, 2, 3]`。
   - `tuple`：元组使用圆括号 `()` 来创建，元素之间也用逗号 `,` 分隔，例如 `(1, 2, 3)`。注意，即使没有括号，只有逗号的情况也会创建元组，例如 `1, 2, 3` 也是一个元组。

3. **性能**：
   - 由于元组是不可变的，因此在某些情况下比列表更快，特别是在迭代元素时。

4. **用途**：
   - `list`：通常用于存储一组元素，这组元素可以动态增加或减少，适合用于需要频繁修改数据的情况。
   - `tuple`：通常用于存储一组元素，这组元素不应该被修改，适合用于表示不可变的数据，如坐标、日期时间等。

示例：
```python
my_list = [1, 2, 3]    # 创建一个列表
my_tuple = (1, 2, 3)  # 创建一个元组

# 修改列表中的元素
my_list[0] = 4
# my_list 现在是 [4, 2, 3]

# 尝试修改元组中的元素会引发错误
# 以下代码会引发 TypeError
# my_tuple[0] = 4
```

