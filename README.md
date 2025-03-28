# Assignment.github.io

HTML CODE🔽

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hero Section</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <section class="hero">
    <div class="hero-content">
      <h1>Welcome to Pha5e</h1>
      <p>Your journey begins here!...</p>
      <button class="cta">Get Started</button>
    </div>
  </section>
  <script src="script.js"></script>
</body>
</html>


CSS CODE🔽

body {
    margin: 0;
    font-family: cursive Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    overflow: hidden;
  }

  button {
    background-color: #e84141b9;
    color: #6c5ce7;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    transition: transform 0.3s ease, background-color 0.3s ease;
  }
  
  button:hover {
    background-color: #5ce778;
    color: #ffffff;
    transform: scale(1.1); /* Slightly enlarges the button */
  }
  
  
  .hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(45deg, #ff7eb3, #6c5ce7);
    color: #ffffff;
    text-align: center;
  }
  
  .hero-content h1 {
    font-size: 4rem;
    animation: fadeIn 1.5s ease-in-out;
  }
  
  .hero-content p {
    font-size: 1.5rem;
    animation: slideIn 2s ease-in-out;
  }
  
  .cta {
    margin-top: 20px;
    padding: 10px 20px;
    font-size: 1rem;
    color: #6c5ce7;
    background-color: #ffffff;
    border: none;
    cursor: pointer;
    transition: transform 0.3s ease;
  }
  
  .cta:hover {
    transform: scale(1.1);
  }
  
  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }
  
  @keyframes slideIn {
    from { transform: translateY(50px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
  }


  JAVASCRIPT CODE🔽

  document.addEventListener('mousemove', (event) => {
    const x = (event.clientX / window.innerWidth) * 100;
    const y = (event.clientY / window.innerHeight) * 100;
  
    document.querySelector('.hero').style.backgroundPosition = `${x}% ${y}%`;
  });
