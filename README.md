# 30.09.22
## 1. Complete the method that takes a boolean value and return a "Yes" string for true, or a "No" string for false.
___
### Мое рещение 
```java
class YesOrNo
{
  public static String boolToWord(boolean b)
  {
    return b ? "Yes" : "No";
  } 
}
```

### Понравившееся решение
```java
class YesOrNo
{
  public static String boolToWord(boolean b)
  {
    if(!b)
      return "No";
    else
      return "Yes";
  }
  
}
```
## 2.You're writing code to control your town's traffic lights. You need a function to handle each change from green, to yellow, to red, and then to green again.
### Мое рещение 
```java
public class TrafficLights {

  public static String updateLight(String current) {
    
    String tRed = "red";
    String tYellow = "yellow";
    String tGreen = "green";
    
    if (current == tGreen) return tYellow;
    else if (current == tYellow) return tRed;
    else return tGreen;
      
  }
}
```

### Понравившееся решение
```java
public class TrafficLights {

  public static String updateLight(String current) {
    switch (current) {
      case "red": return "green";
      case "yellow": return "red";
      case "green": return "yellow";
      default: throw new IllegalArgumentException();
    }
  }

}
```
