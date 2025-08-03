body {
    font-family: 'Arial', sans-serif;
    background: #f0f2f5;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
}

.container {
    width: 100%;
    max-width: 540px;
    background: #fff;
    margin: 20px;
    padding: 40px 30px;
    border-radius: 10px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.todo-app h1 {
    color: #333;
    margin-bottom: 20px;
}

.row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #edeef0;
    border-radius: 30px;
    padding-left: 20px;
    margin-bottom: 25px;
}

input {
    flex: 1;
    border: none;
    outline: none;
    background: transparent;
    padding: 10px;
    font-size: 16px;
}

button {
    border: none;
    outline: none;
    padding: 16px 30px;
    background: #4CAF50; /* Warna hijau */
    color: #fff;
    font-size: 16px;
    cursor: pointer;
    border-radius: 30px;
}

button:hover {
    background: #45a049;
}

ul {
    padding: 0;
}

ul li {
    list-style: none;
    font-size: 17px;
    padding: 12px 8px 12px 50px;
    user-select: none;
    cursor: pointer;
    position: relative;
}

ul li::before {
    content: '';
    position: absolute;
    height: 24px;
    width: 24px;
    border-radius: 50%;
    background-image: url('data:image/svg+xml,%3Csvg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="%23555" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"%3E%3Ccircle cx="12" cy="12" r="10"%3E%3C/circle%3E%3C/svg%3E');
    background-size: cover;
    left: 8px;
    top: 10px;
}

ul li.checked {
    color: #888;
    text-decoration: line-through;
}

ul li.checked::before {
    background-image: url('data:image/svg+xml,%3Csvg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="background-color:%234CAF50; border-radius: 50%;"%3E%3Cpath d="M22 11.08V12a10 10 0 1 1-5.93-9.14"%3E%3C/path%3E%3Cpolyline points="22 4 12 14.01 9 11.01"%3E%3C/polyline%3E%3C/svg%3E');
}

ul li span {
    position: absolute;
    right: 0;
    top: 5px;
    width: 40px;
    height: 40px;
    font-size: 22px;
    color: #555;
    line-height: 40px;
    text-align: center;
    border-radius: 50%;
}

ul li span:hover {
    background: #edeef0;
}
