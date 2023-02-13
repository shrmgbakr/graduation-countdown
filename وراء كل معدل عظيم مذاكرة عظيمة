(function () {
   const second = 1000,
      minute = second * 60,
      hour = minute * 60,
      day = hour * 24;

   let gradDate = "03/01/2023";

   const countDown = new Date(gradDate).getTime(),
      x = setInterval(function () {
         const now = new Date().getTime(),
            distance = countDown - now;

         (document.getElementById("days").innerText = Math.floor(distance / day)),
            (document.getElementById("hours").innerText = Math.floor(
               (distance % day) / hour
            )),
            (document.getElementById("minutes").innerText = Math.floor(
               (distance % hour) / minute
            )),
            (document.getElementById("seconds").innerText = Math.floor(
               (distance % minute) / second
            ));

         //CELEBRATE
         if (distance < 0) {
            document.getElementById("headline").innerText = "I graduated From University!";
            document.getElementById("image").src="./Assets/gradDone.jpg";
            document.getElementById("countdown").style.display = "none";
            document.getElementById("content").style.display = "block";
            document.getElementById("balloons-div").style.display = "block";
            clearInterval(x);
         }
         //seconds
      }, 0);
})();
