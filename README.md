<div id="one_arr"> 一维数组 </div>
<div id="two_arr"> 二维数组 </div>
<div id="obj"> 键值数组 </div>

<script type="text/javascript" src="__PUBLIC__/js/jquery.js"></script>
<script type="text/javascript">
    $(function () {
        $('#one_arr').click(function () {
            var one_arr = ["one", "two", "three", "four"]; 
            $.each(one_arr, function(){
            alert(this); 
            });
        });

        $('#two_arr').click(function () {
            var two_arr = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] 
            $.each(two_arr, function(i, item){
                $.each(item, function(j, result){
                alert(result); 
                });
            });
        });

        $('#obj').click(function () {
            var obj = { one:100, two:364, three:547, four:509}; 
            $.each(obj, function(key, val) {
            alert(obj[key]); 
            });
        });

});
</script>
