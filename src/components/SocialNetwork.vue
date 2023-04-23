<template>
  <head class="container-principal">
    <link
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="./style.css" />
  </head>

  <div class="whats-float">
    <a href="https://api.whatsapp.com/send?phone=50379232974" target="_blank">
      <i class="fa fa-whatsapp"></i
      ><span>Dialecpro<br /><small>Jaime Navas</small></span>
    </a>
  </div>

  <div class="instagram-float instagram">
    <a href="https://www.instagram.com/dielecpro/" target="_blank">
      <i class="fa fa-instagram mr-2"></i
      ><span>Dialecpro<br /><small>Jaime Navas</small></span>
    </a>
  </div>
</template>

<script></script>

<style scoped>
  @media screen and (min-width: 768px) {

    
    h1 {
      color: #fff;
      font-size: 3.625em;
      text-align: center;
      margin-top: 20%;
    }

    .whats-float {
      position: fixed;
      transform: translate(108px, 0px);
      top: 25%;
      right: 0;
      width: 150px;
      overflow: hidden;
      background-color: #25d366;
      color: #fff;
      border-radius: 2px 0 0 2px;
      z-index: 10;
      transition: all 0.5s ease-in-out;
      vertical-align: middle;
    }
    .whats-float a span {
      color: white;
      font-size: 15px;
      padding-top: 8px;
      padding-bottom: 10px;
      position: absolute;
      line-height: 16px;
      font-weight: bolder;
    }

    .whats-float i {
      font-size: 30px;
      color: white;
      line-height: 30px;
      padding: 10px;
      transform: rotate(0deg);
      transition: all 0.5s ease-in-out;
      text-align: center;
    }

    .whats-float:hover {
      color: #ffffff;
      transform: translate(0px, 0px);
    }

    .whats-float:hover i {
      transform: rotate(360deg);
    }

    .instagram-float {
      position: fixed;
      transform: translate(108px, 0px);
      top: 32%;
      right: 0;
      width: 150px;
      overflow: hidden;
      background-color: #2b25d3;
      color: #fff;
      border-radius: 2px 0 0 2px;
      z-index: 10;
      transition: all 0.5s ease-in-out;
      vertical-align: middle;
    }
    .instagram-float a span {
      color: white;
      font-size: 15px;
      padding-top: 8px;
      padding-bottom: 10px;
      position: absolute;
      line-height: 16px;
      font-weight: bolder;
    }

    .instagram-float i {
      font-size: 30px;
      color: white;
      line-height: 30px;
      padding: 10px;
      transform: rotate(0deg);
      transition: all 0.5s ease-in-out;
      text-align: center;
    }

    .instagram-float:hover {
      color: #ffffff;
      transform: translate(0px, 0px);
    }

    .instagram-float:hover i {
      transform: rotate(360deg);
    }

    .instagram {
      background: #f09433;
      background: -moz-linear-gradient(
        45deg,
        #f09433 0%,
        #e6683c 25%,
        #dc2743 50%,
        #cc2366 75%,
        #bc1888 100%
      );
      background: -webkit-linear-gradient(
        45deg,
        #f09433 0%,
        #e6683c 25%,
        #dc2743 50%,
        #cc2366 75%,
        #bc1888 100%
      );
      background: linear-gradient(
        45deg,
        #f09433 0%,
        #e6683c 25%,
        #dc2743 50%,
        #cc2366 75%,
        #bc1888 100%
      );
      filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f09433', endColorstr='#bc1888',GradientType=1 );
    }
  }

  @media screen and (max-width: 768px) {
    .container-principal {
      display: none;
    }

    .whats-float {
        display: none;
    }
    .whats-float a span {
        display: none;
    }

    .whats-float i {
        display: none;
    }

    .whats-float:hover {
        display: none;
    }

    .whats-float:hover i {
        display: none;
    }

    .instagram-float {
        display: none;
    }
    .instagram-float a span {
        display: none;
    }

    .instagram-float i {
        display: none;
    }
  }
</style>
