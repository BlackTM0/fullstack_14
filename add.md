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
   <li><a href="ignore.htm">Игнор-лист github</a></li>
    <li><a href="tel:+79621508603"><img src="images/pozvonit.png" alt="Позвонить" title="Позвоните мне"></a></li>
    <li><a href="https://wa.me/79621508603?text=%D0%9F%D1%80%D0%B8%D0%B2%D0%B5%D1%82%2C%20%D0%BC%D0%B0%D0%BC%D0%BA%D0%B8%D0%BD%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%81%D1%82)"><img src="images/napisat-v-vatsapp.png" alt="Написать в Вастапп" title="Напишите мне в WhatsApp"></a></li>       
</ul>
<div class="bodytext">
<p>Команда add в GitHub – это одна из самых часто используемых команд в системе контроля версий Git. Она позволяет добавлять файлы в индекс, чтобы они были готовы к коммиту.

Чтобы использовать команду add, необходимо открыть терминал и перейти в директорию проекта. Затем можно добавить все файлы в индекс с помощью команды:</p>

<b>git add .</b>

<p><img src="images/komanda-add-github.jpg" alt="команда add" title="скриншот команды add" width="700">


Эта команда добавляет все файлы в текущей директории и ее поддиректориях.</p>

<p>Если нужно добавить только определенный файл, то его имя можно указать после команды add:

<b><i>git add file.txt</i></b></p>
<p>


Также можно добавить несколько файлов, перечислив их через пробел:

<b><i>git add file1.txt file2.txt</i></b></p>
<p>

Если файл уже был добавлен в индекс, то повторный вызов команды add не приведет к его дублированию. Однако, если файл был изменен после последнего коммита, то его измененная версия будет добавлена в индекс.</p>

<p>Если нужно удалить файл из индекса, то можно использовать команду:

<b><i>git reset file.txt</i></b>

Эта команда удаляет файл из индекса, но не удаляет его из рабочей директории.</p>
<p>

Команда add – это базовая команда Git, которая позволяет добавлять файлы в индекс. Она является необходимой для создания <a href="commit.htm"><b>коммитов</b></a> и сохранения изменений в репозитории. Поэтому ее использование должно быть хорошо знакомо всем разработчикам, работающим с Git и GitHub.</p></div>