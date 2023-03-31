<script>
    export let imageSrc = '';
  </script>
  
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap');
  
    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0.5rem 1rem;
      background-color: #f5f5f5;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      font-family: 'Roboto', sans-serif;
    }
  
    .header-logo {
      display: flex;
      align-items: center;
    }
  
    .header-logo img {
      height: 50px;
      margin-right: 0.5rem;
      border-radius: 50%;
    }
  
    .header-nav {
      display: flex;
      align-items: center;
    }
  
    .header-nav a {
      text-decoration: none;
      color: #333;
      margin-right: 1rem;
      padding: 4px 8px;
      font-size: 18px;
      border-radius: 4px;
      transition: background-color 0.3s, color 0.3s;
    }
  
    .header-nav a:hover {
      color: #fff;
      background-color: #666;
    }
  </style>
  
  <div class="header">
    <div class="header-logo">
      {#if imageSrc}
        <img src="{imageSrc}" alt="Logo" />
      {/if}
      <h1>Num Tung Social</h1>
    </div>
    <nav class="header-nav">
      <a href="/">Home</a>
      <a href="/about">About</a>
      <a href="/menu">Menu</a>
    </nav>
  </div>
  