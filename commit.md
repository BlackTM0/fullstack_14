<html>
<head>
<title>Инструкция GitHub. Автор: Войтенков Дмитрий</title>
<meta name="decription" content="Краткая инструкция по использованию GitHub">
<style type="text/css">
.main-menu {
    list-style: none;
    margin: 0;
    padding: 0;
    margin-top: 60px;
    margin-left:300px;
    font-family: 'Montserrat', sans-serif;   
    /* Для выравнивания меню по центру
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    */
}
.main-menu > li {
    display: inline-flex;
}
.main-menu > li + li {
    margin-left: 20px;
}
.main-menu > li > a {
    padding: 0 0 20px 0;
    position: relative;
    text-transform: uppercase;   
    color: #000;
    font-weight: bold;
    letter-spacing: 0.2px;
    font-size: 15px;
    text-decoration: none;   
}
.main-menu > li > a:hover {
    text-decoration: none;   
    color: #337AB7;
}
.main-menu > li > a:after {
    width: 0;
    height: 3px;
    background-color: #337AB7;
    content: '';
    left: 0;
    bottom: 10px;
    position: absolute;
    transition: all .3s;
}
.main-menu > li > a:hover::after {
    width: 100%;
}
.main-menu > li.active a:after {
    width: 100%;
}
.main-menu li {
    margin: 0;
    white-space: nowrap;
}
.main-menu li.menu-children {
    position: relative;
    margin-right: 12px;
}
.main-menu li.menu-children:after {
    position: absolute;
    content: "\2039";
    color: #337AB7;
    font-size: 20px;
    font-weight: bold;
    right: -12px;
    top: -2px;
    transform: rotate(-90deg);
}
.main-menu li li.menu-children:after {
    position: absolute;
    content: "\2039";
    color: #FFF;
    font-size: 20px;
    font-weight: bold;
    right: 10px;
    top: 12px;
    transform: rotate(180deg);
}
.main-menu li.menu-children:hover > ul {
    opacity: 1;
    visibility: visible;
    transform: translateY(0);
}
.main-menu ul {
    padding: 10px 0;
    margin: 0;
    list-style: none;
    background-color: #337AB7;
    position: absolute;
    z-index: 20;
    min-width: 220px;
    top: 100%;
    left: -30px;
    opacity: 0;
    visibility: hidden;
    transform: translateY(5px);
    transition: all 200ms cubic-bezier(0.43, 0.59, 0.16, 1.25);
}
.main-menu ul li {
    display: block;
    padding: 0 10px;
    line-height: 1.1;
}
.main-menu ul li:last-child {
    margin-bottom: 0;
}
.main-menu ul li a {
    display: block;
    color: #fff;
    padding: 10px;
    transition: all .3s;
    text-decoration: none;   
}
.main-menu ul li a:hover {
    color: #337AB7;
    background: #FFF;
    text-decoration: none;   
}
.main-menu ul ul {
    top: 0;
    left: 100%;
}

.contentimg
{
margin-left:300px;
margin-top: 60px; 
margin-bottom:60px;
width: 700px;
} 
.bodytext
{
margin-left:300px;
margin-right:5px;
margin-top: 5px;
margin-bottom:5px;
font-size:20px;
width:700px;

}

</style></head>
<body>
<ul class="main-menu">
    <li class="active"><a href="index.htm">GitHub: что это и для чего</a></li>
    <li class="menu-children">
        <a href="#url">Основные команды Git</a>
        <ul>
            <li><a href="add.htm">Add</a></li>
            <li><a href="commit.htm">Commit</a></li>
<li><a href="push.htm">Push</a></li>
           
        </ul>
    </li>
    <li><a href="branches.htm">Ветки проектов</a></li>
   <li><a href="ignore.htm">Игнор-лист GitHub</a></li>v
    <li><a href="tel:+79621508603"><img src="images/pozvonit.png" alt="Позвонить" title="Позвоните мне"></a></li>
    <li><a href="https://wa.me/79621508603?text=%D0%9F%D1%80%D0%B8%D0%B2%D0%B5%D1%82%2C%20%D0%BC%D0%B0%D0%BC%D0%BA%D0%B8%D0%BD%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%81%D1%82)"><img src="images/napisat-v-vatsapp.png" alt="Написать в Вастапп" title="Напишите мне в WhatsApp"></a></li>       
</ul>
<div class="bodytext"><p>Команда commit в GitHub - это одна из основных команд, используемых при работе с системой контроля версий. Commit позволяет сохранить изменения в репозитории и отслеживать их историю. </p>

<p><b>При выполнении команды commit необходимо указать сообщение, которое описывает внесенные изменения.</b> Это сообщение должно быть информативным и коротким, чтобы другие участники проекта могли легко понять, что было изменено и почему.</p>

<p>Кроме того, при выполнении команды commit важно следить за тем, чтобы изменения были логически связаны между собой. Также рекомендуется часто выполнять команду commit, чтобы иметь возможность быстро вернуться к предыдущим версиям кода в случае необходимости.</p>

<p>Важно помнить, что команда commit сохраняет изменения только локально. Для того чтобы отправить изменения на сервер GitHub, необходимо выполнить команду push. Перед выполнением команды push рекомендуется убедиться, что все изменения были сохранены с помощью команды commit.</p>

<p>В заключение, команда commit является одной из основных команд при работе с системой контроля версий GitHub. Ее правильное использование позволяет отслеживать историю изменений и быстро возвращаться к предыдущим версиям кода.После нее используется команда <a href="push.htm">PUSH></a></p>

<p><img src="images/add commit.jpg"  width="700" alt="последовательность комманд git add git commit" title="последовательность комманд git add git commit"></p></div>