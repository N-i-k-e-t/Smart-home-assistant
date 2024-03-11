const buttons = document.querySelectorAll('button'); 

buttons.forEach(btn => {
  btn.addEventListener('click', function(event) {
    event.preventDefault(); // Prevent abrupt jump
    const sectionId = this.getAttribute('href');
    document.querySelector(sectionId).scrollIntoView({
      behavior: 'smooth'
    });
  });
});
