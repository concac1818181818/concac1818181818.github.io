<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <title>Trái Tim Khoa 3D</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: radial-gradient(circle at center, #ffdde1, #ee9ca7);
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      font-family: Arial, sans-serif;
    }

    .heart-container {
      position: relative;
      width: 200px;
      height: 180px;
      animation: pulse 1.5s infinite;
      transform-style: preserve-3d;
    }

    .heart {
      position: absolute;
      top: 0;
      left: 0;
      width: 200px;
      height: 180px;
      background-color: #ff4d6d;
      clip-path: path('M100,30 A40,40 0 1,1 60,90 Q100,140 140,90 A40,40 0 1,1 100,30');
      transform: rotateX(25deg) rotateY(0deg) rotateZ(0deg);
      box-shadow: 0 15px 30px rgba(0,0,0,0.3);
    }

    .heart-text {
      position: absolute;
      width: 100%;
      text-align: center;
      top: 65px;
      font-size: 28px;
      font-weight: bold;
      color: white;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.4);
      transform: translateZ(40px);
    }

    @keyframes pulse {
      0% { transform: scale(1) rotateX(20deg); }
      50% { transform: scale(1.05) rotateX(25deg); }
      100% { transform: scale(1) rotateX(20deg); }
    }
  </style>
</head>
<body>
  <div class="heart-container">
    <div class="heart"></div>
    <div class="heart-text">Khoa</div>
  </div>
</body>
</html>
