# function

簡單回傳function
```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
        function retruncode ($value)
        {
            echo $value;
        }
        retruncode(30);
    ?>
</body>
</html>
```

## 傳值和傳址

### 錯誤
```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
        $sum = 9;
        function fun($sum)
        {
            return $sum+=1;
        }
        fun($sum);
        echo "取值\$sum:".$sum."<BR>";
        fun($sum);
        echo "取值\$sum:".$sum;
    ?>
</body>
</html>
```

output：

![image](https://user-images.githubusercontent.com/55253641/173556358-8fd5c4e4-072a-48de-9c6f-7699b04e9e1f.png)

### 指定到變數

```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
        $sum = 9;
        function fun(&$sum)
        {
            return $sum+=1;
        }
        fun($sum);
        echo "取值\$sum:".$sum."<BR>";
        fun($sum);
        echo "取值\$sum:".$sum;
    ?>
</body>
</html>
```

output : 

![image](https://user-images.githubusercontent.com/55253641/173556550-ae552cc3-6c86-4a2a-b6b1-a8d61c6f2380.png)

