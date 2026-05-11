<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>中華健言社 100 期會外會 報名表</title>

  <style>
    *{
      box-sizing:border-box;
      margin:0;
      padding:0;
      font-family:"Noto Sans TC","Microsoft JhengHei",sans-serif;
    }

    body{
      background:linear-gradient(180deg,#fff7f0 0%,#ffffff 100%);
      color:#333;
      padding:20px;
    }

    .container{
      max-width:480px;
      margin:0 auto;
      background:#ffffff;
      border-radius:20px;
      overflow:hidden;
      box-shadow:0 8px 24px rgba(0,0,0,0.08);
    }

    .header{
      background:linear-gradient(135deg,#ff8c42,#ffb26b);
      color:#fff;
      padding:28px 24px;
      text-align:center;
    }

    .header h1{
      font-size:28px;
      margin-bottom:10px;
      line-height:1.4;
    }

    .header p{
      font-size:15px;
      line-height:1.8;
    }

    .content{
      padding:24px;
    }

    .info-box{
      background:#fff4ea;
      border-left:5px solid #ff8c42;
      border-radius:12px;
      padding:16px;
      margin-bottom:24px;
      line-height:1.8;
      font-size:15px;
    }

    .form-group{
      margin-bottom:20px;
    }

    label{
      display:block;
      margin-bottom:8px;
      font-weight:700;
      color:#e36b1f;
    }

    input,
    select{
      width:100%;
      padding:14px;
      border:1px solid #ddd;
      border-radius:12px;
      font-size:16px;
      background:#fff;
      transition:0.2s;
    }

    input:focus,
    select:focus{
      border-color:#ff8c42;
      outline:none;
      box-shadow:0 0 0 3px rgba(255,140,66,0.2);
    }

    .radio-group{
      display:flex;
      gap:12px;
      flex-wrap:wrap;
    }

    .radio-card{
      flex:1;
      min-width:120px;
    }

    .radio-card input{
      display:none;
    }

    .radio-card label{
      display:block;
      text-align:center;
      padding:14px;
      border:2px solid #ffd0ad;
      border-radius:14px;
      background:#fffaf5;
      cursor:pointer;
      transition:0.2s;
      color:#555;
    }

    .radio-card input:checked + label{
      background:#ff8c42;
      color:#fff;
      border-color:#ff8c42;
    }

    .note{
      font-size:13px;
      color:#888;
      margin-top:6px;
      line-height:1.6;
    }

    button{
      width:100%;
      padding:16px;
      border:none;
      border-radius:14px;
      background:linear-gradient(135deg,#ff8c42,#ff6b00);
      color:#fff;
      font-size:18px;
      font-weight:bold;
      cursor:pointer;
      transition:0.2s;
      margin-top:10px;
    }

    button:hover{
      transform:translateY(-2px);
      box-shadow:0 6px 16px rgba(255,107,0,0.25);
    }

    .footer{
      text-align:center;
      padding:18px;
      color:#999;
      font-size:13px;
    }

    @media (max-width:480px){
      .header h1{
        font-size:24px;
      }
    }
  </style>
</head>

<body>

  <div class="container">

    <div class="header">
      <h1>中華健言社<br>100 期會外會</h1>
      <p>
        2026/10/10（六）09:00–16:00<br>
        新城風糖休閒園區
      </p>
    </div>

    <div class="content">

      <div class="info-box">
        <strong>活動費用</strong><br>
        會員：550 元<br>
        非會員：700 元（含保險）
      </div>

      <form>

        <div class="form-group">
          <label for="name">姓名</label>
          <input type="text" id="name" placeholder="請輸入姓名" required>
        </div>

        <div class="form-group">
          <label for="phone">手機</label>
          <input type="tel" id="phone" placeholder="請輸入手機號碼" required>
        </div>

        <div class="form-group">
          <label for="idno">身分證字號</label>
          <input type="text" id="idno" placeholder="請輸入身分證字號" required>
          <div class="note">
            備註：僅供保險投保使用
          </div>
        </div>

        <div class="form-group">
          <label for="club">所屬社團</label>
          <select id="club" required>
            <option value="">請選擇社團</option>
            <option>諄言社</option>
            <option>三重社</option>
            <option>三峽社</option>
            <option>鶯歌社</option>
            <option>竹北社</option>
            <option>新竹社</option>
            <option>中壢社</option>
            <option>湖口社</option>
          </select>
        </div>

        <div class="form-group">
          <label>餐點選擇</label>

          <div class="radio-group">

            <div class="radio-card">
              <input type="radio" id="meat" name="meal" value="葷食" checked>
              <label for="meat">葷食</label>
            </div>

            <div class="radio-card">
              <input type="radio" id="veg" name="meal" value="素食">
              <label for="veg">素食</label>
            </div>

          </div>
        </div>

        <button type="submit">立即報名</button>

      </form>

    </div>

    <div class="footer">
      中華健言社 100 期會外會
    </div>

  </div>

</body>
</html>
