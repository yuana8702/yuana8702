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
r118,4,"","// 查找目标元素
const targetElement = document.querySelector(""#fldID_butAction_1"");

// 创建鼠标点击事件
const clickEvent = new MouseEvent(""click"", {
  view: window,
  bubbles: true,
  cancelable: true,
  clientX: 0, // 你想要点击的位置的 x 坐标
  clientY: 0  // 你想要点击的位置的 y 坐标
});

// 模拟点击目标元素
targetElement.dispatchEvent(clickEvent);
","adultfriendfinder.com/",1,
r121,4,"","// 定义检测函数
function checkElement() {
    const errorText = ""This zip/postal code is not valid."";
    const elementsWithText = document.querySelectorAll(""*"");
    for (const element of elementsWithText) {
        if (element.textContent === errorText) {
            // 如果存在错误提示文本，则刷新页面
            clearInterval(intervalId);
            location.reload();
            return;
        }
    }
    console.log(""Error text not found. Stopping interval."");
    clearInterval(intervalId); // 如果错误提示文本不存在，停止定时器
}

// 每3秒执行一次检测函数
const intervalId = setInterval(checkElement, 3000);
","",1,
r122,4,"","// 假设我们有这样一个名字的数组
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
'Melanie',
'Melinda',
'Melissa',
'Michelle',];

// 选择一个随机索引
const randomIndex = Math.floor(Math.random() * names.length);

// 使用随机索引从数组中选择一个名字
const randomName = names[randomIndex];

// 将随机选择的英文名字设置为指定输入框的值
document.getElementById('fldID_REG_handle').value = randomName;
","",1,
r125,0,"^title$","If you're interested in me, let's explore fun and creativity together!","adultfriendfinder.com/",1,
r126,4,"","// 生成随机的十位字母
function generateRandomLetters(length) {
  var result = '';
  var characters = 'abcdefghijklmnopqrstuvwxyz';
  var charactersLength = characters.length;
  for (var i = 0; i < length; i++) {
    result += characters.charAt(Math.floor(Math.random() * charactersLength));
  }
  return result;
}

// 获取文本输入框元素
var emailInput = document.getElementById(""fldID_email"");

// 获取或初始化记忆的邮箱地址
var rememberedEmail = localStorage.getItem('randomEmail');
if (!rememberedEmail) {
    rememberedEmail = generateRandomLetters(10) + '@snapmail.cc';
    localStorage.setItem('randomEmail', rememberedEmail);
}

// 将记忆的邮箱地址填入文本输入框
emailInput.value = rememberedEmail;

// 创建悬浮元素1：用于显示随机邮箱地址
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

// 显示随机邮箱地址
floatingDiv1.textContent = rememberedEmail;

// 构建跳转链接
var jumpUrl = ""https://www.snapmail.cc/emailList/"" + rememberedEmail + ""?count=2"";
// 在新标签页中打开链接
window.open(jumpUrl, '_blank');

// 10秒后自动消失
setTimeout(function() {
  floatingDiv1.style.display = 'none';
}, 10000);

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
r128,4,"","// 定义点击函数
function clickElementByXPath(xpath) {
    var element = document.evaluate(xpath, document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue;
    if (element) {
        element.click(); // 模拟点击
    }
}

// 计数器，用于记录点击次数
var clickCount = 0;

// 延迟3秒后开始点击
setTimeout(function() {
    // 定义循环点击函数
    function loopClick() {
        clickElementByXPath('/html/body/div[4]/div[1]/div/div[1]/div/div/form/div[3]/div[2]/div[3]/a[1]');
        clickCount++;

        // 如果点击次数未达到5次，继续点击
        if (clickCount < 5) {
            setTimeout(loopClick, 3000); // 3秒后再次点击
        }
    }

    // 开始循环点击
    loopClick();
}, 3000); // 延迟3秒开始点击
","adultfriendfinder.com/",1,
r127,4,"","// 获取要点击的按钮元素
var button = document.getElementById('fldID_butAction_2');

// 定义点击函数
function clickButton() {
    button.click(); // 模拟点击按钮
}

// 计数器，用于记录点击次数
var clickCount = 0;

// 延迟3秒后开始点击，并设置循环
setTimeout(function() {
    // 第一次点击
    clickButton();
    clickCount++;

    // 设置间隔点击，最多5次
    var intervalId = setInterval(function() {
        if (clickCount < 5) {
            // 如果点击次数未达到5次，继续点击
            clickButton();
            clickCount++;
        } else {
            // 如果点击次数达到5次，停止循环
            clearInterval(intervalId);
        }
    }, 6000); // 3秒点击一次，然后间隔3秒再点击
}, 3000); // 延迟3秒开始点击
","adultfriendfinder.com/",1,
### AUTOFILL OPTIONS ###,,,,,,
advanced,"[]",,,,,
exceptions,"[]",,,,,
textclips,"[]",,,,,
variables,"[]",,,,,
activecat,1,,,,,
attributesoff,0,,,,,
autoimport,0,https://github.com/yuana8702/yuana8702/blob/5d803f6993a177133b9e74791a0193e25280af2c/README.md,,,,
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
