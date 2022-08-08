**关键字this**有两个用途：一是引用隐式参数，二是调用该类的其他构造器

**关键字super**有两个用途：一是调用超类的方法，二是调用超类的构造器

**方法调用过程**：1）编译器查看对象的声明类型和方法名--找出所有可能被调用的方法

​							2）编译器查看调用方法时提供的参数类型。 编译器已获得需要调用的方法名字和参数类型。 如果不存在就会报错。

 **动态绑定有一个非常重要的特性：** 无需对现存的代码进行修改，就可以对程序进行扩展。 

 假设增加一个新类 Executive, 并且变量 e 有可能引用这个类的对象， 我们不需要对包含调用 e.getSalary() 的代码进行重新编译。如果 e 恰好引用一个 Executive 类的对象，就会自动地调 用 Executive.getSalaryO 方法。 

 在覆盖一个方法的时候，子类方法不能低于超类方法的可见性。特别是， 如果超类 方法是 public, 子类方法一定要声明为 public。 

 如果将一个类声明为 final， 只有其中的方法自动地成为 final, 而不包括域 。

 如果一个方法没有被覆盖并且很短， 编译器就能够对它进行优化处理， 这个过程为称为内联 。

 例如，内联调用 e.getName( ) 将被替换为访问 e.name 域。 

**A insttanceof B可以判断A类型是否可以转换为B，可以则为真**

**关键字protected 允许子类访问超类中被其修饰的方法和域 **  例如： Manager 类中的方法只能够访问 Manager 对象中的 hireDay 域， 而不能访问其他 Employee 对象中的这个域。 

 **Java 中的受保护部分对所有子类及同一个包中的所有其他类都可见。** 

 Object 类中的 equals 方法用于检测一个对象是否等于另外一个对象。 

 Java 语言规范要求 equals 方法具有下面的特性：

 1 ) 自反性：对于任何非空引用 x, x.equals(x） 应该返回 truec。

2 ) 对称性: 对于任何引用 x 和 y, 当且仅当 y.equals(x) 返回 true , x.equals(y) 也应该返 回 true。

 3 ) 传递性： 对于任何引用 x、 y 和 z, 如果 x.equals(y) 返 回 true， y.equals(z) 返回 true, x.equals(z) 也应该返回 true。 

4 ) 一致性： 如果 x 和 y 引用的对象没有发生变化，反复调用 x.eqimIS(y) 应该返回同样 的结果。 

5 ) 对于任意非空引用 x, x.equals(null) 应该返回 false 。

 **下面给出编写一个完美的 equals 方法的建议：**

 **1 ) 显式参数命名为 otherObject, 稍后需要将它转换成另一个叫做 other 的变量。** 

**2 ) 检测 this 与 otherObject 是否引用同一个对象： if (this == otherObject) return true; 这条语句只是一个优化。实际上，这是一种经常采用的形式。因为计算这个等式要比一 个一个地比较类中的域所付出的代价小得多。** 

**3 ) 检测 otherObject 是否为 null, 如 果 为 null, 返 回 false。这项检测是很必要的。 if (otherObject = null) return false;** 

**4 ) 比较 this 与 otherObject 是否属于同一个类。如果 equals 的语义在每个子类中有所改 变，就使用 getClass 检测： if (getClass() != otherObject.getCIass()) return false; 如果所有的子类都拥有统一的语义，就使用 instanceof 检测： if (!(otherObject instanceof ClassName)) return false;** 

**5 ) 将 otherObject 转换为相应的类类型变量： ClassName other = (ClassName) otherObject** 

**6 ) 现在开始对所有需要比较的域进行比较了。使用 == 比较基本类型域，使用 equals 比 较对象域。如果所有的域都匹配， 就返回 true; 否 则 返 回 false。** 

 **如果在子类中重新定义 equals, 就要在其中包含调用 super.equals(other)** 

 对于数组类型的域， 可以使用静态的 Arrays.equals 方法检测相应的数组元素是否相等。  

 如果重新定义 equals方法，就必须重新定义 hashCode 方法， 以便用户可以将对象插人 到散列表中 。

 一旦能确保不会造成严重的后果，可以用@SuppressWamings("unchecked") 标注来标记 这个变量能够接受类型转换， 如下所示： @SuppressWarnings("unchecked") ArrayList result = (ArrayList) employeeDB.find(query); // yields another warning 

 能够分析类能力的程序称为反射（reflective )。 

 **反射机制可以用来：** 

**•在运行时分析类的能力。** 

**•在运行时查看对象， 例如， 编写一个 toString 方法供所有类使用。**

 **•实现通用的数组操作代码。**

 **•利用 Method 对象， 这个对象很像C++中的函数指针。** 

# Class类

forName方法获取类名对应的Class对象--如果类名保存在字符串中。并可在运行中改变，就可以使用这个方法。

 *在启动时， 包含 main 方法的类被加载。它会加载所有需要的类。这些被加栽的类 又要加载它们需要的类， 以此类推。对于一个大型的应用程序来说， 这将会消耗很多时 间， 用户会因此感到不耐烦。可以使用下面这个技巧给用户一种启动速度比较快的幻觉。 不过，要确保包含 main 方法的类没有显式地引用其他的类。首先，显示一个启动画面； 然后，通过调用 Class.forName 手工地加载其他的类 

 将 forName 与 newlnstance 配合起来使用， 可以根据存储在字符串中的类名创建一个对象。

 String s = "java.util .Random"; 

Object m = Cl ass.forName (s) .newlnstance(); 

