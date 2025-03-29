<!DOCTYPE html>
<html lang="fa">
<head> 
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مقالاتی که از دل برون می‌آید</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 70px;
            background-color: rgb(28, 28, 28);
            color: rgb(7, 8, 8);
        }
        .typing {
            font-size: 20px;
            color: azure;
            display: inline-block;
            border-right: 3px solid white; /* نشانگر تایپ */
            padding-right: 5px;
            text-align: center;
            white-space: pre-line; /* حفظ فرمت متن و رفتن به خط بعد */
        }
        img {
            width: 20%;
            max-width: 900px;
            height: auto;
            border-radius: 10px;
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            cursor: pointer;
            border: none;
            background-color: #949494;
            color: white;
            border-radius: 5px;
            transition: 0.3s;
        }
        button:hover {
            background-color: #cccccc;
        }
        #text {
            display: none; /* در ابتدا مخفی است */
            font-size: 20px;
            margin-top: 20px;
            color: #d3d3d3;
        }
    </style>
</head>
<body>
    <h1 style="background-color: rgb(173, 144, 106);"> برای خالی کردن افکارم در کنارتان ماندم.</h1>
    
    <p id="text" class="typing"></p> <!-- پاراگراف برای نمایش افکت تایپ -->


      <img src="https://i.pinimg.com/736x/c2/24/a4/c224a479a201ec56646a09ecbacf427c.jpg" alt="تصویر شاعرانه">



    <script>
        const text = `کنار تو تنهاتر شده ام.
        از تو تا اوج تو، زندگی من گسترده است.
        از من تا ام تو گسترده ای.
        با تو برخوردم.
        به راز پرستش پیوستم.
        از تو به راه افتادم.
        به جلوه ی رنج رسیدم.
        و با این همه ای شفاف.
        و با این همه ای شگرف.
        مرا راهی از تو به در نیست.
        زمین باران را صدا می زند.
        من تو را.`;

        let index = 0;
        function typeEffect() {
            if (index < text.length) {
                document.getElementById("text").innerHTML += text.charAt(index) === "\n" ? "<br>" : text.charAt(index);
                index++;
                setTimeout(typeEffect, 70); // تنظیم سرعت تایپ (هر 70 میلی‌ثانیه یک حرف اضافه شود)
            } else {
                document.getElementById("text").style.borderRight = "none"; // حذف نشانگر بعد از اتمام
            }
        }
        typeEffect();
    </script>
<h2>
<button onclick="showText()">بزن روش کمتر حرف بزن</button>
<p id="text">  Stop making drama, you are not Shakespeare!</p>

<script>
    function showText() {
        document.getElementById("text").style.display = "block";
    }
</script>

</h2>

</body>

</html>
