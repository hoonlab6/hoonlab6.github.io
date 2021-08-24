---
layout: page
title: Hoon Lab at Pharmacy, SKKU
permalink: /
---

# Welcome to Hoon Lab

### Our lab is Computational Biomedicine [@hoonbiolab](https://twitter.com/hoonbiolab).

<head>
<link href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@700&display=swap" rel="stylesheet">
<style>
body {
    font-family: 'Noto Sans', sans-serif; font-size: 22px;
}
.wrapper {
    display:flex;
    flex-direction:row;
    flex-wrap:wrap;
    justify-content:center;
}
.box {
    background-color: #fafafa;
    box-shadow: 0px 2px 2px rgba(0,0,0,.2), 0px 0px 2px rgba(0,0,0,.2);
    width: 100%;
    border-radius: 2px;
    margin:20px;
    display:flex;
    flex-direction:column;
    cursor:pointer;
}
.box:hover {
    box-shadow: 0px 15px 20px rgba(0,0,0,.25),0px 0px 30px rgba(0,0,0,.1);
}
.box .text {
    padding: 24px;
}
.box .bb {
    border: 1px solid red;
}
.box .title {
    color:  black;
    font-weight: 500;
    font-size: 20px;
    margin-top: -2px;
    margin-bottom: 16px;
}
.box p {
    color: rgba(0,0,0,.5);
    font-size: 16px;
    line-height: 24px;
    margin: 0px;
}
.box .act {
    padding: 8px 0;
    text-align: right;
}
.card-button {
    text-transform: uppercase;
    display: inline-block;
    font-size: 13px;
    padding: 12px 10px;
    color: #00a5ef;
    font-weight: 500;
    margin-right: 8px;
    cursor: pointer;
}
</style>
<head>


<h2>Rescent News</h2>
<div class="wrapper">
  {% for service in site.data.metadata.services %}<div class="box">
  <div class="text">
    <div class="title">{{ service.name }}</div>
      <p><img src="{{ service.logo }}" style="height:140px; position:absolute">
       <span style="width:50%; float:right">{{ service.description }}</span>
      </p>
    </div>
    <div class="act">
	<a href="{{ service.url }}" target="_blank"><div class="card-button">Documentation</div></a>
    </div>
  </div>{% endfor %}
</div>

<h2>Resources</h2>
<div class="wrapper">
  {% for resource in site.data.metadata.resources %}<div class="box">
  <div class="text">
    <div class="title">{{ resource.name }}</div>
      <p><img src="{{ resource.logo }}" style="height:160px; position:absolute">
       <span style="width:50%; float:right">{{ resource.description }}</span>
      </p>
    </div>
    <div class="act">
	<a href="{{ resource.url }}" target="_blank"><div class="card-button">Documentation</div></a>
    </div>
  </div>{% endfor %}
</div>

<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.button {
  padding: 12px 20px;
  font-size: 22px;
  text-align: center;
  cursor: pointer;
  outline: none;
  color: #fff;
  background-color: #1E2D6A;
  border: none;
  border-radius: 15px;
  box-shadow: 0 9px #999;
}
.button:hover {background-color: #1E2D6A}
.button:active {
  background-color: #1E2D6A;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
</style>
</head>
<body>

<button class="button"><a href='https://photos.google.com/u/0/share/AF1QipP5EpeeFRyzUYlB05eRdj0uSO-OLeG7xh4LmiYNmyp2ULNzuxmsR5TXkR3aWW_oKQ?key=WVVKUUhyZExyMndIcnVlNTBUekhjdDlkdThDcjJ3'>Click Here</a></button> to learn more about our lab

</body>


