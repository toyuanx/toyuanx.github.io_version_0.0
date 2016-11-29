11月博客资源
===
> **全选与全不选**功能常出现在**后台管理**与**列表操作**中，通过总结网上博文，写了一个简易功能，可以实现动态生成checkbox的全选。

##功能

<!DOCTYPE>
<html>
<head>
    <meta charset="utf-8">
    <title>全选与全不选</title>
    <script type="text/javascript" src="http://cdn.bootcss.com/jquery/3.1.1/jquery.js"></script>
</head>
<body>
<div>
    <input id="all-check" type="checkbox">点击选择
    <br>
    <input type="checkbox">1
    <input type="checkbox">2
    <input type="checkbox">3
    <input type="checkbox">4
    <input type="checkbox">5
    <input type="checkbox">6
    <input type="checkbox">7
</div>

</body>
<script>
    jQuery("#all-check").click(function () {
        var isChecked = jQuery(this).prop("checked");
        jQuery("input[type='checkbox']").prop("checked", isChecked);
    });
</script>
</html>

##代码
```JAVASCRIPT
<!DOCTYPE>
<html>

<head>
    <meta charset="utf-8">
    <title>全选与全不选</title>
    <script type="text/javascript" src="http://cdn.bootcss.com/jquery/3.1.1/jquery.js"></script>
</head>

<body>
<div>
    <input id="all-check" type="checkbox">点击选择
    <br>
    <input type="checkbox">1
    <input type="checkbox">2
    <input type="checkbox">3
    <input type="checkbox">4
    <input type="checkbox">5
    <input type="checkbox">6
    <input type="checkbox">7
</div>
</body>

<script>
    jQuery("#all-check").click(function () {
        var isChecked = jQuery(this).prop("checked");
        jQuery("input[type='checkbox']").prop("checked", isChecked);
    });
</script>

</html>
```

##结语
积少成多，受益匪浅。
