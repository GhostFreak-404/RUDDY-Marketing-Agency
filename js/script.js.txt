const anchorElement = document.getElementsByClassName('scrolltotop')[0];
const imageElement = document.getElementsByClassName('scrolltotop')[0].firstElementChild;


function view() {
    if (anchorElement.getBoundingClientRect().top <= 400) {
      imageElement.classList.add("position");
    } else {
      imageElement.classList.remove("position");
    }
}

window.addEventListener("scroll", view)
