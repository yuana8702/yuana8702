### AUTOFILL PROFILES ###,,,,,,
Profile ID,Name,Site,Hotkey,,,
### AUTOFILL RULES ###,,,,,,
Rule ID,Type,Name,Value,Site,Mode,Profile
r109,4,"","function generateRandomUSZipCode() {
  const zipCodeRanges = [
    { min: 10000, max: 14999 }, // New York
    { min: 20000, max: 24999 }, // Washington, D.C.
    { min: 30000, max: 34999 }, // Georgia
    { min: 35000, max: 39999 }, // Alabama
    { min: 40000, max: 49999 }, // Kentucky
  ];
  const randomRange = zipCodeRanges[Math.floor(Math.random() * zipCodeRanges.length)];
  const randomZipCode = Math.floor(Math.random() * (randomRange.max - randomRange.min + 1)) + randomRange.min;

  return randomZipCode.toString().padStart(5, '0'); 
}
let inputBox = document.getElementById('fldID_zip');
inputBox.value = generateRandomUSZipCode();
","adultfriendfinder.com/",1,
r111,1,"^password$","AY666888","adultfriendfinder.com/",1,
r112,3,"^looking_for_person_new$","1010","adultfriendfinder.com/",1,
r114,2,"^REG_sex$","""2""","adultfriendfinder.com/",1,
r115,2,"^bday_month$","""6""","adultfriendfinder.com/",1,
r116,2,"^bday_day$","""04""","adultfriendfinder.com/",1,
r117,2,"^bday_year$","""1988""","adultfriendfinder.com/",1,
r118,4,"","
const targetElement = document.querySelector(""#fldID_butAction_1"");


const clickEvent = new MouseEvent(""click"", {
  view: window,
  bubbles: true,
  cancelable: true,
  clientX: 0, 
  clientY: 0  
});


targetElement.dispatchEvent(clickEvent);
","adultfriendfinder.com/",1,
r121,4,"","
function checkElement() {
    const errorText = ""This zip/postal code is not valid."";
    const elementsWithText = document.querySelectorAll(""*"");
    for (const element of elementsWithText) {
        if (element.textContent === errorText) {
            
            clearInterval(intervalId);
            location.reload();
            return;
        }
    }
    console.log(""Error text not found. Stopping interval."");
    clearInterval(intervalId); 
}


const intervalId = setInterval(checkElement, 3000);
","",1,
r122,4,"","
const names = ['Abigail',
'Agatha',
'Adelaide',
'Adelina',
'Alethea',
'Aggie',
'Agnes',
'Aileen',
'Alexandra',
'Alexis',
'Alice',
'Alison',
'Amanda',
'Angela',
'Angie',
'Anita',
'Anne',
'Anna',
'Annabel',
'Annie',
'Annette',
'Anthea',
'Antonia',
'Audrey',
'Allson',
'Alma',
'Althea',
'Angelica',
'Aspasia',
'Aurelian',
'Avis',
'Beata',
'Belle',
'Babs',
'Barbara',
'Beatrice',
'Becky',
'Belinda',
'Bernadette',
'Beryl',
'Betty',
'Bid',
'Brenda',
'Bridget',
'Brittany',
'Bertha',
'Bonny',
'Camilla',
'Candice',
'Carla',
'Carol',
'Caroline',
'Carrie',
'Catherine',
'Cathy',
'Cecilia',
'Cecily',
'Celia',
'Charlene',
'Charlotte',
'Cherry',
'Cheryl',
'Chloe',
'Chris',
'Chrissie',
'Christina',
'Christine',
'Cindy',
'Clare',
'Claudia',
'Cleo',
'Connie',
'Constance',
'Crystal',
'Candida',
'Carmen',
'Celestine',
'Charissa',
'Colleen',
'Cora',
'Corinna',
'Cynthia',
'Dulcie',
'Dottie',
'Daisy',
'Daphne',
'Dawn',
'Debby',
'Deborah',
'Deirdre',
'Delia',
'Della',
'Denise',
'Diana',
'Diane',
'Dolly',
'Donna',
'Dora',
'Doreen',
'Doris',
'Dorothy',
'Elva',
'Edith',
'Edna',
'Eileen',
'Elaine',
'Eleanor',
'Eleanora',
'Eliza',
'Elizabeth',
'Ella',
'Ellen',
'Ellie',
'Elsa',
'Elsie',
'Elspeth',
'Emily',
'Emma',
'Erica',
'Ethel',
'Eunice',
'Evelyn',
'Eugenia',
'Eulalia',
'Evadne',
'Evangeline',
'Faustina',
'Felicity',
'Fidelia',
'Fiona',
'Flora',
'Florence',
'Felicia',
'Flavia',
'Frieda',
'Freda',
'Florrie',
'Fran',
'Frances',
'Frankie',
'Gene',
'Georgia',
'Georgie',
'Georgina',
'Geraldine',
'Germaine',
'Gertie',
'Gertrude',
'Gill',
'Gillian',
'Ginny',
'Gladys',
'Glenda',
'Gloria',
'Grace',
'Gracie',
'Ashley',
'Gwen',
'Gwendoline',
'Hannah',
'Harriet',
'Hazel',
'Heather',
'Helen',
'Henrietta',
'Hilary',
'Hilda',
'Hedda',
'Hedwig',
'Helga',
'Hortensia',
'Isabella',
'Ingrid',
'Irene',
'Iris',
'Isabel',
'Jemima',
'Juliana',
'Jan',
'Jane',
'Janet',
'Janey',
'Janice',
'Jackie',
'Jacqueline',
'Jean',
'Jeanie',
'Jennifer',
'Jenny',
'Jess',
'Jessica',
'Jessie',
'Jill',
'Joan',
'Joanna',
'Joanne',
'Jocelyn',
'Josephine',
'Josie',
'Jode',
'Joyce',
'Judith',
'Judy',
'Julia',
'Julie',
'Juliet',
'June',
'Karen',
'Kathleen',
'Kate',
'Kathy',
'Katie',
'Kelly',
'Kimberly',
'Kirsten',
'Kitty',
'Katharine',
'Leila',
'Laura',
'Lauretta',
'Lesley',
'Libby',
'Lilian',
'Lily',
'Linda',
'Lindsay',
'Lisa',
'Livia',
'Lois',
'Lori',
'Lorna',
'Louisa',
'Louise',
'Lucia',
'Lucinda',
'Lucy',
'Lydia',
'Lynn',
'Leslie',
'Lucile',
'LuLu',
'Mabel',
'Madeleine',
'Madge',
'Maggie',
'Maisie',
'Mandy',
'Marcia',
'Marcie',
'Margaret',
'Margery',
'Maria',
'Marian',
'Mary',
'Marilyn',
'Marlene',
'Martha',
'Melanie',
'Mercedes',
'Mignon',
'Mimi',
'Martha',
'Martina',
'Mary',
'Maud',
'Maureen',
'Mavis',
'Melanie',
'Melinda',
'Melissa',
'Michelle',];

const randomIndex = Math.floor(Math.random() * names.length);

const randomName = names[randomIndex];

document.getElementById('fldID_REG_handle').value = randomName;
","",1,
r125,0,"^title$","If you're interested in me, let's explore fun and creativity together!","adultfriendfinder.com/",1,
r126,4,"","
function generateRandomLetters(length) {
  var result = '';
  var characters = 'abcdefghijklmnopqrstuvwxyz';
  var charactersLength = characters.length;
  for (var i = 0; i < length; i++) {
    result += characters.charAt(Math.floor(Math.random() * charactersLength));
  }
  return result;
}


var emailInput = document.getElementById(""fldID_email"");


var rememberedEmail = localStorage.getItem('randomEmail');
if (!rememberedEmail) {
    rememberedEmail = generateRandomLetters(10) + '@snapmail.cc';
    localStorage.setItem('randomEmail', rememberedEmail);
}


emailInput.value = rememberedEmail;


var floatingDiv1 = document.createElement('div');
floatingDiv1.style.position = 'fixed';
floatingDiv1.style.top = '50%';
floatingDiv1.style.left = '50%';
floatingDiv1.style.transform = 'translate(-50%, -50%)';
floatingDiv1.style.background = '#ffffff';
floatingDiv1.style.padding = '10px';
floatingDiv1.style.border = '1px solid #000000';
floatingDiv1.style.boxShadow = '0 0 10px rgba(0, 0, 0, 0.5)';
floatingDiv1.style.zIndex = '9999';
document.body.appendChild(floatingDiv1);


floatingDiv1.textContent = rememberedEmail;


var jumpUrl = ""https://www.snapmail.cc/emailList/"" + rememberedEmail + ""?count=2"";

window.open(jumpUrl, '_blank');


setTimeout(function() {
  floatingDiv1.style.display = 'none';
}, 15000);

// 创建悬浮元素2：用于显示“阿远制作”
var floatingDiv2 = document.createElement('div');
floatingDiv2.style.position = 'fixed';
floatingDiv2.style.top = '10%';
floatingDiv2.style.left = '50%';
floatingDiv2.style.transform = 'translate(-50%, -50%)';
floatingDiv2.style.background = '#ffffff';
floatingDiv2.style.padding = '10px';
floatingDiv2.style.border = '1px solid #000000';
floatingDiv2.style.boxShadow = '0 0 10px rgba(0, 0, 0, 0.5)';
floatingDiv2.style.zIndex = '9999';
document.body.appendChild(floatingDiv2);

floatingDiv2.textContent = '阿远脚本';
","",1,
r128,4,"","
function clickElementByXPath(xpath) {
    var element = document.evaluate(xpath, document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue;
    if (element) {
        element.click(); 
    }
}


var clickCount = 0;


setTimeout(function() {

    function loopClick() {
        clickElementByXPath('/html/body/div[4]/div[1]/div/div[1]/div/div/form/div[3]/div[2]/div[3]/a[1]');
        clickCount++;


        if (clickCount < 5) {
            setTimeout(loopClick, 3000); // 3秒后再次点击
        }
    }


    loopClick();
}, 3000); 
","adultfriendfinder.com/",1,
r127,4,"","
var button = document.getElementById('fldID_butAction_2');


function clickButton() {
    button.click(); 
}


var clickCount = 0;


setTimeout(function() {

    clickButton();
    clickCount++;


    var intervalId = setInterval(function() {
        if (clickCount < 5) {

            clickButton();
            clickCount++;
        } else {

            clearInterval(intervalId);
        }
    }, 6000); 
}, 3000); 
","adultfriendfinder.com/",1,
### AUTOFILL OPTIONS ###,,,,,,
advanced,"[]",,,,,
exceptions,"[]",,,,,
textclips,"[]",,,,,
variables,"[]",,,,,
activecat,1,,,,,
attributesoff,0,,,,,
autoimport,0,,,,,
backup,0,30,,,,
badge,1,,,,,
closeinfobar,1,1,,,,
debug,0,,,,,
delay,0,0.5,,,,
filtercats,0,,,,,
fluid,1,,,,,
hidebackup,0,,,,,
manual,0,,,,,
mask,1,,,,,
menu,1,,,,,
overwrite,1,,,,,
sitefilters,1,,,,,
skiphidden,0,,,,,
sound,0,,,,,
vars,1,,,,,
voice,0,1,,,,
