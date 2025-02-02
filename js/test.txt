// Function to change the background color when the button is clicked
document.getElementById('changeColorButton').addEventListener('click', function() {
  const colors = ['#FF5733', '#33FF57', '#5733FF', '#F0F8FF', '#FF1493'];
  const randomColor = colors[Math.floor(Math.random() * colors.length)];
  document.body.style.backgroundColor = randomColor;
});

// Scroll animation for the main box
window.addEventListener('scroll', function() {
  const mainBox = document.querySelector('.main-box');
  const scrollPosition = window.scrollY;

  // Add a class that triggers a scaling effect when scrolling down
  if (scrollPosition > 100) {
    mainBox.style.transform = 'translate(-50%, -50%) scale(1.1)';
  } else {
    mainBox.style.transform = 'translate(-50%, -50%) scale(1)';
  }
});
