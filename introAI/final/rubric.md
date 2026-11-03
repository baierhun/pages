<style>
  .ai-rubric {
    --border: #d5dce5;
    --ink: #243247;
    color: var(--ink);
    font-family: Arial, sans-serif;
    line-height: 1.5;
    margin: 1.5rem 0;
  }

  .ai-rubric .table-scroll {
    overflow-x: auto;
    border: 1px solid var(--border);
    border-radius: 10px;
    margin-bottom: 1.5rem;
  }

  .ai-rubric table {
    width: 100%;
    border-collapse: collapse;
  }

  .ai-rubric caption {
    padding: 14px 16px;
    background: #f1f5f9;
    font-size: 1.1rem;
    font-weight: 700;
    text-align: left;
  }

  .ai-rubric th,
  .ai-rubric td {
    padding: 14px;
    border-bottom: 1px solid var(--border);
    border-right: 1px solid var(--border);
    text-align: left;
    vertical-align: top;
  }

  .ai-rubric tr > :last-child {
    border-right: 0;
  }

  .ai-rubric tbody tr:last-child > * {
    border-bottom: 0;
  }

  .ai-rubric thead th {
    background: #243247;
    color: white;
    font-size: 0.9rem;
  }

  .ai-rubric .criteria {
    min-width: 1050px;
    table-layout: fixed;
    font-size: 0.9rem;
  }

  .ai-rubric .criteria thead th:first-child {
    width: 17%;
  }

  .ai-rubric .criteria tbody th {
    background: #f1f5f9;
    font-weight: 700;
  }

  .ai-rubric .maximum {
    display: block;
    margin-top: 6px;
    color: #526176;
    font-size: 0.8rem;
    font-weight: 400;
  }

  .ai-rubric .points {
    display: inline-block;
    margin-bottom: 8px;
    padding: 2px 9px;
    border: 1px solid currentColor;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 700;
  }

  .ai-rubric .criteria tbody td:nth-child(2) { background: #edf8f1; }
  .ai-rubric .criteria tbody td:nth-child(3) { background: #eef5fd; }
  .ai-rubric .criteria tbody td:nth-child(4) { background: #fff9e9; }
  .ai-rubric .criteria tbody td:nth-child(5) { background: #fff2e9; }
  .ai-rubric .criteria tbody td:nth-child(6) { background: #fdf0f0; }

  .ai-rubric .grades {
    max-width: 440px;
  }

  .ai-rubric .grades th,
  .ai-rubric .grades td {
    padding: 9px 16px;
  }

  .ai-rubric .grades tbody th {
    width: 50%;
    font-weight: 400;
  }

  .ai-rubric .grades tbody td {
    font-weight: 700;
  }

  .ai-rubric .grades tbody tr:nth-child(even) {
    background: #f8fafc;
  }

  .ai-rubric .note {
    padding: 12px 16px;
    border-left: 4px solid #526d96;
    background: #f1f5f9;
  }

  @media print {
    .ai-rubric {
      font-size: 9pt;
      print-color-adjust: exact;
      -webkit-print-color-adjust: exact;
    }

    .ai-rubric .table-scroll {
      overflow: visible;
      border-radius: 0;
    }

    .ai-rubric .criteria {
      min-width: 0;
      font-size: 8pt;
    }

    .ai-rubric th,
    .ai-rubric td {
      padding: 7px;
    }

    .ai-rubric tr {
      break-inside: avoid;
    }

    .ai-rubric thead {
      display: table-header-group;
    }
  }

    .ai-rubric,
    .ai-rubric .table-scroll {
        width: 100%;
        max-width: 100%;
        box-sizing: border-box;
    }

    .ai-rubric .criteria {
        width: 100%;
        min-width: 0;
        table-layout: fixed;
    }

    .ai-rubric th,
    .ai-rubric td {
        padding: 8px;
        overflow-wrap: anywhere;
    }

    .ai-rubric .grades {
        max-width: 440px;
    }
</style>

<div class="ai-rubric">
  <h2>🎬 AI Creative Studio Project Rubric</h2>

  <p>
    Your grade reflects <strong>what you create, how you use AI, and how you
    develop your work over time</strong>. You can earn up to
    <strong>40 points</strong>.
  </p>

  <div class="table-scroll" role="region"
       aria-label="Project rubric" tabindex="0">
    <table class="criteria">
      <caption>Project Criteria · 40 Points Total</caption>
      <thead>
        <tr>
          <th scope="col">Category</th>
          <th scope="col">Excellent</th>
          <th scope="col">Strong</th>
          <th scope="col">Developing</th>
          <th scope="col">Limited</th>
          <th scope="col">Insufficient</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row">
            Creative Direction &amp; Final Product
            <span class="maximum">10 points possible</span>
          </th>
          <td>
            <span class="points">10 points</span><br>
            Your project has a clear purpose, feels complete, and shows your
            personality through thoughtful creative choices.
          </td>
          <td>
            <span class="points">8 points</span><br>
            Your idea is clear and your project is mostly finished. Some parts
            need more development or polish.
          </td>
          <td>
            <span class="points">6 points</span><br>
            Your idea is understandable, but the project is uneven or partly
            unfinished.
          </td>
          <td>
            <span class="points">4 points</span><br>
            Your idea needs more development, or large parts are unfinished
            or disconnected.
          </td>
          <td>
            <span class="points">0 points</span><br>
            You submit little or no meaningful finished work.
          </td>
        </tr>
        <tr>
          <th scope="row">
            Use of Multiple AI Types
            <span class="maximum">5 points possible</span>
          </th>
          <td>
            <span class="points">5 points</span><br>
            You use at least two different AI types repeatedly and purposefully.
            Each contributes meaningfully to your finished project.
          </td>
          <td>
            <span class="points">4 points</span><br>
            You use at least two different AI types more than once per tool.
            Both contribute, but they could work together more effectively.
          </td>
          <td>
            <span class="points">3 points</span><br>
            You use at least two AI types, but one has a minor role or shows
            little back-and-forth development.
          </td>
          <td>
            <span class="points">2 points</span><br>
            You use only one AI type, or rely mainly on single prompts
            without follow-up.
          </td>
          <td>
            <span class="points">0 points</span><br>
            You do not demonstrate meaningful AI use.
          </td>
        </tr>
        <tr>
          <th scope="row">
            Revision &amp; Problem-Solving
            <span class="maximum">10 points possible</span>
          </th>
          <td>
            <span class="points">10 points</span><br>
            You identify weak outputs and make purposeful improvements through
            revised prompts, editing, or rebuilding. Your evidence clearly
            shows improvement.
          </td>
          <td>
            <span class="points">8 points</span><br>
            You make useful revisions, though some weaknesses still
            need attention.
          </td>
          <td>
            <span class="points">6 points</span><br>
            You make some revisions, but they are mostly small changes or
            leave obvious problems unresolved.
          </td>
          <td>
            <span class="points">4 points</span><br>
            You make few meaningful revisions and mostly accept AI outputs
            as they are.
          </td>
          <td>
            <span class="points">0 points</span><br>
            You show no evidence of revision or problem-solving.
          </td>
        </tr>
        <tr>
          <th scope="row">
            Process &amp; Sustained Effort
            <span class="maximum">10 points possible</span>
          </th>
          <td>
            <span class="points">10 points</span><br>
            Your evidence clearly shows planning, experimentation, and progress
            across multiple work sessions. Your decisions are easy to follow.
          </td>
          <td>
            <span class="points">8 points</span><br>
            Your evidence shows work across multiple sessions, with a few gaps
            in documenting your progress.
          </td>
          <td>
            <span class="points">6 points</span><br>
            You provide some evidence, but it is difficult to follow how your
            project developed over time.
          </td>
          <td>
            <span class="points">4 points</span><br>
            You provide very little evidence of your process or work across
            multiple sessions.
          </td>
          <td>
            <span class="points">0 points</span><br>
            You submit no meaningful process evidence.
          </td>
        </tr>
        <tr>
          <th scope="row">
            Presentation &amp; Reflection
            <span class="maximum">5 points possible</span>
          </th>
          <td>
            <span class="points">5 points</span><br>
            You clearly explain what you made and why, how you used each AI
            type, and a specific problem you solved or worked around.
          </td>
          <td>
            <span class="points">4 points</span><br>
            You explain all required elements, but some details could be
            clearer or more specific.
          </td>
          <td>
            <span class="points">3 points</span><br>
            One required element is missing, or several explanations are vague.
          </td>
          <td>
            <span class="points">2 points</span><br>
            Your explanation is minimal and leaves out several required elements.
          </td>
          <td>
            <span class="points">0 points</span><br>
            You do not present or provide a meaningful explanation of your work.
          </td>
        </tr>
      </tbody>
    </table>
  </div>

  <p>
    Add the points earned in all five categories, then use the table below
    to find your final letter grade.
  </p>

  <div class="table-scroll grades">
  <table>
    <caption>Final Letter Grade</caption>
    <thead>
      <tr>
        <th scope="col">Total Points</th>
        <th scope="col">Letter Grade</th>
      </tr>
    </thead>
    <tbody>
      <tr><th scope="row">39–40</th><td>A+</td></tr>
      <tr><th scope="row">37–38</th><td>A</td></tr>
      <tr><th scope="row">35–36</th><td>A−</td></tr>
      <tr><th scope="row">33–34</th><td>B+</td></tr>
      <tr><th scope="row">31–32</th><td>B</td></tr>
      <tr><th scope="row">29–30</th><td>B−</td></tr>
      <tr><th scope="row">27–28</th><td>C+</td></tr>
      <tr><th scope="row">25–26</th><td>C</td></tr>
      <tr><th scope="row">23–24</th><td>C−</td></tr>
      <tr><th scope="row">21–22</th><td>D+</td></tr>
      <tr><th scope="row">19–20</th><td>D</td></tr>
      <tr><th scope="row">16–18</th><td>D−</td></tr>
      <tr><th scope="row">0–15</th><td>F</td></tr>
    </tbody>
  </table>
</div>

  <p class="note">
    <strong>Remember:</strong> Two tools that perform the same function count
    as one AI type. Repeated use should show development or revision. Your
    process evidence must demonstrate work across multiple sessions; a polished
    final product does not replace that evidence.
  </p>
</div>
