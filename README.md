<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">

<style>
	*{
    padding: 0;
    margin: 0;
 }
 body{
    background-color: black;
 }
    .main{
    background-image: url("https://raw.githubusercontent.com/CodeWithHarry/Sigma-Web-Dev-Course/refs/heads/main/Video%2053/assets/images/bg.jpg");
    height: 644px;
    background-position: center center;
    background-size: max(1200px, 100vw);
    background-repeat: no-repeat;
position: relative;
}
  .main .box {
    height: 644px;
    width: 100%;
    opacity: 0.69;
    position: absolute;
    top: 0;
    background-color: black;
}

nav {
    max-width: 60vw;
    justify-content: space-between;
    margin: auto;
    display: flex;
    align-items: center;
    height: 100px;
    position: relative;
    z-index: 10;
}

nav  img {
    height: 100px;
    color: red;
    width: 130px;
    position: relative;
    z-index: 10;
}
.hero{
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    height: calc(100% - 100px);
    gap: 23px;
    padding: 0 30px;
    position: relative;
    z-index: 10;
    font-family: martal system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    gap:  20px;
}
.btn{
    color: white;
    padding: 3px 8px;
    font-weight: bold;
    background-color: rgba(248, 243, 243, 0.021);
    border: 1px solid white;
    border-radius: 4px;
    cursor: pointer;

}

.hero> :nth-child(1){
    font-size: 44px;
    font-weight: 900;
    text-align: center;
}
.sepration{
    height: 5px;
    background-color: rgb(59, 57, 57);
    opacity: 0.9;
}
.btn-red{
    background-color: red;
    color: white;
    padding: 3px 8px;
    font-size: 20px;
    border-radius: 4px;
    font-weight: 400;
}
.main input{
    padding: 3px 24px;
    font-size: 20px;
    border-radius: 4px;
    background-color: rgba(23, 23, 23, 0.7);
    color: white;
}
.btn-red-sm{
    background-color: #fb0606;
    color: white;
}
.first{
    display: flex;
    justify-content: center;
    max-width: 70vw;
    margin: auto;
    color: white;
    align-items: center;
}
.secImg{
    position: relative;
}
.secImg img{
    width: 555px;
    position: relative;
   margin-top: 20%;
   z-index:1;
    
}

.secImg video{
    position: absolute;
    top: 234px;
    right: 81px;
    width: 401px;
    z-index:0 ;
}


section.first > div{
    display: flex;
    flex-direction: column;
    padding: 34px 0;
}
section.first > div :first-child{
    font-size: 48px;
    font-weight: bolder;
}
section.first > div :nth-child(2){
    font-size: 24px;
    
}
.faq h2 {
    text-align: center;
    font-size: 48px;
}

.faq {
    background: black;
    color: white;
    padding: 34px;
}
.faqbox:hover{
    background-color: rgb(94, 100, 104);
}
.faqbox {
    transition: all 1s ease-out;
    font-size: 20px;
    display: flex;
    justify-content: space-between;
    background-color: #2d2d2d;
    padding: 24px;
    max-width: 60vw;
    margin: 34px auto;
    cursor: pointer;
    height: 30px;
}
</style>



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
