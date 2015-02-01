!SLIDE big ====================================================================================

<div class="right" style="padding-right: 70px">
![](angularjs-500px.png)
</div>

![](img-panique.jpg)

## _AngularJS 2.0... <span class="red">et avant ?</span>_


!SLIDE small ===========================

<br/>

<table class="left" style="margin: 20px 0 40px 120px">
<tr>
<td><img src="data/conf/GDE-2014-Angular JS.svg" width="150px"></td>
<td class="biggest" nowrap>
Thierry Chatel<br/>
<img src="data/conf/methotic.png" width="330px">
&nbsp;&nbsp;&nbsp;
<img src="data/conf/crealead.jpg" width="125px">
</td>
</tr>
</table>

### _Consultant indépendant et formateur AngularJS_

<table class="left" style="margin-left: 200px; padding: 50px">
<tr>
<tr><td>![](i-m.png)</td><td>tchatel@methotic.com</td></tr>
<tr><td>![](i-tw.png)</td><td>@ThierryChatel</td></tr>
<tr><td>![](i-gp.png)</td><td>+ThierryChatel</td></tr>
<tr><td>![](i-gh.png)</td><td>tchatel</td></tr>
</table>



!SLIDE subsection ====================================================================================

# le drame à ngEurope


!SLIDE image ============================

![](tweet01.png)


!SLIDE image ============================

![](tweet02.png)


!SLIDE image ============================

![](tweet03.png)


!SLIDE image ============================

![](tweet04.png)


!SLIDE image ============================

![](tweet05.png)


!SLIDE ======================

## _Réécrire mon_
## _appli AngularJS 1.3 ?_

!SLIDE ======================

## _J’ai besoin d’un framework_
## _qui va durer 10 ans._

!SLIDE small ======================

### _“We need frameworks that are stable and supported long-term;_
### _not that are constantly inventing new concepts_
### _and being rewritten with breaking changes every 5 minutes.”_
[Danny Tuppeny](http://blog.dantup.com/2014/10/have-the-angular-team-lost-their-marbles/)

!SLIDE image ======================

# vraiment, 10 ans ?

![](img-dino.png)

!SLIDE ======================

![](logo-prototype.gif)

### février 2005

!SLIDE ======================

![](logo-scriptaculous.png)

### juin 2005

!SLIDE ======================

## Ajax : asynchronous JavaScript and XML

![](photo-garret.jpg)

###  Jesse James Garrett
### _article du 18 février 2005_


!SLIDE bigger ============================

<table class="left" style="margin-left: 140px">
<tr>
<tr><td style="color: grey">2009</td><td style="color: grey">premier proto</td></tr>
<tr><td>2012</td><td>AngularJS 1.0</td></tr>
<tr><td>2013</td><td>AngularJS 1.2</td></tr>
<tr><td>2014</td><td>AngularJS 1.3</td></tr>
<tr><td>2015</td><td>AngularJS 1.4</td></tr>
<tr><td style="color: green">_2016 ?_</td><td style="color: green">AngularJS 2.0</td></tr>
<tr><td style="color: green">_2018 ?_</td><td style="color: green">fin du support 1.x</td></tr>
</table>



!SLIDE subsection ====================================================================================

# est-ce toujours AngularJS ?

!SLIDE bullets ============================

* plus de contrôleurs
* plus de $scope
* plus de angular.module()
* syntaxe des directives
* syntaxe des templates
* syntaxe d'injection des dépendances

!SLIDE ============================

## nouvelle implémentation
# même vision

![](img-oeil.jpg)


!SLIDE subsection ====================================================================================

# pari risqué ?

!SLIDE bullets ============================

* Struts 2
* Symfony 2
* Play 2
* JSF 2
* Tapestry 5

!SLIDE ============================

## communauté perdue ?

![](img-perdu.jpg)

!SLIDE ============================

## migration ?

![](img-migration.jpg)



!SLIDE subsection ====================================================================================

# pourquoi ?

!SLIDE image  ============================

# _"Designed for the future"_

![](img-orion.jpg)

!SLIDE bullets  ============================

* mobile first
* Web Components
* ECMAScript 6

!SLIDE bullets  ============================

# simplification & cohérence

![](img-cube.png)

!SLIDE  ============================

        @ComponentDirective
        class SantaTodoApp {
          constructor() {
            this.newTodoTitle = '';
          }
          addTodo: function() { ... }
          removeTodo: function(todo) { ... }
          todosOf: function(filter) { ... }
        }


!SLIDE small ============================

    <div>
      <input type="text" [value]="newTodoTitle">
      <button (click)="addTodo()">+</buton>

      <tab-container>
        <tab-pane title="Good kids">
          <div [ng-repeat|todo]="todosOf('good')">
            <input type="checkbox"
                   [checked]="todo.done">
            {{todo.title}}
            <button (click)="deleteTodo(todo)">X</button>
          </div>
        </tab-pane>



!SLIDE subsection ====================================================================================

# démarrer en AngularJS 1.x ?

!SLIDE ========================================

## _meilleur AngularJS à ce jour_

![](img-camion.jpg)

!SLIDE =========================================

## là pour longtemps

![](img-chichen-itza.jpg)

!SLIDE =========================================

## quelles alternatives ?

![](img-glace.jpg)

!SLIDE =========================================

## migration nécessaire ?
### pas si < 5 ans

!SLIDE =========================================

## seulement l'interface web

![](img-web.jpg)


!SLIDE subsection ====================================================================================

# se préparer à la v2

!SLIDE bullets  ============================

# syntaxe "Controller as ..."

* plus proche de la v2

!SLIDE bullets  ============================

# faire des services

* tout le code métier
* tout ce qui peut être isolé
* conserver l'état (plutôt que dans le scope)

!SLIDE bullets  ============================

# faire des directives

* pour alléger les contrôleurs
* pour factoriser les templates

!SLIDE ============================

# faire simple
## et du code clair

!SLIDE ============================

# tests
## unitaires et E2E

!SLIDE bullets  ============================

## double bénéfice
## des
# bonnes pratiques



!SLIDE subsection =======================================================================

# conclusion

!SLIDE ==================================

## choix le moins risqué

![](img-alpinisme.jpg)

!SLIDE ===================================

## v2 = gage d'avenir

![](img-avenir.jpg)
