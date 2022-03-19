# **Katerina Podkovyrova**

## **Contact Info**
+ Telegram: [wakemeuptomorrow](https://t.me/wakemeuptomorrow)
+ Discord: podkovyrova(#0788)
+ E-mail: podkovyrova.es@mail.ru
+ GitHub: [podkovyrova](https://github.com/podkovyrova)

## **About**
I'm living in Moscow and finishing education in Economics science. One year ago I decided to start learning in Information Technologies. Honestly, I find out it more complicated and amazing than Economics. So, this is the main reason I'm here. 
In summer 2021 I had mastered the base of HTML, CSS and JavaScript.
Since 2022 I have been working as QA engineer for MobileTeleSystems Digital. Testing is fun but I want to become a developer.
My goal for the next six months is to finish RS School and get my first job as a frontend developer (:

## **Skills**
+ HTML5, CSS3 (SASS/SCSS)
+ JavaScript: fundamentals & DOM
+ Git/GitHub
+ VSCode
+ Figma
+ Agile, Scrum, Kanban
+ BEM 
+ QA Tools: Postman, Charles Proxy, Graylog and so so so on 
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
