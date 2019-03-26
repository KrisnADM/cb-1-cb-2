<html>
<head>
    <script>
    function nilai()
    {
        var nilai1=["1","2","3","4","5","6","7","8","9","10"];
        var nilai2=["10","20","30","40","50","60","70","80","90","100"];
        var nilai3=["100","200","300","400","500","600","700","800","900","1000"];
        var p;
        p = document.getElementById("cb1").value;
        var text;
        if(p == "n1"){
            for( var i=0; i<nilai1.length; i++){
                text += "<option>" + nilai1[i] +"</option>";
            }
        } else if(p == "n2"){
            for(var i=0; i<nilai2.length; i++){
                text += "<option>" + nilai2[i] +"</option>";
            }
        } else {
        for(var i=0; i<nilai3.length; i++){
            text += "<option>" + nilai3[i] +"</option>";
            }
        }
        document.getElementById("cb2").innerHTML=text;
    }
    </script>
</head>
<body>
    <select id="cb1" onchange="nilai()">
        <option value="n1">nilai1</option>
        <option value="n2">nilai2</option>
        <option value="n3">nilai3</option>
    </select>
    <br>    
    <select id="cb2">       

    </select>
</body>
</html>
