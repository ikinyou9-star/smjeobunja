<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>임상연구 참여 대상자 확인하기</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      padding: 45px 20px;
      background-color: #f3f4f6;
      font-family: Arial, "Noto Sans KR", sans-serif;
      color: #222;
    }

    .container {
      width: 100%;
      max-width: 600px;
      margin: 0 auto;
      padding: 48px 30px 30px;
      background-color: #fff;
      border-radius: 13px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.09);
    }

    h1 {
      margin: 5px 0 16px;
      text-align: center;
      font-size: 31px;
      line-height: 1.35;
    }

    .description {
      margin-bottom: 25px;
      color: #666;
      font-size: 16px;
      line-height: 1.7;
    }

    .notice {
      display: inline-block;
      margin-bottom: 6px;
      color: #b42318;
      font-weight: bold;
    }

    .field-label {
      display: block;
      margin-top: 20px;
      margin-bottom: 8px;
      font-size: 16px;
      font-weight: bold;
    }

    input[type="number"] {
      width: 100%;
      padding: 13px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 16px;
    }

    input[type="number"]:focus {
      border-color: #2f6fe4;
      outline: none;
      box-shadow: 0 0 0 3px rgba(47,111,228,0.12);
    }

    .question {
      margin-top: 23px;
      font-weight: bold;
      line-height: 1.5;
    }

    .radio-group {
      margin-top: 12px;
    }

    .radio-option {
      display: block;
      margin: 14px 0;
      font-weight: normal;
      cursor: pointer;
    }

    .radio-option input {
      margin-right: 7px;
    }

    button {
      width: 100%;
      margin-top: 24px;
      padding: 15px;
      border: none;
      border-radius: 7px;
      background-color: #2f6fe4;
      color: #fff;
      font-size: 17px;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      background-color: #255bc1;
    }

    #result {
      display: none;
      margin-top: 24px;
      padding: 20px;
      border-radius: 8px;
      text-align: center;
      font-size: 17px;
      line-height: 1.7;
    }

    .eligible {
      background-color: #eaf8ee;
      border: 1px solid #9bd3aa;
      color: #176b32;
    }

    .not-eligible {
      background-color: #fff0f0;
      border: 1px solid #e5aaaa;
      color: #a32020;
    }

    @media (max-width: 600px) {
      body {
        padding: 20px 12px;
      }

      .container {
        padding: 32px 20px 25px;
      }

      h1 {
        font-size: 25px;
      }
    }
  </style>
</head>

<body>

  <div class="container">

    <h1>임상연구 참여 대상자 확인하기</h1>

    <p class="description">
      <span class="notice">※ 만 나이 기준으로 입력해 주세요.</span><br>
      만 나이, 키, 체중을 입력하고 비만 관련 약물 복용 여부를 선택하면
      BMI를 자동 계산하여 임상연구 참여 대상자 해당 여부를 확인합니다.
    </p>

    <label class="field-label" for="age">만 나이(세)</label>
    <input
      type="number"
      id="age"
      placeholder="예) 35"
      min="0"
      max="120"
      step="1"
    >

    <label class="field-label" for="height">키(cm)</label>
    <input
      type="number"
      id="height"
      placeholder="예) 170"
      min="1"
      step="0.1"
    >

    <label class="field-label" for="weight">체중(kg)</label>
    <input
      type="number"
      id="weight"
      placeholder="예) 75"
      min="1"
      step="0.1"
    >

    <div class="question">
      현재 비만 관련 약물을 복용하거나 처방받고 있습니까?
    </div>

    <div class="radio-group">

      <label class="radio-option">
        <input
          type="radio"
          name="medication"
          value="yes"
        >
        예
      </label>

      <label class="radio-option">
        <input
          type="radio"
          name="medication"
          value="no"
        >
        아니오
      </label>

    </div>

    <button
      type="button"
      onclick="checkEligibility()"
    >
      BMI 계산 및 대상자 확인
    </button>

    <div id="result"></div>

  </div>

  <script>
    function checkEligibility() {

      const ageInput =
        document.getElementById("age").value;

      const heightInput =
        document.getElementById("height").value;

      const weightInput =
        document.getElementById("weight").value;

      const medication =
        document.querySelector(
          'input[name="medication"]:checked'
        );

      const resultBox =
        document.getElementById("result");

      const age = Number(ageInput);
      const height = Number(heightInput);
      const weight = Number(weightInput);

      if (
        ageInput === "" ||
        heightInput === "" ||
        weightInput === "" ||
        age <= 0 ||
        height <= 0 ||
        weight <= 0
      ) {
        alert(
          "만 나이, 키, 체중을 모두 올바르게 입력해주세요."
        );
        return;
      }

      if (!Number.isInteger(age)) {
        alert(
          "만 나이(세)는 정수로 입력해주세요."
        );
        return;
      }

      if (!medication) {
        alert(
          "비만 관련 약물 복용 여부를 선택해주세요."
        );
        return;
      }

      const heightMeter = height / 100;

      const bmi =
        weight / (heightMeter * heightMeter);

      const eligible =
        age >= 19 &&
        age <= 65 &&
        bmi >= 25 &&
        bmi <= 34.9 &&
        medication.value === "no";

      resultBox.style.display = "block";

      if (eligible) {

        resultBox.className = "eligible";

        resultBox.innerHTML =
          "<strong>계산된 BMI: " +
          bmi.toFixed(2) +
          "</strong><br><br>" +
          "✅ 임상연구 참여 대상자에 해당합니다.";

      } else {

        resultBox.className = "not-eligible";

        resultBox.innerHTML =
          "<strong>계산된 BMI: " +
          bmi.toFixed(2) +
          "</strong><br><br>" +
          "❌ 임상연구 참여 대상자에 해당하지 않습니다.";

      }
    }
  </script>

</body>
</html>
