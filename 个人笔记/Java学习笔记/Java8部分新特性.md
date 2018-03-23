# Java8部分新特性

## 接口的默认方法

假设没有默认方法这种机制，那么如果要为Mortal增加一个新的方法revive,那么所有实现了Mortal接口的类，都需要做改动。

但是引入了默认方法后，原来的类，不需要做任何改动，并且还能得到这个默认方法。

通过这种手段，就能够很好的扩展新的类，并且做到不影响原来的类。
```
package charactor;
 
public interface Mortal {
    public void die();
 
    default public void revive() {
        System.out.println("本英雄复活了");
    }
}
```
## Lambda

Java没有函数的概念，因此，Java的Lambda表达式必须绑定到被称为**功能接口**的特定对象类型。

### 表现形式

```
(int a, int b) -> {  return a + b; }

() -> System.out.println("Hello World");

(String s) -> { System.out.println(s); }

() -> 42

() -> { return 3.1415 };
```

- 可选类型声明：不需要声明参数类型，编译器可以统一识别参数值。
- 可选的参数圆括号：一个参数无需定义圆括号，但多个参数需要定义圆括号。
- 可选的大括号：如果主体包含了一个语句，就不需要使用大括号。
- 可选的返回关键字：如果主体只有一个表达式返回值则编译器会自动返回值，大括号需要指定明表达式返回了一个数值。

### 方法引用

