# Ex04 Places Around Me
## Date: 

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE
```
<!DOCTYPE html>
<html lang="en">
<head>
</head>
<script>
    function coord(event) {
        let x=event.clientX;
        let y=event.clientY;
        document.getElementById("txt1").value=x;
        document.getElementById("txt2").value=y;
    }
</script>
<body>
    <img src="map.png" width="1000px" usemap="#MapNew" onmousemove="coord(event)">
    <MAP name="MapNew">
        <AREA shape="RECT" coords="334,209,414,200" href="https://stannsmhss.com/" Title="ST.Anne's High School" >
        <AREA shape="RECT" coords="476,148,509,149" href="https://snvmhss.org/" Title="Shri Nehru Vidyalaya School" >
        <AREA shape="RECT" coords="621,152,683,155" href="https://www.hivemontessori.com/" Title="Hive Montessori School" >
    </MAP> <br>
    X coord:<input type="text" name="" id="txt1"> <br>
    Y coord:<input type="text" name="" id="txt2"> 

</body>
</html>
```

## OUTPUT

![alt text](map.png)

![alt text](<output 1.png>)

![alt text](<output 2.png>)

![alt text](<output 3.png>)





## RESULT
The program for implementing image maps using HTML is executed successfully.
