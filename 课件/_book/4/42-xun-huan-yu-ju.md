## **4.2循环语句**

### **4.2.1for**

```go
var i,sum int

for i = 1; i <= 100; i++ {
    sum+=i
}
fmt.Println("sum=",sum)
```

### **4.2.2range**

关键字 range 会返回两个值，第一个返回值是元素的数组下标，第二个返回值是元素的值：

```go
s := "abc"
for i := range s{//支持string/array/slice/map。
    fmt.Printf("%c\n",s[i])
}

for _, c := range s{//忽略index
    fmt.Printf("%c\n",c)
}

for i, c := range s{
    fmt.Printf("%d,%c\n",i,c)
}
```



