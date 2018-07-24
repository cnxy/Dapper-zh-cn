#### 本文翻译自：[StackExchange.Dapper](https://github.com/StackExchange/Dapper)
#### 原版教程源自：[Dapper Tutorial](http://dapper-tutorial.net/dapper)
#### 中文教程源自：[中文Dapper教程.GitBook](https://legacy.gitbook.com/book/esofar/dapper-tutorial-cn/details)
#### 中文教程PDF：[dapper-tutorial-cn](https://github.com/cnxy/Dapper-zh-cn/blob/master/dapper-tutorial-cn.pdf)

Dapper - .Net版本的简单对象映射器
========================================
[![Build status](https://ci.appveyor.com/api/projects/status/8rbgoxqio76ynj4h?svg=true)](https://ci.appveyor.com/project/StackExchange/dapper)

发行说明
-------------
请见 [stackexchange.github.io/Dapper](https://stackexchange.github.io/Dapper/)

组件
--------

MyGet 预发行 feed: https://www.myget.org/gallery/dapper

|   组件  | NuGet稳定版 |    NuGet预发行版 | 下载 | MyGet |
| ------- | -------------- | ------------------- | ----------- | ------- |
| [Dapper](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/v/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/vpre/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/dt/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper) |
| [Dapper.Contrib](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/v/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/vpre/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/dt/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.Contrib.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.Contrib) |
| [Dapper.EntityFramework](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/v/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/vpre/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/dt/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.EntityFramework.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.EntityFramework) |
| [Dapper.EntityFramework.StrongName](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/v/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/vpre/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/dt/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.EntityFramework.StrongName.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.EntityFramework.StrongName) |
| [Dapper.Rainbow](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/v/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/vpre/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/dt/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.Rainbow.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.Rainbow) |
| [Dapper.SqlBuilder](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/v/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/vpre/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/dt/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.SqlBuilder.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.SqlBuilder) |
| [Dapper.StrongName](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/v/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/vpre/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/dt/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.StrongName.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.StrongName) |

特点
--------
Dapper是一个[NuGet库](https://www.nuget.org/packages/Dapper)，您可以将其添加到项目中，以扩展您的`IDbConnection`接口。

它提供了3个使用方法：

执行一个查询并将结果映射到强类型列表
------------------------------------------------------------

```csharp
public static IEnumerable<T> Query<T>(this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null, bool buffered = true)
```
示例：

```csharp
public class Dog
{
    public int? Age { get; set; }
    public Guid Id { get; set; }
    public string Name { get; set; }
    public float? Weight { get; set; }

    public int IgnoredProperty { get { return 1; } }
}

var guid = Guid.NewGuid();
var dog = connection.Query<Dog>("select Age = @Age, Id = @Id", new { Age = (int?)null, Id = guid });

Assert.Equal(1,dog.Count());
Assert.Null(dog.First().Age);
Assert.Equal(guid, dog.First().Id);
```

执行一个查询并将其映射到动态对象列表
-------------------------------------------------------

```csharp
public static IEnumerable<dynamic> Query (this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null, bool buffered = true)
```
这个方法会执行SQL语句，并返回一个动态列表。

示例：

```csharp
var rows = connection.Query("select 1 A, 2 B union all select 3, 4");

Assert.Equal(1, (int)rows[0].A);
Assert.Equal(2, (int)rows[0].B);
Assert.Equal(3, (int)rows[1].A);
Assert.Equal(4, (int)rows[1].B);
```

执行不返回结果的命令
-----------------------------------------

```csharp
public static int Execute(this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null)
```

示例：

```csharp
var count = connection.Execute(@"
  set nocount on
  create table #t(i int)
  set nocount off
  insert #t
  select @a a union all select @b
  set nocount on
  drop table #t", new {a=1, b=2 });
Assert.Equal(2, count);
```

多次执行命令
--------------------------------

还允许使用相同的参数签名方便有效地多次执行命令（例如批量加载数据）

示例：

```csharp
var count = connection.Execute(@"insert MyTable(colA, colB) values (@a, @b)",
    new[] { new { a=1, b=1 }, new { a=2, b=2 }, new { a=3, b=3 } }
  );
Assert.Equal(3, count); // 插入3行: "1,1", "2,2" 与 "3,3"
```
这适用于已经实现IEnumerable<T>接口的集合对象T。

性能
-----------

Dapper的一个关键特性是性能。 以下度量标准显示了对DB执行500个`SELECT`语句并将返回的数据映射到对象所需的时间。

性能测试分为3个列表：

- 支持从数据库中提取静态类型对象框架的POCO序列化，使用原生SQL语句。
- 支持返回动态对象列表框架的动态序列化。
- 典型的框架用法：通常典型的框架使用与最佳使用性能明显不同，并且它不会涉及编写SQL语句。
### 超过500次迭代的SELECT映射性能 - POCO序列化 

| 方法                                              | 执行时间 | 备注 |
| --------------------------------------------------- | -------- | ------- |
| 手工编码 (使用 `SqlDataReader`)                | 47ms     |
| Dapper `ExecuteMapperQuery`                         | 49ms     |
| [ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite) (使用Id查询) | 50ms |
| [PetaPoco](https://github.com/CollaboratingPlatypus/PetaPoco) | 52ms     | [可以更快](https://web.archive.org/web/20170921124755/http://www.toptensoftware.com/blog/posts/94-PetaPoco-More-Speed) |
| BLToolkit                                           | 80ms     |
| SubSonic CodingHorror                               | 107ms    |
| NHibernate SQL                                      | 104ms    |
| Linq 2 SQL `ExecuteQuery`                           | 181ms    |
| Entity framework `ExecuteStoreQuery`                | 631ms    |

### 超过500次迭代的SELECT映射性能 - 动态序列化

| 方法                                                   | 执行时间 | 备注 |
| -------------------------------------------------------- | -------- | ------- |
| Dapper `ExecuteMapperQuery` (动态)                    | 48ms     |
| [Massive](https://github.com/FransBouma/Massive)         | 52ms     |
| [Simple.Data](https://github.com/markrendle/Simple.Data) | 95ms     |


### 超过500次迭代的SELECT映射性能 - 典型用法

| 方法                                | 执行时间 | 备注 |
| ------------------------------------- | -------- | ------- |
| Linq 2 SQL CompiledQuery              | 81ms     | 非典型的且不涉及复杂的代码 |
| NHibernate HQL                        | 118ms    |
| Linq 2 SQL                            | 559ms    |
| Entity framework                      | 859ms    |
| SubSonic ActiveRecord.SingleOrDefault | 3619ms   |


性能基准测试信息 [点击这里](https://github.com/StackExchange/Dapper/tree/master/Dapper.Tests.Performance).

可以任意提交包含其他ORM的补丁 - 运行基准测试时，请确保在Release中编译，且不能附加调试器
(<kbd>Ctrl</kbd>+<kbd>F5</kbd>).

或者，你可以使用Frans Bouma的[RawDataAccessBencher](https://github.com/FransBouma/RawDataAccessBencher)或[OrmBenchmark](https://github.com/InfoTechBridge/OrmBenchmark)测试套件作为测试工具使用。

参数化查询
---------------------

可以匿名类型作为参数进行传递，这可以轻松地命名这些参数名称，且能够在数据库平台的查询分析器中简单地使用剪切、粘贴SQL语句并运行。

```csharp
new {A = 1, B = "b"} // A映射到参数@A，B映射到参数@B
```

列表支持
------------
Dapper允许将`IEnumerable<int>`作为传递参数，并能够自动地参数化查询

例子:

```csharp
connection.Query<int>("select * from (select 1 as Id union all select 2 union all select 3) as X where Id in @Ids", new { Ids = new int[] { 1, 2, 3 } });
```

以上将被转换成：

```csharp
select * from (select 1 as Id union all select 2 union all select 3) as X where Id in (@Ids1, @Ids2, @Ids3)" // @Ids1 = 1 , @Ids2 = 2 , @Ids2 = 3
```

文字代替
------------
Dapper支持布尔与数字类型的文字代替。

```csharp
connection.Query("select * from User where UserId = {=Id}", new {Id = 1}));
```

文字替换不作为参数发送; 更好的计划和过滤索引用法将被允许，但通常应谨慎在测试后使用。 当注入的值实际上是固定值（例如，特定于查询的“类别ID”，“状态代码”或“区域”）时，此功能特别有用。 当你在思考文字*live*数据时，也有可能想到*also*并测试特定于提供程序的查询提示，如带有常规参数的[`OPTIMIZE FOR UNKNOWN`](https://blogs.msdn.microsoft.com/sqlprogrammability/2008/11/26/optimize-for-unknown-a-little-known-sql-server-2008-feature/)。


缓冲与未缓冲阅读器
---------------------
Dapper的默认行为是执行SQL并在返回时缓冲整个阅读器。 在大多数情况下，这是理想的，因为它最小化了数据库中的共享锁并减少了数据库网络时间。

但是，在执行大量查询时，可能需要最小化内存占用并仅根据需要加载对象。 为此，将`buffered：false`传递给`Query`方法。

多重映射
---------------------
Dapper允许将单个行映射到多个对象。 如果想避免无关的查询和立即加载关联，这是一个很关键的特性。

例子：

思考这两个类: `Post` and `User`

```csharp
class Post
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string Content { get; set; }
    public User Owner { get; set; }
}

class User
{
    public int Id { get; set; }
    public string Name { get; set; }
}
```

现在我们要把posts表单与users表单进行映射查询。到目前为止，如果我们需要结合2个查询的结果，我们需要一个新的对象来表达它，但在这种情况下将`User`对象放在`Post`对象中更有意义。

这是多重映射的用户案例。你告诉dapper查询返回一个`Post`和一个`User`对象，然后给它描述你想要对包含`Post`和`User`对象的每一行做什么的函数。 在我们的例子中，我们想要获取用户对象并将其放在post对象中。所以编写函数如下：

```csharp
(post, user) => { post.Owner = user; return post; }
```

`Query`方法的3个类型参数指定dapper应该使用哪些对象及返回的内容进行反序列化行。我们将把这两行解释为`Post`和`User`的组合，然后我们返回一个`Post`对象。 因此类型声明变为

```csharp
<Post, User, Post>
```

所有东西都放在一起，看起来像这样：

```csharp
var sql =
@"select * from #Posts p
left join #Users u on u.Id = p.OwnerId
Order by p.Id";

var data = connection.Query<Post, User, Post>(sql, (post, user) => { post.Owner = user; return post;});
var post = data.First();

Assert.Equal("Sams Post1", post.Content);
Assert.Equal(1, post.Id);
Assert.Equal("Sam", post.Owner.Name);
Assert.Equal(99, post.Owner.Id);
```

Dapper能够通过假设Id列被命名为“Id”或“id”来拆分返回的行。 如果主键不同或者希望将行拆分为“Id”以外的其他位置，请使用可选的`splitOn`参数。

多重结果
---------------------
Dapper允许在单个查询中处理多个结果。

例子：

```csharp
var sql =
@"
select * from Customers where CustomerId = @id
select * from Orders where CustomerId = @id
select * from Returns where CustomerId = @id";

using (var multi = connection.QueryMultiple(sql, new {id=selectedId}))
{
   var customer = multi.Read<Customer>().Single();
   var orders = multi.Read<Order>().ToList();
   var returns = multi.Read<Return>().ToList();
   ...
}
```

存储过程
---------------------
Dapper完全支持存储过程：

```csharp
var user = cnn.Query<User>("spGetUser", new {Id = 1},
        commandType: CommandType.StoredProcedure).SingleOrDefault();
```

如果你想要更有趣的东西，你可以这样做：

```csharp
var p = new DynamicParameters();
p.Add("@a", 11);
p.Add("@b", dbType: DbType.Int32, direction: ParameterDirection.Output);
p.Add("@c", dbType: DbType.Int32, direction: ParameterDirection.ReturnValue);

cnn.Execute("spMagicProc", p, commandType: CommandType.StoredProcedure);

int b = p.Get<int>("@b");
int c = p.Get<int>("@c");
```

Ansi字符串和varchar
---------------------
Dapper支持varchar参数，如果使用param在varchar列上执行where子句，请确保以这种方式传递它：

```csharp
Query<Thing>("select * from Thing where Name = @Name", new {Name = new DbString { Value = "abcde", IsFixedLength = true, Length = 10, IsAnsi = true });
```

在SQL Server中，使用unicode编码查询unicode与ANSI编码或查询非unicode编码时，变得至关重要。

每行类型转换
---------------------

通常，自己希望将给定表中的所有行视为相同的数据类型。 但是，在某些情况下，能够将不同的行解析为不同的数据类型是有用的。 这就是`IDataReader.GetRowParser`派上用场的地方。


假设有一个名为“Shapes”的数据库表，其中包含列：`Id`，`Type`和`Data`，你想要基于Type列的值将它的行解析为`Circle`，`Square`或`Triangle`对象。

```csharp
var shapes = new List<IShape>();
using (var reader = connection.ExecuteReader("select * from Shapes"))
{
    // Generate a row parser for each type you expect.
    // The generic type <IShape> is what the parser will return.
    // The argument (typeof(*)) is the concrete type to parse.
    var circleParser = reader.GetRowParser<IShape>(typeof(Circle));
    var squareParser = reader.GetRowParser<IShape>(typeof(Square));
    var triangleParser = reader.GetRowParser<IShape>(typeof(Triangle));

    var typeColumnIndex = reader.GetOrdinal("Type");

    while (reader.Read())
    {
        IShape shape;
        var type = (ShapeType)reader.GetInt32(typeColumnIndex);
        switch (type)
        {
          	case ShapeType.Circle:
            	shape = circleParser(reader);
            	break;
            case ShapeType.Square:
            	shape = squareParser(reader);
            	break;
            case ShapeType.Triangle:
            	shape = triangleParser(reader);
            	break;
          	default:
            	throw new NotImplementedException();
        }

      	shapes.Add(shape);
    }
}
```

限制与警告
---------------------
Dapper缓存有关它运行的每个查询的信息，这使它能够快速实现对象并快速处理参数。 当前实现将此信息缓存在`ConcurrentDictionary`对象中。仅使用一次的语句通常会从此缓存中刷新。尽管如此，如果您在不使用参数的情况下动态生成SQL字符串，则可能会遇到内存问题。

Dapper的简洁性意味着ORM附带的许多功能都被剥离了。Dapper担心95％的情况，并为您提供大多数时间所需的工具，并不试图解决所有问题。

Dapper支持哪些数据库？
---------------------
Dapper没有特定于DB的实现细节，它适用于所有.NET ADO提供程序，包括[SQLite](https://www.sqlite.org/),SQL CE，Firebird，Oracle，MySQL，PostgreSQL和SQL Server。

有完整的例子清单吗？
---------------------
Dapper有一个完整位于[测试工程](https://github.com/StackExchange/Dapper/tree/master/Dapper.Tests)的测试套件。

谁在用这个？
---------------------
[Stack Overflow](https://stackoverflow.com/)正在使用Dapper。

------------------------------------------------------------------------

######
原文(Original Text)：

Dapper - a simple object mapper for .Net
========================================
[![Build status](https://ci.appveyor.com/api/projects/status/8rbgoxqio76ynj4h?svg=true)](https://ci.appveyor.com/project/StackExchange/dapper)

Release Notes
-------------
Located at [stackexchange.github.io/Dapper](https://stackexchange.github.io/Dapper/)

Packages
--------

MyGet Pre-release feed: https://www.myget.org/gallery/dapper

| Package | NuGet Stable | NuGet Pre-release | Downloads | MyGet |
| ------- | ------------ | ----------------- | --------- | ----- |
| [Dapper](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/v/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/vpre/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper](https://img.shields.io/nuget/dt/Dapper.svg)](https://www.nuget.org/packages/Dapper/) | [![Dapper MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper) |
| [Dapper.Contrib](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/v/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/vpre/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib](https://img.shields.io/nuget/dt/Dapper.Contrib.svg)](https://www.nuget.org/packages/Dapper.Contrib/) | [![Dapper.Contrib MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.Contrib.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.Contrib) |
| [Dapper.EntityFramework](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/v/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/vpre/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework](https://img.shields.io/nuget/dt/Dapper.EntityFramework.svg)](https://www.nuget.org/packages/Dapper.EntityFramework/) | [![Dapper.EntityFramework MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.EntityFramework.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.EntityFramework) |
| [Dapper.EntityFramework.StrongName](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/v/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/vpre/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName](https://img.shields.io/nuget/dt/Dapper.EntityFramework.StrongName.svg)](https://www.nuget.org/packages/Dapper.EntityFramework.StrongName/) | [![Dapper.EntityFramework.StrongName MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.EntityFramework.StrongName.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.EntityFramework.StrongName) |
| [Dapper.Rainbow](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/v/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/vpre/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow](https://img.shields.io/nuget/dt/Dapper.Rainbow.svg)](https://www.nuget.org/packages/Dapper.Rainbow/) | [![Dapper.Rainbow MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.Rainbow.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.Rainbow) |
| [Dapper.SqlBuilder](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/v/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/vpre/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder](https://img.shields.io/nuget/dt/Dapper.SqlBuilder.svg)](https://www.nuget.org/packages/Dapper.SqlBuilder/) | [![Dapper.SqlBuilder MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.SqlBuilder.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.SqlBuilder) |
| [Dapper.StrongName](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/v/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/vpre/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName](https://img.shields.io/nuget/dt/Dapper.StrongName.svg)](https://www.nuget.org/packages/Dapper.StrongName/) | [![Dapper.StrongName MyGet](https://img.shields.io/myget/dapper/vpre/Dapper.StrongName.svg)](https://www.myget.org/feed/dapper/package/nuget/Dapper.StrongName) |

Features
--------
Dapper is a [NuGet library](https://www.nuget.org/packages/Dapper) that you can add in to your project that will extend your `IDbConnection` interface.

It provides 3 helpers:

Execute a query and map the results to a strongly typed List
------------------------------------------------------------

```csharp
public static IEnumerable<T> Query<T>(this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null, bool buffered = true)
```
Example usage:

```csharp
public class Dog
{
    public int? Age { get; set; }
    public Guid Id { get; set; }
    public string Name { get; set; }
    public float? Weight { get; set; }

    public int IgnoredProperty { get { return 1; } }
}

var guid = Guid.NewGuid();
var dog = connection.Query<Dog>("select Age = @Age, Id = @Id", new { Age = (int?)null, Id = guid });

Assert.Equal(1,dog.Count());
Assert.Null(dog.First().Age);
Assert.Equal(guid, dog.First().Id);
```

Execute a query and map it to a list of dynamic objects
-------------------------------------------------------

```csharp
public static IEnumerable<dynamic> Query (this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null, bool buffered = true)
```
This method will execute SQL and return a dynamic list.

Example usage:

```csharp
var rows = connection.Query("select 1 A, 2 B union all select 3, 4");

Assert.Equal(1, (int)rows[0].A);
Assert.Equal(2, (int)rows[0].B);
Assert.Equal(3, (int)rows[1].A);
Assert.Equal(4, (int)rows[1].B);
```

Execute a Command that returns no results
-----------------------------------------

```csharp
public static int Execute(this IDbConnection cnn, string sql, object param = null, SqlTransaction transaction = null)
```

Example usage:

```csharp
var count = connection.Execute(@"
  set nocount on
  create table #t(i int)
  set nocount off
  insert #t
  select @a a union all select @b
  set nocount on
  drop table #t", new {a=1, b=2 });
Assert.Equal(2, count);
```

Execute a Command multiple times
--------------------------------

The same signature also allows you to conveniently and efficiently execute a command multiple times (for example to bulk-load data)

Example usage:

```csharp
var count = connection.Execute(@"insert MyTable(colA, colB) values (@a, @b)",
    new[] { new { a=1, b=1 }, new { a=2, b=2 }, new { a=3, b=3 } }
  );
Assert.Equal(3, count); // 3 rows inserted: "1,1", "2,2" and "3,3"
```
This works for any parameter that implements IEnumerable<T> for some T.

Performance
-----------

A key feature of Dapper is performance. The following metrics show how long it takes to execute 500 `SELECT` statements against a DB and map the data returned to objects.

The performance tests are broken in to 3 lists:

- POCO serialization for frameworks that support pulling static typed objects from the DB. Using raw SQL.
- Dynamic serialization for frameworks that support returning dynamic lists of objects.
- Typical framework usage. Often typical framework usage differs from the optimal usage performance wise. Often it will not involve writing SQL.

### Performance of SELECT mapping over 500 iterations - POCO serialization

| Method                                              | Duration | Remarks |
| --------------------------------------------------- | -------- | ------- |
| Hand coded (using a `SqlDataReader`)                | 47ms     |
| Dapper `ExecuteMapperQuery`                         | 49ms     |
| [ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite) (QueryById) | 50ms |
| [PetaPoco](https://github.com/CollaboratingPlatypus/PetaPoco) | 52ms     | [Can be faster](https://web.archive.org/web/20170921124755/http://www.toptensoftware.com/blog/posts/94-PetaPoco-More-Speed) |
| BLToolkit                                           | 80ms     |
| SubSonic CodingHorror                               | 107ms    |
| NHibernate SQL                                      | 104ms    |
| Linq 2 SQL `ExecuteQuery`                           | 181ms    |
| Entity framework `ExecuteStoreQuery`                | 631ms    |

### Performance of SELECT mapping over 500 iterations - dynamic serialization

| Method                                                   | Duration | Remarks |
| -------------------------------------------------------- | -------- | ------- |
| Dapper `ExecuteMapperQuery` (dynamic)                    | 48ms     |
| [Massive](https://github.com/FransBouma/Massive)         | 52ms     |
| [Simple.Data](https://github.com/markrendle/Simple.Data) | 95ms     |


### Performance of SELECT mapping over 500 iterations - typical usage

| Method                                | Duration | Remarks |
| ------------------------------------- | -------- | ------- |
| Linq 2 SQL CompiledQuery              | 81ms     | Not super typical involves complex code |
| NHibernate HQL                        | 118ms    |
| Linq 2 SQL                            | 559ms    |
| Entity framework                      | 859ms    |
| SubSonic ActiveRecord.SingleOrDefault | 3619ms   |


Performance benchmarks are available [here](https://github.com/StackExchange/Dapper/tree/master/Dapper.Tests.Performance).

Feel free to submit patches that include other ORMs - when running benchmarks, be sure to compile in Release and not attach a debugger (<kbd>Ctrl</kbd>+<kbd>F5</kbd>).

Alternatively, you might prefer Frans Bouma's [RawDataAccessBencher](https://github.com/FransBouma/RawDataAccessBencher) test suite or [OrmBenchmark](https://github.com/InfoTechBridge/OrmBenchmark).

Parameterized queries
---------------------

Parameters are passed in as anonymous classes. This allow you to name your parameters easily and gives you the ability to simply cut-and-paste SQL snippets and run them in your db platform's Query analyzer.

```csharp
new {A = 1, B = "b"} // A will be mapped to the param @A, B to the param @B
```

List Support
------------
Dapper allows you to pass in `IEnumerable<int>` and will automatically parameterize your query.

For example:

```csharp
connection.Query<int>("select * from (select 1 as Id union all select 2 union all select 3) as X where Id in @Ids", new { Ids = new int[] { 1, 2, 3 } });
```

Will be translated to:

```csharp
select * from (select 1 as Id union all select 2 union all select 3) as X where Id in (@Ids1, @Ids2, @Ids3)" // @Ids1 = 1 , @Ids2 = 2 , @Ids2 = 3
```

Literal replacements
------------
Dapper supports literal replacements for bool and numeric types.

```csharp
connection.Query("select * from User where UserId = {=Id}", new {Id = 1}));
```

The literal replacement is not sent as a parameter; this allows better plans and filtered index usage but should usually be used sparingly and after testing. This feature is particularly useful when the value being injected
is actually a fixed value (for example, a fixed "category id", "status code" or "region" that is specific to the query). For *live* data where you are considering literals, you might *also* want to consider and test provider-specific query hints like [`OPTIMIZE FOR UNKNOWN`](https://blogs.msdn.microsoft.com/sqlprogrammability/2008/11/26/optimize-for-unknown-a-little-known-sql-server-2008-feature/) with regular parameters.

Buffered vs Unbuffered readers
---------------------
Dapper's default behavior is to execute your SQL and buffer the entire reader on return. This is ideal in most cases as it minimizes shared locks in the db and cuts down on db network time.

However when executing huge queries you may need to minimize memory footprint and only load objects as needed. To do so pass, `buffered: false` into the `Query` method.

Multi Mapping
---------------------
Dapper allows you to map a single row to multiple objects. This is a key feature if you want to avoid extraneous querying and eager load associations.

Example:

Consider 2 classes: `Post` and `User`

```csharp
class Post
{
    public int Id { get; set; }
    public string Title { get; set; }
    public string Content { get; set; }
    public User Owner { get; set; }
}

class User
{
    public int Id { get; set; }
    public string Name { get; set; }
}
```

Now let us say that we want to map a query that joins both the posts and the users table. Until now if we needed to combine the result of 2 queries, we'd need a new object to express it but it makes more sense in this case to put the `User` object inside the `Post` object.

This is the user case for multi mapping. You tell dapper that the query returns a `Post` and a `User` object and then give it a function describing what you want to do with each of the rows containing both a `Post` and a `User` object. In our case, we want to take the user object and put it inside the post object. So we write the function:

```csharp
(post, user) => { post.Owner = user; return post; }
```

The 3 type arguments to the `Query` method specify what objects dapper should use to deserialize the row and what is going to be returned. We're going to interpret both rows as a combination of `Post` and `User` and we're returning back a `Post` object. Hence the type declaration becomes

```csharp
<Post, User, Post>
```

Everything put together, looks like this:

```csharp
var sql =
@"select * from #Posts p
left join #Users u on u.Id = p.OwnerId
Order by p.Id";

var data = connection.Query<Post, User, Post>(sql, (post, user) => { post.Owner = user; return post;});
var post = data.First();

Assert.Equal("Sams Post1", post.Content);
Assert.Equal(1, post.Id);
Assert.Equal("Sam", post.Owner.Name);
Assert.Equal(99, post.Owner.Id);
```

Dapper is able to split the returned row by making an assumption that your Id columns are named `Id` or `id`. If your primary key is different or you would like to split the row at a point other than `Id`, use the optional `splitOn` parameter.

Multiple Results
---------------------
Dapper allows you to process multiple result grids in a single query.

Example:

```csharp
var sql =
@"
select * from Customers where CustomerId = @id
select * from Orders where CustomerId = @id
select * from Returns where CustomerId = @id";

using (var multi = connection.QueryMultiple(sql, new {id=selectedId}))
{
   var customer = multi.Read<Customer>().Single();
   var orders = multi.Read<Order>().ToList();
   var returns = multi.Read<Return>().ToList();
   ...
}
```

Stored Procedures
---------------------
Dapper fully supports stored procs:

```csharp
var user = cnn.Query<User>("spGetUser", new {Id = 1},
        commandType: CommandType.StoredProcedure).SingleOrDefault();
```

If you want something more fancy, you can do:

```csharp
var p = new DynamicParameters();
p.Add("@a", 11);
p.Add("@b", dbType: DbType.Int32, direction: ParameterDirection.Output);
p.Add("@c", dbType: DbType.Int32, direction: ParameterDirection.ReturnValue);

cnn.Execute("spMagicProc", p, commandType: CommandType.StoredProcedure);

int b = p.Get<int>("@b");
int c = p.Get<int>("@c");
```

Ansi Strings and varchar
---------------------
Dapper supports varchar params, if you are executing a where clause on a varchar column using a param be sure to pass it in this way:

```csharp
Query<Thing>("select * from Thing where Name = @Name", new {Name = new DbString { Value = "abcde", IsFixedLength = true, Length = 10, IsAnsi = true });
```

On SQL Server it is crucial to use the unicode when querying unicode and ANSI when querying non unicode.

Type Switching Per Row
---------------------

Usually you'll want to treat all rows from a given table as the same data type. However, there are some circumstances where it's useful to be able to parse different rows as different data types. This is where `IDataReader.GetRowParser` comes in handy.

Imagine you have a database table named "Shapes" with the columns: `Id`, `Type`, and `Data`, and you want to parse its rows into `Circle`, `Square`, or `Triangle` objects based on the value of the Type column.

```csharp
var shapes = new List<IShape>();
using (var reader = connection.ExecuteReader("select * from Shapes"))
{
    // Generate a row parser for each type you expect.
    // The generic type <IShape> is what the parser will return.
    // The argument (typeof(*)) is the concrete type to parse.
    var circleParser = reader.GetRowParser<IShape>(typeof(Circle));
    var squareParser = reader.GetRowParser<IShape>(typeof(Square));
    var triangleParser = reader.GetRowParser<IShape>(typeof(Triangle));

    var typeColumnIndex = reader.GetOrdinal("Type");

    while (reader.Read())
    {
        IShape shape;
        var type = (ShapeType)reader.GetInt32(typeColumnIndex);
        switch (type)
        {
          	case ShapeType.Circle:
            	shape = circleParser(reader);
            	break;
            case ShapeType.Square:
            	shape = squareParser(reader);
            	break;
            case ShapeType.Triangle:
            	shape = triangleParser(reader);
            	break;
          	default:
            	throw new NotImplementedException();
        }

      	shapes.Add(shape);
    }
}
```

Limitations and caveats
---------------------
Dapper caches information about every query it runs, this allow it to materialize objects quickly and process parameters quickly. The current implementation caches this information in a `ConcurrentDictionary` object. Statements that are only used once are routinely flushed from this cache. Still, if you are generating SQL strings on the fly without using parameters it is possible you may hit memory issues.

Dapper's simplicity means that many feature that ORMs ship with are stripped out. It worries about the 95% scenario, and gives you the tools you need most of the time. It doesn't attempt to solve every problem.

Will Dapper work with my DB provider?
---------------------
Dapper has no DB specific implementation details, it works across all .NET ADO providers including [SQLite](https://www.sqlite.org/), SQL CE, Firebird, Oracle, MySQL, PostgreSQL and SQL Server.

Do you have a comprehensive list of examples?
---------------------
Dapper has a comprehensive test suite in the [test project](https://github.com/StackExchange/Dapper/tree/master/Dapper.Tests).

Who is using this?
---------------------
Dapper is in production use at [Stack Overflow](https://stackoverflow.com/).

