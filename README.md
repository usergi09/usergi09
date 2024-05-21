<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>To-Do List with Speaking Bunny</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f0f8ff;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            background: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
        }
        h1 {
            color: #444;
            margin-top: 20px;
        }
        .todo-container {
            width: 80%;
            max-width: 600px;
            margin-top: 20px;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .todo-input {
            width: calc(100% - 40px);
            padding: 10px;
            margin-bottom: 10px;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        .todo-list {
            list-style-type: none;
            padding: 0;
        }
        .todo-item {
            padding: 10px;
            margin-bottom: 5px;
            border-bottom: 1px solid #eee;
            display: flex;
            justify-content: space-between;
        }
        .todo-item:last-child {
            border-bottom: none;
        }
        .todo-item input {
            margin-right: 10px;
        }
        .todo-item button {
            background: none;
            border: none;
            color: #888;
            cursor: pointer;
            font-size: 16px;
        }
        .todo-item button:hover {
            color: #f00;
        }
        .bunny-container {
            position: relative;
            margin-top: 20px;
        }
        .bunny {
            width: 100px;
            height: auto;
        }
        .speech-bubble {
            position: absolute;
            top: -80px;
            left: 110px;
            width: 150px;
            background: #fff;
            border: 2px solid #333;
            border-radius: 10px;
            padding: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            font-size: 14px;
            text-align: center;
        }
       
