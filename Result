<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <title>ফলাফল খুঁজুন</title>
  <style>
    body { font-family: 'SolaimanLipi', sans-serif; background: #f4f4f4; padding: 20px; text-align: center; }
    input, button { padding: 10px; font-size: 16px; margin: 5px; }
    #resultArea { margin-top: 20px; background: #fff; padding: 20px; border-radius: 10px; display: inline-block; text-align: left; }
  </style>
</head>
<body>
  <h1>রোল নম্বর দিয়ে ফলাফল খুঁজুন</h1>
  <input type="text" id="rollInput" placeholder="রোল নম্বর লিখুন">
  <button onclick="searchResult()">খুঁজুন</button>

  <div id="resultArea"></div>

  <script>
    const results = {
      "101": {
        নাম: "আব্দুল কাইয়ুম",
        বাংলা: ৮০,
        ইংরেজি: ৭৫,
        গণিত: ৯০,
        মোট: ২৪৫,
        গ্রেড: "A+"
      },
      "102": {
        নাম: "ফারিয়া ইয়াসমিন",
        বাংলা: ৭৫,
        ইংরেজি: ৭০,
        গণিত: ৮০,
        মোট: ২২৫,
        গ্রেড: "A"
      },
      "103": {
        নাম: "জুবায়ের হোসাইন",
        বাংলা: ৬৫,
        ইংরেজি: ৬০,
        গণিত: ৭০,
        মোট: ১৯৫,
        গ্রেড: "B"
      }
    };

    function searchResult() {
      const roll = document.getElementById("rollInput").value.trim();
      const data = results[roll];

      const area = document.getElementById("resultArea");
      if (data) {
        area.innerHTML = `
          <h3>রোল: ${roll}</h3>
          <p><strong>নাম:</strong> ${data.নাম}</p>
          <p><strong>বাংলা:</strong> ${data.বাংলা}</p>
          <p><strong>ইংরেজি:</strong> ${data.ইংরেজি}</p>
          <p><strong>গণিত:</strong> ${data.গণিত}</p>
          <p><strong>মোট নম্বর:</strong> ${data.মোট}</p>
          <p><strong>গ্রেড:</strong> ${data.গ্রেড}</p>
        `;
      } else {
        area.innerHTML = `<p style="color: red;">এই রোল নম্বরের কোনো ফলাফল পাওয়া যায়নি।</p>`;
      }
    }
  </script>
</body>
</html>
