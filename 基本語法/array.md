# array陣列

## foreach array專用迴圈
```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
       $name = array("Jack","Alice","Stanley","Tony","John","xiaoan","yuniko","xargon","kenny","tnming");
       foreach( $name as $allname){
            echo $allname."\t";
       }
    ?>
</body>
</html>
```

## 二微陣列
### 需要使用雙陣列迴圈來把值取出來
```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
       $suject = array("座號/科目","國文","英文","數學","自然");
       $student = array("1","23","60","99","40");
       $student_2 = array("2","49","92","54","62");
       $student_3 = array("3","73","30","70","53");
       $array = array($suject,$student,$student_2,$student_3);

       foreach($array as $show_row)
       {    foreach($show_row as $show_column)
            { echo $show_column."\t"; }
            echo "<BR>";
       }
    ?>
</body>
</html>

```


```php
<html>
<head> 
    <title>PHP var 測試</title>
</head>
<body>
    <?php
        $array["a"] = 1;
        $array[] = 2;
        $array["b"] = 3;
        $array[] = 4;

        echo "1.\t";
        print_r($array);
    ?>
</body>
</html>
```

output：

![image](https://user-images.githubusercontent.com/55253641/173551770-9642bfca-083c-4151-accc-c53461779224.png)
