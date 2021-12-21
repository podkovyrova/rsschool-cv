# **Katerina Podkovyrova**

## **Contact Info**
+ Telegram: *@wakemeuptomorrow*
+ Discord: *podkovyrova*
+ E-mail: *podkovyrova.es@mail.ru*
+ GitHub: *[podkovyrova](https://github.com/podkovyrova)*

## **About**
Today I am 21 years old and after gaining work experience in the studied specialty at the university, I decided to change my profession.
Since childhood, I have been interested in technologies and programs: when I accidentally opened DevTools in a browser, I got scared, but at the same time I became interested in how it all works.
Now I understand how it works and I want to create my own web pages and applications.
4 months ago I learned about such a profession as Frontend-developer and began to actively learn HTML and CSS on my own. Also, I have created several landing pages.
My goal for the next six months is to finish RS School and get my first job as a Junior Frontend Developer.

## **Skills**
+ HTML5, CSS3 (SASS/SCSS)
+ JavaScript: fundamentals & DOM
+ Git/GitHub
+ VSCode
+ Figma
+ Agile, Scrum, Kanban
+ BEM 
## Code 
Slider code I created
```
const upBtn = document.querySelector('.up-button');
const downBtn = document.querySelector('.down-button'); 
const sidebar = document.querySelector('.sidebar');
const mainSlide = document.querySelector('.main-slide');
const container = document.querySelector('.container');

const slidesCount = mainSlide.querySelectorAll('div').length; 

let activeSlideIndex = 0; 

sidebar.style.top = `-${(slidesCount-1) * 100}vh`;

upBtn.addEventListener('click', () => {
    changeSlide('up');
})
downBtn.addEventListener('click', () => {
    changeSlide('down');
})

document.addEventListener('keydown', event => {  
    if (event.key === 'ArrowUp') {
        changeSlide('up');
    } else if (event.key === 'ArrowDown') {
        changeSlide('down');
    }
})

function changeSlide(direction) {
    if (direction === 'up') {
        activeSlideIndex++;
        if(activeSlideIndex === slidesCount) {
            activeSlideIndex = 0;
        }
    } else if (direction === 'down') {
        activeSlideIndex--;
        if(activeSlideIndex < 0) {
            activeSlideIndex = slidesCount - 1;
        }
    }

    const heightOfWindow = container.clientHeight;

    mainSlide.style.transform = `translateY(-${activeSlideIndex * heightOfWindow}px)`; 
    sidebar.style.transform = `translateY(${activeSlideIndex * heightOfWindow}px)`;
}
```

## **Education**
1. Financial University under the Goverment of the Russian Federation - *bachelor-degree*
2. KPMG Foundation for Graduates
3. Code Basics: [HTML]("https://ru.code-basics.com/languages/html"), [CSS]("https://ru.code-basics.com/languages/css")
4. 5 day JS-intensive by Vladilen Minin
5. RS School Course «JavaScript/Front-end. Stage 0» (in progress)

## **Languages**
**Russian** - native speaker

**English** - A2
