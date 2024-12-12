## 专项练习-Linq集成查询和Lambda表达式


##### 基础练习

1. **查询特定元素**
   找出数组中等于5的元素。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6 };
   ```

2. **查询特定范围的元素**
   找出数组中在2到8之间的元素。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6 };
   ```

3. **查询并转换元素**
   将数组中的每个数字乘以2。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6 };
   ```

4. **查询特定属性的对象**
   找出所有名字以"王"开头的学生。

   ```csharp
   List<Student> students = new List<Student>
   {
       new Student {Id=1, Name = "王有才", Age = 21 },
       new Student {Id=2,  Name = "王中王", Age = 22 },
       new Student {Id=3,  Name = "张语嫣", Age = 23 },
       new Student {Id=4,  Name = "詹宇航", Age = 35 },
       new Student {Id=5,  Name = "郑雨良", Age = 26 },
   };
   ```

5. **查询并排序**
   找出所有年龄大于20岁的学生，并按年龄降序排列。

   ```csharp
      List<Student> students = new List<Student>
   {
       new Student {Id=1, Name = "王有才", Age = 21 },
       new Student {Id=2, Name = "罗婷", Age = 21 },
       new Student {Id=3,  Name = "王中王", Age = 22 },
       new Student {Id=4,  Name = "李子柒", Age = 22 },
       new Student {Id=5,  Name = "张语嫣", Age = 23 },
       new Student {Id=6,  Name = "詹宇航", Age = 35 },
       new Student {Id=7,  Name = "郑雨良", Age = 26 },
       new Student {Id=8,  Name = "欧文", Age = 26 },
   };
   ```

6. **查询并去重**
   找出数组中所有不重复的数字。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
   ```

7. **查询第一个元素**
   找出数组中第一个大于3的元素。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
   ```

8. **查询最后一个元素**
   找出数组中最后一个小于7的元素。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
   ```

9. **查询元素是否存在**
   检查数组中是否存在大于10的元素。

   ```csharp
   int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
   ```

10. **查询元素的计数**
    计算数组中大于5的元素数量。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

11. **查询元素的总和**
    计算数组中所有元素的总和。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

12. **查询元素的最大值**
    找出数组中的最大值。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

13. **查询元素的最小值**
    找出数组中的最小值。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

14. **查询元素的平均值**
    计算数组中所有元素的平均值。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

15. **查询特定条件的元素**
    找出数组中能被3整除的元素。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

##### 中级练习

16. **查询并选择特定属性**
    找出所有学生的姓名和年龄。

    ```csharp
    List<Student> students = new List<Student>
    {
        new Student {Id=1, Name = "王有才", Age = 21 },
        new Student {Id=2, Name = "罗婷", Age = 21 },
        new Student {Id=3,  Name = "王中王", Age = 22 },
        new Student {Id=4,  Name = "李子柒", Age = 22 },
        new Student {Id=5,  Name = "张语嫣", Age = 23 },
        new Student {Id=6,  Name = "詹宇航", Age = 35 },
        new Student {Id=7,  Name = "郑雨良", Age = 26 },
        new Student {Id=8,  Name = "欧文", Age = 26 },
    };
    ```

17. **查询并分组**
    按年龄分组学生，并计算每个年龄组的学生数量。

    ```csharp
    List<Student> students = new List<Student>
    {
        new Student {Id=1, Name = "王有才", Age = 21 },
        new Student {Id=2, Name = "罗婷", Age = 21 },
        new Student {Id=3,  Name = "王中王", Age = 22 },
        new Student {Id=4,  Name = "李子柒", Age = 22 },
        new Student {Id=5,  Name = "张语嫣", Age = 23 },
        new Student {Id=6,  Name = "詹宇航", Age = 35 },
        new Student {Id=7,  Name = "郑雨良", Age = 26 },
        new Student {Id=8,  Name = "欧文", Age = 26 },
    };
    ```

18. **查询并联结**
    联结学生和课程表，找出每个学生的所有课程。

    ```csharp
    List<Student> students = new List<Student>
    {
        new Student {Id=1, Name = "王有才", Age = 21 },
        new Student {Id=2, Name = "罗婷", Age = 21 },
        new Student {Id=3,  Name = "王中王", Age = 22 },
        new Student {Id=4,  Name = "李子柒", Age = 22 },
        new Student {Id=5,  Name = "张语嫣", Age = 23 },
        new Student {Id=6,  Name = "詹宇航", Age = 35 },
        new Student {Id=7,  Name = "郑雨良", Age = 26 },
        new Student {Id=8,  Name = "欧文", Age = 26 },
    };
    List<Course> courses=new List<Course>
    {
            new Course{StudentId=1,CourseName="英语"},
            new Course{StudentId=1,CourseName="数学"},
            new Course{StudentId=2,CourseName="语文"},
            new Course{StudentId=3,CourseName="物理"},
            new Course{StudentId=4,CourseName="化学"},
            new Course{StudentId=4,CourseName="生物"},
            new Course{StudentId=4,CourseName="语文"},
    };
    ```

19. **查询并反转**
    反转数组中的元素顺序。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

20. **查询并填充**
    找出数组中第一个大于2的元素，并用它填充后面的所有位置。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

21. **查询并排除**
    从数组中排除所有小于5的元素。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

22. **查询并填充默认值**
    如果数组中存在null值，用默认值0替换。

    ```csharp
    int?[] nullableNumbers = { 1, null, 3, null, 5 };
    ```

23. **查询并转换类型**
    将字符串数组转换为整数数组。

    ```csharp
    string[] stringNumbers = { "1", "2", "3", "4" };
    ```


24. **查询并使用OfType过滤**
    从对象数组中过滤出字符串类型的元素。

    ```csharp
    object[] objects = { "String", 123, "Another String", 456 };
    var result = objects.OfType<string>().ToList();
    ```

##### 高级练习

25. **查询并使用Zip合并**
    合并两个数组，并创建一个包含元素对的新数组。

    ```csharp
    int[] numbers1 = { 1, 2, 3 };
    int[] numbers2 = { 4, 5, 6 };
    ```

26. **查询并使用Range生成**
    生成一个包含1到10的整数数组。

    ```csharp
    ```

27. **查询并使用Repeat重复**
    重复一个元素多次，创建一个新数组。

    ```csharp
    ```

28. **查询并使用Take限制数量**
    从数组中取出前5个元素。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```

29. **查询并使用Skip跳过元素**
    跳过数组中的前3个元素，然后取出剩余的元素。

    ```csharp
    int[] numbers = { 1, 2, 3, 4, 5, 6,18,23,64,7,18,2,3 };
    ```
