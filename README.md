Index.html<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NoorLight Muslim Companion App</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Nunito:400,700">
  <style>
    :root {
      --primary: #009688;
      --accent: #ffd600;
      --background: #f5f9fa;
      --card: #ffffff;
      --text: #212121;
      --shadow: 0 8px 32px #0002;
    }
    [data-theme="dark"] {
      --primary: #23272f;
      --accent: #ffd600;
      --background: #181a1b;
      --card: #23272f;
      --text: #eee;
      --shadow: 0 2px 10px #0006;
    }
    body {
      background: var(--background);
      color: var(--text);
      font-family: 'Nunito', Arial, sans-serif;
      margin: 0;
      min-height: 100vh;
      transition: background 0.3s, color 0.3s;
    }
    header {
      background: var(--primary);
      color: white;
      padding: 36px 0 28px 0;
      text-align: center;
      border-radius: 0 0 36px 36px;
      box-shadow: var(--shadow);
      position: relative;
    }
    .theme-switch {
      position: absolute;
      top: 16px;
      right: 24px;
      background: var(--accent);
      color: var(--primary);
      border: none;
      font-size: 1.3rem;
      cursor: pointer;
      border-radius: 50%;
      width: 44px;
      height: 44px;
      box-shadow: 0 2px 8px #0003;
      transition: background 0.2s;
    }
    .container {
      max-width: 800px;
      margin: 44px auto;
      padding: 0 18px;
    }
    .card {
      background: var(--card);
      border-radius: 20px;
      box-shadow: var(--shadow);
      margin-bottom: 38px;
      padding: 32px 24px;
      transition: box-shadow 0.2s;
      position: relative;
      overflow: hidden;
      animation: fadeIn 0.6s;
    }
    @keyframes fadeIn { from { opacity: 0; transform: translateY(30px);} to { opacity:1; transform: none;}}
    .card h2 { margin-top: 0;}
    button, input, select {
      font-size: 1rem;
      padding: 10px 16px;
      border-radius: 8px;
      border: none;
      margin: 8px 0;
    }
    button {
      background: var(--primary);
      color: white;
      cursor: pointer;
      transition: background 0.2s;
      font-weight: 700;
    }
    button:hover {
      background: #25c6a3;
    }
    input, select {
      background: #f1f3f5;
      color: var(--text);
      border: 1px solid #ddd;
      width: 70%;
      margin-right: 8px;
    }
    .flex-row {
      display: flex;
      align-items: center;
      gap: 12px;
      flex-wrap: wrap;
    }
    .compass {
      width: 130px;
      height: 130px;
      margin: 24px auto 8px auto;
      display: block;
      background: #eef;
      border-radius: 50%;
      box-shadow: 0 2px 8px #0002;
    }
    .subtitle {
      font-size: 1.1rem;
      color: var(--primary);
      font-weight: 700;
      margin-bottom: 8px;
    }
    .settings-panel {
      display: none;
      margin-top: 16px;
    }
    .settings-panel.active {
      display: block;
    }
    .mosque-list a {
      color: var(--primary);
      text-decoration: underline;
    }
    .quote {
      font-style: italic;
      color: #009688;
      margin-top: 12px;
      font-size: 1.12rem;
      text-align: center;
      border-left: 3px solid var(--accent);
      padding-left: 16px;
    }
    .calendar-table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
    }
    .calendar-table th, .calendar-table td {
      border: 1px solid #ddd;
      padding: 4px 6px;
      text-align: center;
      font-size: 0.96