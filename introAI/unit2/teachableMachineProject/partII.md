<style>
    table body {
      font-family: Arial, Helvetica, sans-serif;
      line-height: 1.5;
      max-width: 900px;
      margin: 0 auto;
      padding: 30px 20px;
      color: #222;
      background: #fff;
    }

    table h1 {
      margin-bottom: 0;
      font-size: 2em;
    }

    table h2 {
      margin-top: 0;
      color: #555;
      font-size: 1.35em;
      font-weight: normal;
    }

    table h3 {
      margin-top: 30px;
      margin-bottom: 8px;
    }

    .student-info {
      margin: 25px 0;
      font-size: 1.05em;
    }

    .student-info p {
      margin: 10px 0;
    }

    .instructions {
      background: #f5f5f5;
      border-left: 5px solid #888;
      padding: 12px 16px;
      margin: 20px 0 25px 0;
    }

    .instructions p {
      margin: 6px 0;
    }

    .keep-going {
      background: #f5f5f5;
      border: 1px solid #ccc;
      border-radius: 6px;
      padding: 15px 18px;
      margin: 25px 0;
    }

    .keep-going h3 {
      margin-top: 0;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin: 15px 0 25px 0;
    }

    th,
    td {
      border: 1px solid #999;
      padding: 10px;
    }

    th {
      background: #eee;
      text-align: center;
    }

    td {
      height: 32px;
    }

    th:first-child,
    td:first-child {
    width: 7%;
    text-align: center;
    }

    th:nth-child(2),
    td:nth-child(2) {
    width: 33%;
    }

    th:nth-child(3),
    td:nth-child(3) {
    width: 20%;
    }

    th:nth-child(4),
    td:nth-child(4) {
    width: 20%;
    }

    th:nth-child(5),
    td:nth-child(5) {
    width: 20%;
    text-align: center;
    }
    .results {
      margin-top: 30px;
    }

    .result-line {
      margin: 18px 0;
      font-size: 1.05em;
    }

    .line {
      display: inline-block;
      min-width: 100px;
      border-bottom: 1px solid #222;
      margin-left: 5px;
    }

    @media print {
      table body {
        max-width: none;
        padding: 0;
        font-size: 11pt;
      }

      table h1 {
        font-size: 20pt;
      }

      table h2 {
        font-size: 14pt;
      }

      .instructions,
      .keep-going {
        background: white;
      }

      table {
        page-break-inside: avoid;
      }

      tr {
        page-break-inside: avoid;
      }

      .keep-going {
        page-break-inside: avoid;
      }
    }

    @media (max-width: 600px) {
      table body {
        padding: 20px 12px;
      }

      table {
        font-size: 0.9em;
      }

      th,
      td {
        padding: 7px 5px;
      }

      th:last-child,
      td:last-child {
        width: 25%;
      }
    }
</style>
  
<div class="title">
    <h1>
        Machine Learning Experiment
    </h1>
    <div class="print-on">
        <strong>Names:</strong>&nbsp;<span>&nbsp;</span>
    </div>
</div>

## Part 2: Train & Test

Now it's time to run your experiment!

Your goal is to train your model and find out **how accurately it can classify new examples.**

---

## 1. Train Your Model

Train your model using the categories you planned in Part 1.

Remember: **Consider both quantity and quality of training examples.** Your examples should include meaningful variation.

### What types of variation did you include?

☐ Different examples
☐ Different positions
☐ Different angles
☐ Different distances
☐ Different backgrounds
☐ Different lighting
☐ Other: _________________________________________________

### Briefly describe your training data.

What did you do to make sure your training examples were varied?

<br><br><br>
<br><br><br>

## 2. Test Your Model

Now test your model using **new examples that were NOT used for training.** Record your results on the back of this page. For this experiment, **a prediction is correct** if the category with the highest probability matches the actual category.

---

## 3. Calculate Your Results

**Number of correct predictions:** _______

**Total number of tests:** _______

**Accuracy:** _______%

### Compare With Your Prediction

In Part 1, you predicted that your model would be:

**Predicted accuracy:** _______%

**Actual accuracy:** _______%

---

<div class="break"></div>

<table>
  <thead>
    <tr>
      <th>Test</th>
      <th>Test Example</th>
      <th>Actual Category</th>
      <th>Model Prediction</th>
      <th>Correct?</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>2</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>3</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>4</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>5</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>6</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>7</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>8</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>9</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>10</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>11</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>12</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>13</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>14</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
    <tr><td>15</td><td></td><td></td><td></td><td>☐ Yes &nbsp; ☐ No</td></tr>
  </tbody>
</table>
