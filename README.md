[Uploading index.ht<!DOCTYPE html>
<html lang="en">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta charset="utf-8">
    <title>Mini Calender</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="hero">
        <div class="calender">
            <div class="left">
                <p id="date">01</p>
                <p id="day">Sunday</p>
            </div>
            <div class="right">
                <p id="month">January</p>
                <p id="year">2024</p>
            </div>
        </div>
    </div>

<script>

const date = document.getElementById('date');
const day = document.getElementById('day');
const month = document.getElementById('month');
const year = document.getElementById('year');

const today = new Date();

const weekDays = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];
const allMonths = ["January", "February", "March", "April", "May", "June", "July", "August",
"September", "October", "November", "December"];

date.innerHTML = (today.getDate()<10?"0":"") + today.getDate();
day.innerHTML = weekDays[today.getDay()];
month.innerHTML = allMonths[today.getMonth()];
year.innerHTML = today.getFullYear();

</script>

</body>
[Uploading * {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}

.hero {
    width: 100%;
    min-height: 100vh;
    background: linear-gradient(45deg, #1d0000, #20205b);
    display: flex;
    align-items: center;
    justify-content: center;
}

.calender {
    width: 300px;
    height: 250px;
    background: #fff;
    display: flex;
    align-items: center;
    border-radius: 10px;
}

.left, .right {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    font-size: 24px;
}

.right {
    width: 42%;
    background: #f4351e;
    color: #fff;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}

.left {
    width: 58%;
}

#date {
    font-size: 100px;
    line-height: 90px;
}styles.css…]()

</html>ml…]()


