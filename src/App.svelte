
<div id="loading-screen">
  <img src="/mem2.PNG" alt="e" class="loading-image" width="300px"/>
  <div class="wave">
    <span class="dot"></span>
    <span class="dot"></span>
    <span class="dot"></span>
    <span class="dot"></span>
    <span class="dot"></span>
  </div>
  <p id="loading-text" class="loading-text">welcome to aequor finance ...</p>
  <div class="progress-bar">
    <div class="progress-fill"></div>
  </div>
</div>

<main>
  <nav class="menu-bar">
   
  </nav>
<Router>
  <nav class="menu-bar">
    <Link to="/docs" style={{ color: 'white'}} class="menu-link">Docs</Link>
    <Link to="/stake" style={{ color: 'white' }} class="menu-link">Stake</Link>
    <Link to="/social" style={{ color: 'white' }} class="menu-link">Social</Link>
    <Link to="/bank" style={{ color: 'white' }} class="menu-link">Presale</Link>
  </nav>

  <Route path="/docs" component={Docs} />
  <Route path="/bank" component={Bank} />
</Router>



  <header>
    <h1 >Aequor 💧 Finance</h1>

  </header>

  <img src="/mrm.png" alt="fx logo" class="glow-effect" width="300px" />

  

  <section class="bubble-container">
    <div class="bubble" style="--i: 0; --size: 40px; --left: 10%;"></div>
    <div class="bubble" style="--i: 1; --size: 60px; --left: 20%;"></div>
  </section>

</main>

<main id="main2">
  <nav class="menu-bar">
    <a href="#docs">Docs</a>
    <a href="#stake">Stake</a>
    <a href="#social">Social</a>
    <a href="#bank">Bank</a>
  </nav>

  <header>
    <h1>Aequor 💧 Finance</h1>
  </header>

  <img src="/mrm.png" alt="fx2 logo" class="glow-effect" width="300px" />

  <section class="bubble-container">
    <div class="bubble" style="--i: 0; --size: 40px; --left: 10%;"></div>
    <div class="bubble" style="--i: 1; --size: 60px; --left: 20%;"></div>
  </section>
</main>


<style>
  @import url('https://fonts.googleapis.com/css2?family=Splash:wght@400&display=swap');
  @import url('https://fonts.googleapis.com/css?family=Press+Start+2P');
  @import url('https://fonts.googleapis.com/css?family=Caesar+Dressing&display=swap');

  body {
  margin: 0;
  padding: 0;
  overflow: hidden;
  font-family: 'Montserrat', sans-serif;
  background: url('/oceandeep.PNG') no-repeat center center fixed;
  background-size: cover;
  color: #ffffff;
}


  #loading-screen {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url('/oceandeep.PNG') no-repeat center center fixed;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    z-index: 1000;
    transition: opacity 1s ease, visibility 1s ease;
  }

  .menu-bar:hover {
    background-color: rgb(5, 67, 79); /* Background color on hover */
    border: 8px solid #075c1c;
  }
  #loading-screen .spinner {
    border: 8px solid rgba(255, 255, 255, 0.2);
    border-top: 8px solid #fff;
    border-radius: 50%;
    width: 80px;
    height: 80px;
    animation: spin 2s linear infinite;
  }

  .menu-link {
    color: white;
    text-decoration: none;
  }

  .menu-link:hover {
    color: #00c853; /* Example hover color */
    text-decoration: underline; /* Example hover effect */
  }


  .progress-bar {
  width: 80%;
  height: 20px;
  background-color: rgba(255, 255, 255, 0.3);
  border-radius: 10px;
  margin-top: 20px;
  overflow: hidden;
}

.progress-fill {
  width: 0;
  height: 100%;
  background: linear-gradient(to right, #00c853, #006994);
  border-radius: 10px;
  transition: width 0.5s ease;
}

  #loading-screen .loading-text {
    margin-top: 1rem;
    font-family: 'Caesar Dressing', cursive;
    font-size: 1.5rem;
    color: #00c853;
    text-shadow: 0 0 10px rgba(0, 255, 255, 0.6);
  }

  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .link {
  color: #d83939;
  text-decoration: none ;
/* Optional: removes underline */
}



.link:hover {
  color: #ffffff; /* Keeps the text white on hover */
}
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    text-align: center;
    perspective: 1000px;
    opacity: 0;
    visibility: hidden;
    transition: opacity 1s ease, visibility 1s ease;
  }

  #loading-screen.hidden + main {
    opacity: 1;
    visibility: visible;
  }
  .menu-bar {
  display: flex;
  justify-content: center;
  gap: 2rem;
  padding: 1.3rem;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 10;
  margin-left: -27px;
  color: white;
  
  border: 4px solid #ffffff; /* Adjust color and thickness as needed */
  border-radius: 15px; /* Adjust border-radius as needed */
  background-color: rgba(0, 0, 0, 0.3); /* Optional: Add background color */
}



.menu-bar a {
  font-family: 'Caesar Dressing', cursive;
  font-size: 1rem;
  color: #ffffff; /* Ensure the text is white */
  text-decoration: none;
  padding: 0.5rem 1rem;
  transition: background-color 0.3s ease, transform 0.3s ease, filter 0.3s ease;
  border-radius: 5px;
}

.menu-bar a:hover {
  background-color: #006620; /* Deep blue background color on hover */
  transform: translateY(-10px);
  filter: drop-shadow(0 0 10px rgba(0, 255, 255, 0.8));
  border-radius: 30px;
}

  header h1 {
    font-size: 1.8rem;
    text-transform: uppercase;
    font-family: 'Caesar Dressing', cursive;
    letter-spacing: 0.1em;
     color: #00c853;
    text-shadow: 0 0 20px rgba(0, 255, 255, 0.8);
    animation: pulse 2s infinite;
  }

  header p {
    font-family: 'Caesar Dressing', cursive;
    font-size: .9rem;
    margin-top: 0.5rem;
    text-shadow: 0 0 10px rgba(0, 255, 255, 0.6);
  }

  @keyframes pulse {
    0%, 100% {
      transform: scale(1);
      opacity: 1;
    }
    50% {
      transform: scale(1.05);
      opacity: 0.8;
    }
  }

  .bubble-container {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 100%;
    overflow: hidden;
    pointer-events: none;
    z-index: -1;
  }

  .bubble {
    position: absolute;
    bottom: -100px;
    width: var(--size);
    height: var(--size);
    background: rgba(255, 255, 255, 0.3);
    border-radius: 50%;
    left: var(--left);
    animation: rise 10s infinite ease-in;
    animation-delay: calc(-10s * var(--i));
    box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.5);
    transform: scale(1) translateZ(0);
  }

  @keyframes rise {
    0% {
      bottom: -100px;
      transform: scale(1) translateZ(0);
    }
    50% {
      transform: scale(1.2) translateZ(50px);
    }
    100% {
      bottom: 100vh;
      transform: scale(0.8) translateZ(0);
    }
  }

  .glow-effect {
    animation: glow 2s infinite alternate, float 5s infinite ease-in-out;
    filter: drop-shadow(0 0 20px rgba(0, 255, 255, 0.8));
  }

  @keyframes glow {
     from { filter: drop-shadow(0 0 20px rgba(0, 255, 255, 0.8)); }
     to { filter: drop-shadow(0 0 30px rgba(0, 255, 255, 1)); }
  }

  @keyframes float {
     0%, 100% { transform: translateY(0); }
     50% { transform: translateY(-20px); }
  }

  .wave {
    display: flex;
    gap: 8px;
  }

  .dot {
    width: 15px;
    height: 15px;
    background: linear-gradient(to right, #ffffff, #00c853); 
    border-radius: 50%;
    animation: wave 1.2s linear infinite;
  }

  .dot:nth-child(1) { animation-delay: 0s; }
  .dot:nth-child(2) { animation-delay: 0.2s; }
  .dot:nth-child(3) { animation-delay: 0.4s; }
  .dot:nth-child(4) { animation-delay: 0.6s; }
  .dot:nth-child(5) { animation-delay: 0.8s; }

  @keyframes wave {
    0%, 60%, 100% {
      transform: translateY(0);
    }
    30% {
      transform: translateY(-15px);
    }
  }

  main, #main2 {
  transition: opacity 0.5s ease, visibility 0.5s ease;
}


main.hidden {
  opacity: 0;
  visibility: hidden;
}

#main2.visible {
  display: block;
  opacity: 1;
  visibility: visible;
}

.hidden {
  opacity: 0;
  visibility: hidden;
}

.visible {
  opacity: 1;
  visibility: visible;
}

#main2 {
  display: none; /* Initially hidden */
  opacity: 0;
  visibility: hidden;
}

/* When the .visible class is added, display main2 */


  
</style>

<script>
window.addEventListener('load', () => {
  const loadingScreen = document.getElementById('loading-screen');
  const progressFill = document.querySelector('.progress-fill');
  const loadingText = document.getElementById('loading-text');
  const mainContent = document.querySelector('main');
  const main2Content = document.getElementById('main2');

  if (!loadingScreen || !progressFill || !loadingText || !mainContent || !main2Content) {
    console.error('One or more elements not found on the page.');
    return;
  }

  let progress = 0;
  const progressSteps = [
    { percentage: 15, text: "Diving into ocean depths" },
    { percentage: 30, text: "Scooping mermaids" },
    { percentage: 45, text: "Swimming" },
    { percentage: 60, text: "Diving" },
    { percentage: 75, text: "Almost at ocean depth" },
    { percentage: 100, text: "Meeting Poseidon" },
  ];

  const progressInterval = setInterval(() => {
    progress += 1;
    progressFill.style.width = `${progress}%`;

    const step = progressSteps.find(step => step.percentage === progress);
    if (step) {
      loadingText.textContent = step.text;
    }

    if (progress === 100) {
      clearInterval(progressInterval);
      // Delay for a moment before hiding the loading screen
      setTimeout(() => {
        loadingScreen.style.opacity = '0';
        loadingScreen.style.visibility = 'hidden';
        mainContent.style.opacity = '1';
        mainContent.style.visibility = 'visible';
        main2Content.style.opacity = '0';
        main2Content.style.visibility = 'hidden';
      }, 500); // Adjust delay if needed
    }
  }, 50); // Adjust the speed of progress fill as needed
});

let lastScrollTop = 0;

window.addEventListener('scroll', () => {
  const main = document.querySelector('main');
  const main2 = document.getElementById('main2');
  const currentScroll = window.pageYOffset || document.documentElement.scrollTop;

  if (main && main2) {
    if (currentScroll > lastScrollTop) {
      // Scrolling down
      main.style.opacity = '0';
      main.style.visibility = 'hidden';
      main2.style.opacity = '1';
      main2.style.visibility = 'visible';
    } else {
      // Scrolling up
      main.style.opacity = '1';
      main.style.visibility = 'visible';
      main2.style.opacity = '0';
      main2.style.visibility = 'hidden';
    }
  } else {
    console.error('Main or main2 element not found.');
  }

  lastScrollTop = currentScroll <= 0 ? 0 : currentScroll; // For Mobile or negative scrolling
});

import { Router, Route, Link } from "svelte-navigator";
import Docs from '../src/docs.svelte';
import Bank from '../src/bank.svelte';

</script>


