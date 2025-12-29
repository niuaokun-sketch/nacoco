[style.css](https://github.com/user-attachments/files/24369298/style.css)[Uploading index.html…]()
[script.js](https://github.com/user-attachments/files/24369306/script.js)

/* 全局设置：去除默认边距，设置字体 */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f4f4f9; /* 浅灰色背景 */
}

/* 导航栏样式 */
header {
    background-color: #2c3e50; /* 深蓝色背景 */
    color: white;
    padding: 1rem 2rem;
    display: flex;
    justify-content: space-between; /* 左右两端对齐 */
    align-items: center;
}

header .logo {
    font-size: 1.5rem;
    font-weight: bold;
}

header nav ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

header nav a {
    color: white;
    text-decoration: none;
}

/* 首页大图区域样式 */
.hero {
    background-color: white;
    text-align: center;
    padding: 100px 20px;
    border-bottom: 1px solid #ddd;
}

.hero h1 {
    font-size: 2.5rem;
    color: #2c3e50;
    margin-bottom: 10px;
}

.hero button {
    margin-top: 20px;
    padding: 10px 20px;
    background-color: #3498db; /* 蓝色按钮 */
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
}

.hero button:hover {
    background-color: #2980b9; /* 鼠标悬停变深色 */
}

/* 内容区域样式 */
.container {
    max-width: 1000px;
    margin: 40px auto; /* 居中显示 */
    padding: 0 20px;
}

h2 {
    text-align: center;
    margin-bottom: 30px;
    color: #2c3e50;
}

.article-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); /* 自适应网格布局 */
    gap: 20px;
}

/* 文章卡片样式 */
.card {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1); /* 阴影效果 */
}

.card h3 {
    margin-bottom: 10px;
    color: #333;
}

.card a {
    display: inline-block;
    margin-top: 15px;
    color: #3498db;
    text-decoration: none;
    font-weight: bold;
}

/* 底部样式 */
footer {
    text-align: center;
    padding: 20px;
    background-color: #2c3e50;
    color: white;
    margin-top: 50px;
}
// 这是一个简单的 JavaScript 函数
function sayHello() {
    alert("你好！恭喜你，你的第一个网站代码运行成功了！");
}

// 在控制台打印一句话（按F12可以在浏览器控制台看到）
console.log("网站已加载完毕，随时准备为您服务。");
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的个人主页</title>
    <!-- 引入样式表 -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- 1. 顶部导航栏 -->
    <header>
        <div class="logo">我的世界</div>
        <nav>
            <ul>
                <li><a href="#home">首页</a></li>
                <li><a href="#blog">文章</a></li>
                <li><a href="#about">关于我</a></li>
            </ul>
        </nav>
    </header>

    <!-- 2. 主要展示区 (Hero Section) -->
    <section id="home" class="hero">
        <h1>欢迎来到NACO的网站</h1>
        <p>这里是我记录生活、分享知识的地方。</p>
        <button onclick="sayHello()">点击我打个招呼</button>
    </section>

    <!-- 3. 内容文章区 -->
    <section id="blog" class="container">
        <h2>最新文章</h2>
        <div class="article-grid">
            <!-- 文章卡片 1 -->
            <article class="card">
                <h3>第一篇博客</h3>
                <p>这是我的第一篇文章。虽然现在内容还很少，但我可以通过修改代码随时增加新的内容...</p>
                <a href="#">阅读更多</a>
            </article>

            <!-- 文章卡片 2 -->
            <article class="card">
                <h3>学习搭建网站</h3>
                <p>我决定放弃现成的模板，从零开始编写代码。这样我才能真正理解网站是如何运行的。</p>
                <a href="#">阅读更多</a>
            </article>
            
             <!-- 文章卡片 3 (预留位置) -->
            <article class="card">
                <h3>未来内容的占位符</h3>
                <p>我可以随时复制这段代码，粘贴在后面，就能生成第三篇文章。</p>
                <a href="#">阅读更多</a>
            </article>
        </div>
    </section>

    <!-- 4. 底部版权区 -->
    <footer id="about">
        <p>&copy; 2025 我的个人网站. 保留所有权利。</p>
    </footer>

    <!-- 引入脚本 -->
    <script src="script.js"></script>
</body>
</html>
