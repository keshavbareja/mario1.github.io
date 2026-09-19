<!DOCTYPE html>
<html>
<head>
  <title>Mini Mario Engine</title>
  <style>
    body { 
      background: #222; 
      display: flex; 
      justify-content: center; 
      align-items: center; 
      height: 100vh; 
      margin: 0; 
    }
    canvas { 
      background: #87CEEB; /* Sky blue */
      border: 4px solid #fff; 
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }
  </style>
</head>
<body>

<canvas id="gameCanvas" width="500" height="350"></canvas>

<script>
  const canvas = document.getElementById("gameCanvas");
  const ctx = canvas.getContext("2d");

  // 1. Define the Player Object
  const mario = {
    x: 50,
    y: 200,
    width: 20,
    height: 30,
    dx: 0,       // Horizontal velocity
    dy: 0,       // Vertical velocity
    speed: 4,
    jumpPower: -10,
    grounded: false
  };

  const gravity = 0.5;
  const keys = { right: false, left: false, up: false };

  // 2. Track Keyboard Input
  window.addEventListener("keydown", (e) => {
    if (e.code === "ArrowRight") keys.right = true;
    if (e.code === "ArrowLeft") keys.left = true;
    if (e.code === "ArrowUp" || e.code === "Space") keys.up = true;
  });

  window.addEventListener("keyup", (e) => {
    if (e.code === "ArrowRight") keys.right = false;
    if (e.code === "ArrowLeft") keys.left = false;
    if (e.code === "ArrowUp" || e.code === "Space") keys.up = false;
  });

  // 3. Update Game Logic (Physics & Math)
  function update() {
    // Left/Right Movement
    if (keys.right) mario.dx = mario.speed;
    else if (keys.left) mario.dx = -mario.speed;
    else mario.dx = 0;

    // Jumping (Only if touching the ground)
    if (keys.up && mario.grounded) {
      mario.dy = mario.jumpPower;
      mario.grounded = false;
    }

    // Apply Gravity pulling downwards
    mario.dy += gravity;
    
    // Apply velocity to current position
    mario.x += mario.dx;
    mario.y += mario.dy;

    // 4. Ground Collision (The floor is at y = 300)
    if (mario.y + mario.height >= 300) {
      mario.y = 300 - mario.height; // Snap to the floor
      mario.dy = 0;                 // Stop falling
      mario.grounded = true;        // Allow jumping again
    }

    // Screen Boundary Collision (Keep player on screen)
    if (mario.x < 0) mario.x = 0;
    if (mario.x + mario.width > canvas.width) mario.x = canvas.width - mario.width;
  }

  // 5. Render the Graphics
  function draw() {
    // Clear the previous frame
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    // Draw the Ground
    ctx.fillStyle = "#8B4513"; // Brown dirt
    ctx.fillRect(0, 300, canvas.width, 50);
    ctx.fillStyle = "#228B22"; // Green grass top
    ctx.fillRect(0, 300, canvas.width, 10);

    // Draw Mario (represented by a red rectangle)
    ctx.fillStyle = "#FF0000"; 
    ctx.fillRect(mario.x, mario.y, mario.width, mario.height);
  }

  // 6. The Game Loop
  function loop() {
    update();
    draw();
    requestAnimationFrame(loop); // Runs 60 times per second
  }

  // Start the engine
  loop();
</script>

</body>
</html>
