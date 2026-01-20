<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">



</head>

<body>
    <div class="main">
        <nav>
            <span><img width="53" src="https://www.theverge.com/2016/6/20/11979948/netflix-new-icon-logo"></span>
            <div>
                <button class="btn">English</button>
                <button class="btn btn-red-sm">Sign In</button>
            </div>
        </nav>
        <div class="box">
        </div>
        <div class="hero">
            <span>Enjoy big movies, hit series and more from ₹ 149.</span>
            <span>Join today. Cancel anytime.</span>
            <span>Ready to watch? Enter your email to create or restart your membership.</span>
            <div>
                <input type="text " placeholder="email address">
                <button class="btn-red">Get Started &gt;
                </button>
            </div>
        </div>

    </div>
    <div class="sepration"></div>
    <section class="first">
        <div>
            <span>Enjoy on your TV</span>
            <span>Watch on smart TVs, PlayStation, Xbox, Chromecast, Apple TV, Blu-ray players and more.</span>
        </div>
        <div class="secImg">
            <img src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/tv.png" alt="">
            <video src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/video-tv-in-0819.m4v"
                autoplay loop muted></video>
        </div>
    </section>
    <div class="sepration"></div>
     <section class="first second">
         <div class="secImg">
             <img src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/mobile-0819.jpg" alt="">
             
         </div>
        <div>
             <span>Download your shows to watch offline</span>
            <span>Save your favourites easily and always have something to watch.</span>
        </div>
    </section>
     <div class="sepration"></div>
    <section class="first third">
        <div>
           <span>Watch everywhere</span>
            <span>Stream unlimited movies and TV shows on your phone, tablet, laptop, and TV.</span>
        </div>
        </div>
        <div class="secImg">
            <img src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/tv.png" alt="">
            <video src="https://assets.nflxext.com/ffe/siteui/acquisition/ourStory/fuji/desktop/video-devices-in.m4v"
                autoplay loop muted></video>
        </div>
    </section>
     <div class="sepration"></div>
    <section class="first">
        
        <div class="secImg">
            <img src="https://occ-0-2849-3646.1.nflxso.net/dnm/api/v6/19OhWN2dO19C9txTON9tvTFtefw/AAAABVr8nYuAg0xDpXDv0VI9HUoH7r2aGp4TKRCsKNQrMwxzTtr-NlwOHeS8bCI2oeZddmu3nMYr3j9MjYhHyjBASb1FaOGYZNYvPBCL.png?r=54d" alt="">
            
               
        </div>
         <div>
            <span>Create profiles for kids</span>
            <span>Send children on adventures with their favourite characters in a space made just for them—free with
                your membership.</span>
        </div>
    </section>
    <div class="sepration"></div>
    <section class="faq">
        <h2>Frequently Asked Question</h2>
        <div class="faqbox">
        <span>What is Netflix</span>
        <svg width="24" height="0 0 24 24" fill="none"  xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
        <div class="faqbox">
        <span>How much does Netflix cost?</span>
        <svg width="24" height="0 0 24 24" fill="none"  xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
        <div class="faqbox">
        <span>What can I watch on Netflix?</span>
        <svg width="24" height="0 0 24 24" fill="none"  xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
        <div class="faqbox">
        <span>Where can I watch?</span>
        <svg width="24" height="0 0 24 24" fill="none"  xmlns="http://www.w3.org/2000/svg"></svg>
        </div>
    </section>
    <div class="sepration"></div>
    <script>
        const btn = document.querySelector(".btn-red");
        const input = document.querySelector("input");
      
        btn.addEventListener("click", () => {
          const email = input.value.trim();
      
          if (email === "") {
            alert("Please enter email");
            return;
          }
      
          // simple email validation
          const pattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
          if (!pattern.test(email)) {
            alert("Enter valid email");
            return;
          }
      
          // store email (acts like backend)
          let users = JSON.parse(localStorage.getItem("users")) || [];
          users.push(email);
          localStorage.setItem("users", JSON.stringify(users));
      
          alert("Email registered successfully!");
          input.value = "";
        });
      </script>
</body>

</html>
