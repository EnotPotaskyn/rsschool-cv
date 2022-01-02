# Evgenii Usovich

![my Photo](1.jpg)

## My Contact Info:
* Location: Minsk, Belarus
* Phone: +375 29 887-92-95
* Email: ackii@bk.ru
* GitHub: [EnotPotaskyn](https://github.com/EnotPotaskyn)https://www.barsu.by/
* Discord: [Евгений(@EnotPotaskyn)](ackii#3886)

## About Me

I am 30 years old. I want to be Front-End Development! I have good interpersonal skills, am an excellent team worker and very willing to learn and develop new skills.

## Skills
* HTML
* CSS/SASS
* JavaScript (Basic)
* Git

## Code example:

```
let makeElement = function (tagName, className, text) {
  
  let element = document.createElement(tagName);
  element.classList.add(className);
  if (text) {
    element.textContent = text;
  }
  return element;
};

let renderCards = function (good) {

let listItem = makeElement('li','good')

let title = makeElement('h2', 'good__description', good.text);
  listItem.appendChild(title);
  
let picture = makeElement('img', 'good__image');
  picture.src = good.imgUrl;
  picture.alt = good.text;
  listItem.appendChild(picture);

let price = makeElement('p','good__price',good.price + '₽/кг')
 listItem.appendChild(price);
 
 let availabilityClass = 'good--available'
 if(!good.inStock){
   availabilityClass = 'good--unavailable'
   }
  listItem.classList.add(availabilityClass);
  
  if(good.isHit){
    listItem.classList.add('good--hit');
    let specialOffer = makeElement('p', 'good__special-offer', good.specialOffer);
    listItem.appendChild(specialOffer);
    }
    
  return listItem
}

let cardList = document.querySelector('.goods');

for (let i = 0; i < cardsData.length; i++) {
  let cardItem = renderCards(cardsData[i]);
  cardList.appendChild(cardItem);
}
```
## Education
* [Baranovichi State University](https://www.barsu.by/)
     - Faculty of Engineering
* [HTML Academy](https://htmlacademy.ru/)

## Language
+ English - A2(B1 in proccess...)
+ Russian - native speaker
