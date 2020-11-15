<template>
<div class="main">
   <ul class="topnav">
  <li><a class="name" href="#home" style="color:white ">MADE UP</a></li>
  <li><a class="active" href="#news">For Me</a></li>
  <li><a href="#contact">Jeans</a></li>
  <li><a href="#news">Shirts</a></li>
   <li><a href="#contact">T-Shirts</a></li>
  <li><a href="#contact">Trousers</a></li>
  <li><a href="#news">Joggers</a></li>
  <li><a href="#contact">Shorts</a></li>
  <li class="right"><a href="#about"><img src="https://png.pngtree.com/png-vector/20190223/ourlarge/pngtree-profile-line-black-icon-png-image_691051.jpg" style="width:40px;margin-top:-10px"></a></li>
  <li class="right"><a href="#about"><img src="data:image/png;base64,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" style="width:40px;margin-top:-10px"></a></li>
<li class="right"><a href="#about"><img src="https://cdn1.iconfinder.com/data/icons/hawcons/32/698956-icon-111-search-512.png" style="width:40px;margin-top:-10px"></a></li>
</ul>
 <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/%D0%9D%D0%B0_%D1%84%D0%BE%D0%BD%D0%B5_%D0%BF%D0%B0%D0%BD%D0%BE%D1%80%D0%B0%D0%BC%D1%8B_%D0%91%D0%B0%D0%BA%D1%83.jpg/1280px-%D0%9D%D0%B0_%D1%84%D0%BE%D0%BD%D0%B5_%D0%BF%D0%B0%D0%BD%D0%BE%D1%80%D0%B0%D0%BC%D1%8B_%D0%91%D0%B0%D0%BA%D1%83.jpg" class="img1">
 <div class="t1"><p style="margin-top:10px"> Clothes that <span style="color:#E10000">respire</span></p></div>
 <div class="t2"><p style="margin-top:10px"> for men who <span style="color:#E10000"> aspire</span></p></div>
 <button class="btn1">BROWSE COLLECTIONS</button>
 <img src="https://www.apetogentleman.com/wp-content/uploads/2018/12/leather-jackets-bomber.jpg" class="img2">
 <div class="t3"><p style="margin-top:10px"> <span style="color:#E10000"> Summer </span> here and</p></div>
 <div class="t4"><p style="margin-top:10px"> so is our <span style="color:#E10000">collection</span></p></div>
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSnRMmEJ2qva7_ogaWiVPcE9saR1fTGJ9E_IB0oe0KHUxIcby3h-zMrwxYaRasIVUq3f_86Ptz17E-2kGtW0oQujPFvBMOxAwiOf_2xY_Q&usqp=CAU&ec=45725305" class="img3">
<div class="t4"><p style="margin-top:10px"> <span style="color:#E10000"> Wrinkle-free</span> t-shirts</p></div>
<img src="https://thumbs.dreamstime.com/b/portrait-man-dressed-stylish-brown-leather-jacket-jeans-backpack-watches-biker-gloves-posing-top-mountain-view-173019178.jpg" class="img4">
<div class="t5"><p style="margin-top:10px"> <span style="color:#E10000"> Stain-free</span> denim shirts</p></div>
<hr class="l1"> 
<p class="t6">LATEST COLLECTIONS</p>
<hr class="l2">
<div class="tra">
  <div class="flex-item-left"><img src="https://previews.123rf.com/images/ravital/ravital1802/ravital180200063/96073491-a-pile-of-different-blue-jeans-fashion-things-from-denim-as-a-background-.jpg" class="img5"><p class="t7">Printed Polo T-Shirt<span class="t8">₹1,499.00</span></p></div>
  <div class="flex-item-right"><img src="https://i.pinimg.com/236x/e0/6a/a3/e06aa3a37008d994dda19198f58c6d33.jpg" class="img6"><p class="t9">Printed Polo T-Shirt<span class="t10">₹1,499.00</span></p></div>
  <div class="flex-item-left"><img src="https://previews.123rf.com/images/ravital/ravital1802/ravital180200063/96073491-a-pile-of-different-blue-jeans-fashion-things-from-denim-as-a-background-.jpg" class="img7"><p class="t11">Printed Polo T-Shirt<span class="t12">₹1,499.00</span></p></div>
  <div class="flex-item-right"><img src="https://i.pinimg.com/236x/e0/6a/a3/e06aa3a37008d994dda19198f58c6d33.jpg" class="img8"><p class="t13">Printed Polo T-Shirt<span class="t14">₹1,499.00</span></p></div>
  <div class="flex-item-left"><img src="https://previews.123rf.com/images/ravital/ravital1802/ravital180200063/96073491-a-pile-of-different-blue-jeans-fashion-things-from-denim-as-a-background-.jpg" class="img9"><p class="t15">Printed Polo T-Shirt<span class="t16">₹1,499.00</span></p></div>
</div>
<div class="rs">
<p class="t17">TESTMONIALS</p>

<div class="rb"> 
<label class="rn">Vikas</label>
<p class="rc">Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was worth the price.</p>
<p></p>
</div>
<img src="https://i.pinimg.com/originals/d9/5b/98/d95b98b33fe717907dcbb3aceed81797.jpg" class="img10">


<div class="rb1"> 
<label class="rn1">Vikas</label>
<p class="rc1">Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was worth the price.</p>
<p></p>
</div>
<img src="https://i.pinimg.com/originals/d9/5b/98/d95b98b33fe717907dcbb3aceed81797.jpg" class="img11">


<div class="rb2"> 
<label class="rn2">Vikas</label>
<p class="rc2">Love the cloth material! So breezy and comfortable. Really durable as well. I must say the jeans I bought was worth the price.</p>
<p></p>
</div>
<img src="https://i.pinimg.com/originals/d9/5b/98/d95b98b33fe717907dcbb3aceed81797.jpg" class="img12">

</div>
<div class="news">
<label class="n1">GET COUPONS & STYLE GUIDES</label>
<label class="n2">Subscribe to our Newsletter</label>
<input type="email" placeholder="   E-mail" style="width: 360px;height: 40px;margin-top:6cm;margin-left:-3cm; font-family:  futura;">
<button class="btn2">SUBSCRIBE</button>
</div>
  <div class="foo">
<div class="column"><div>
  <ul  class="foul">
    <li ><span class="s1"><a href="###" >About Us</a></span> </li><br>
     <li ><a href="###" >Delivery Information </a> </li><br>
      <li><a href="###" >Returns & Exchange </a> </li><br>
       <li ><a href="###" >Technical & Privacy </a></li><br>
        <li ><a href="###" > Order Status</a> </li>
  </ul>
  </div>
  </div>
<div class="column">
<a href="###" class="mu2">
<p class="pp">MADE UP</p>
</a>
<p class="pp1">Stay in touch with us
</p>
<a href="###"><img src="https://i.pinimg.com/originals/b7/63/69/b763699fd1fa3bfb374442593ae642e1.png" style="width:40px;margin-left:30px;margin-top:5cm"></a>
<a href="###"><img src="https://i.pinimg.com/originals/63/9b/3d/639b3dafb544d6f061fcddd2d6686ddb.png" style="width:50px;"></a>
<a href="###"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQ94QnoTUAs8Y74tllt1Us_0ZkQoKADtMG2YUCB58tigId_I0RINkJnuR76BAfWmK36ixw-M3kxuhsxJ3CR9ibObJldeXIpWjeLiiNlHlI&usqp=CAU&ec=45725305" style="width:40px; border-radius:25px"></a>
</div>
<div class="column">
  <p class="fl">Our Corporate Office  
  </p>
  <p class="fla">No: 7,A2B road, Adayar Rajpuram,
    <br> T-Nagar, Chennai - 642002.</p>
    <img src="https://cdn4.iconfinder.com/data/icons/ionicons/512/icon-email-512.png" style="width:20px;margin-left:-240px;margin-top:5cm"><p class="fe"> sales@derbymen.com</p>
    
</div>
  </div>
</div>
</template>
<script>
export default {
  
}
</script>
 <style  scoped>

 /*navbar */

 ul.topnav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #FFFFFF;
  border: 1px solid #DDDDDD;
box-sizing: border-box;
height: 70px;
margin-top: -1.7cm;
}

ul.topnav li {float: left;}

ul.topnav li a {
  display: block;
  color: #444444;
  text-align: center;
  padding: 26px 18px;
  text-decoration: none;
  position: inline;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;


}

.right
{
  margin-left: -20px;
  
}
li {
    margin-left: 30px;
}

.name
{
  background-color: #E10000;
  color: #FFFFFF;
}
ul.topnav li.right {float: right;}
ul.topnav li a.active {color: #E10000;}
.img1
{
  position: absolute;
width: 1348px;
height: 680px;
left: 0px;
top: 70px;
}
.t1
{
    font-family:  futura;
  position: absolute;
width: 182px;
height: 39px;
left: 549px;
top: 396px;
background: #FFFFFF;
opacity: 0.9;
}
.t2
{
    font-family:  futura;
  position: absolute;
width: 182px;
height: 39px;
left: 549px;
top: 445px;
background: #FFFFFF;
opacity: 0.9;
}
.btn1
{
  position: absolute;
width: 240px;
height: 50px;
left: 520px;
top: 572px;
color: #FFFFFF;
background: #E10000;
}
.img2
{
  position: absolute;
width: 635px;
height: 740px;
left: 0px;
top: 757px;
}
.t3
{
  position: absolute;
width: 189px;
height: 39px;
left: 223px;
top: 1086px;
  font-family:  futura;
background: #FFFFFF;
opacity: 0.9;
}
.t4
{
  position: absolute;
width: 176px;
height: 39px;
left: 230px;
top: 1130px;
  font-family:  futura;
background: #FFFFFF;
opacity: 0.9;
}
.img3
{
  position: absolute;
width: 700px;
height: 365px;
left: 645px;
top: 757px;
}
.t4{
  position: absolute;
width: 180.34px;
height: 39px;
left: 872px;
top: 920px;
  font-family:  futura;
background: #FFFFFF;
opacity: 0.9;
}
.img4
{
  
position: absolute;
width: 700px;
height: 365px;
left: 645px;
top: 1132px;

}
.t5
{
  
position: absolute;
width: 197px;
height: 40px;
left: 864px;
top: 1295px;
  font-family:  futura;
background: #FFFFFF;
opacity: 0.9;
}

/*option section*/

.l1
{
  position: absolute;
width: 446px;
height: 0px;
left: 60px;
top: 1569px;

border: 1px solid #DDDDDD;
}
.l2
{
  position: absolute;
width: 448px;
height: 0px;
left: 772px;
top: 1569px;

border: 1px solid #DDDDDD;
}
.t6
{
  position: absolute;
width: 240px;
height: 21px;
left: 520px;
top: 1550px;
  font-family:  Michroma;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 21px;
color: #333333;
}
.img5
{
position: absolute;
width: 222px;
height: 318px;
left: 61px;
top: 1622px;
}
.t7
{
  position: absolute;
width: 113px;
height: 20px;
left: 116px;
top: 1955px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #333333;

}
.t8
{ 
position: absolute;
width: 58px;
height: 19px;
left: 25px;
top:30px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 13px;
line-height: 19px;
color: #E10000;
}
.img6
{
position: absolute;
width: 222px;
height: 318px;
left: 293px;
top: 1622px;
}
.t9
{
  position: absolute;
width: 113px;
height: 20px;
left: 348px;
top: 1955px;
font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;

color: #404040;

}
.t10
{ 
position: absolute;
width: 58px;
height: 19px;
left: 25px;
top:30px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 13px;
line-height: 19px;
color: #E10000;
}
.img7
{

position: absolute;
width: 221.88px;
height: 318px;
left: 525px;
top: 1622px;
}
.t11
{
  position: absolute;
width: 113px;
height: 20px;
left: 580px;
top: 1955px;
font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #333333;

}
.t12
{ 
position: absolute;
width: 58px;
height: 19px;
left: 25px;
top:30px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 13px;
line-height: 19px;
color: #E10000;
}
.img8
{
position: absolute;
width: 222px;
height: 318px;
left: 757px;
top: 1622px;
}
.t13
{
  position: absolute;
width: 113px;
height: 20px;
left: 812px;
top: 1955px;
font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;

color: #333333;

}
.t14
{ 
position: absolute;
width: 58px;
height: 19px;
left: 25px;
top:30px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 13px;
line-height: 19px;
color: #E10000;
}
.img9
{
position: absolute;
width: 222px;
height: 318px;
left: 989px;
top: 1622px;
}
.t15
{
  
position: absolute;
width: 113px;
height: 20px;
left: 1044px;
top: 1955px;
font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;

color: #333333;
}
.t16
{ 
position: absolute;
width: 58px;
height: 19px;
left: 25px;
top:30px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 13px;
line-height: 19px;
color: #E10000;
}
.rs
{
  position: absolute;
width: 1340px;
height: 360px;
left: 0px;
top: 2051px;

background: #F9F9F9;
}
.t17
{
  position: absolute;
width: 172px;
height: 26px;
left: 554px;
top: 35px;

 font-family:  Michroma;
font-style: normal;
font-weight: normal;
font-size: 24px;
line-height: 25px;

color: #333333;
}

/*reviw section*/


.img10
{
  position: absolute;
width: 50px;
height: 50px;
left: 60px;
top: 150px;
border-radius: 43px;
}
.rb
{
  position: absolute;
width: 329px;
height: 137px;
left: 88px;
top:170px;
background: #FFFFFF;
box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.08);
border-radius: 6px;
}
.rn
{
  position: absolute;
width: 32px;
height: 20px;
left: 30px;
top:20px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #404040;
}
.rc
{
  position: absolute;
width: 279px;
height: 60px;
left: 30px;
top:30px;
text-align: left;
font-family: Jost;
font-style: italic;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #707070;
}
.img11
{
  position: absolute;
width: 50px;
height: 50px;
left: 462px;
top: 150px;
border-radius: 43px;
}
.rb1
{
  position: absolute;
width: 329px;
height: 137px;
left: 490px;
top:170px;
background: #FFFFFF;
box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.08);
border-radius: 6px;
}
.rn1
{
  position: absolute;
width: 32px;
height: 20px;
left: 30px;
top:20px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #404040;
}
.rc1
{
  position: absolute;
width: 279px;
height: 60px;
left: 30px;
top:30px;
text-align: left;
font-family: Jost;
font-style: italic;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #707070;
}
.img12
{
  position: absolute;
width: 50px;
height: 50px;
left: 863px;
top: 150px;
border-radius: 43px;
}
.rb2
{
  position: absolute;
width: 329px;
height: 137px;
left: 891px;
top:170px;
background: #FFFFFF;
box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.08);
border-radius: 6px;
}
.rn2
{
  position: absolute;
width: 32px;
height: 20px;
left: 30px;
top:20px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #404040;
}
.rc2
{
  position: absolute;
width: 279px;
height: 60px;
left: 30px;
top:30px;
text-align: left;
font-family: Jost;
font-style: italic;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #707070;
}

/*email section*/

.news
{
  position: absolute;
width: 1340px;
height: 360px;
left: 0px;
top: 2407px;

background: #000000;
opacity: 0.4;
}
.n1
{
position: absolute;
width: 500px;
height: 35px;
left: 435px;
top:110px;
  font-family:  futura;
font-style: normal;
font-weight: 600;
font-size: 24px;
line-height: 35px;
color: #FFFFFF;
}
.n2
{
  position: absolute;
width: 236px;
height: 29px;
left: 563px;
top: 150px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 20px;
line-height: 29px;
color: #FFFFFF;
}
.btn2
{
   font-family:  futura;
  position: absolute;
width: 125px;
height: 40px;
left: 810px;
top: 230px;
background-color: red;
color: #FFFFFF;
}


/* footer*/

.foo
{
  position: absolute;
width: 1340px;
height: 360px;
left: 0px;
top: 2767px;
background: #333333;
}
.column {
  color: white;
  float: left;
 width: 30%;
  padding: 10px;
  height: 360px; 
}
ul.foul
{
  
 list-style-type: none;
 margin-top: 2cm;
}
ul.foul li a {
  
  display: block;
  color: #BBBBBB;
  margin-left: 5cm;
 text-align: left;
  text-decoration: none;
  position: inline;
   font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 24px;
}
.mu2
{
  position: absolute;
width: 115px;
height: 70px;
left: 600.17px;
top: 2cm;
text-align: center;
background: #E10000;
}
.pp
{
  position: absolute;
width: 103px;
height: 25px;
left: 5px;
  font-family:  futura;
font-style: normal;
font-weight: bold;
font-size: 20px;
line-height: 25px;
text-align: center;
color: #FFFFFF;
}
.pp1
{
  position: absolute;
width: 151px;
height: 20px;
left: 580px;
top:4cm;

  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 16px;
line-height: 20px;
color: #BBBBBB;
}
.fl
{
  position: absolute;
width: 128px;
height: 20px;
left: 932px;
top:60px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
color: #DDDDDD;
}
.fla
{
  position: absolute;
width: 218px;
height: 48px;
left: 932px;
top:90px;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 24px;
color: #BBBBBB;
text-align: left;
}
.fe
{
  position: absolute;
width: 129px;
height: 20px;
left: 964px;
margin-top: -0.69cm;
  font-family:  futura;
font-style: normal;
font-weight: normal;
font-size: 14px;
line-height: 20px;
text-align: center;
color: #BBBBBB;
}
 </style>