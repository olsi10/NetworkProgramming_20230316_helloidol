# 안녕하세용 hello idol

---

1. start project
    1. pip install django~=3.2
   2. django-admin startproject helloidol .
   3. python manage.py runserver

2. startapp _playground_ 
   1. Terminal
      1. python manage.py startapp _playground_
   2. _helloidol_/settings.py
      1. 'playground', in INSTALLED_APPS

3. playground/ 
   - 정보 전달 : urls -> views -> (models ->) templates
   - 코드 작성 : (models ->)views -> templates -> urls
   1. views
      1. _say_hello( )_
      2. _say_hello_html( )_
      3. _say_bye( )_
      4. -> templates에 context 전달
   2. urls 
      1. _playground/hello/_ -> _say_hello( )_
      2. _playground/hello_html/_ -> _say_hello_html( )_
      3. _playground/bye/_ -> _say_bye( )_
   3. templates/playground/hello.html
      1. hello.html
      2. bye.html
   
4. helloidol/
   1. urls, playground/urls
      1. _playground/_ -> _hello/_ -> _say_hello( )_
      2. _playground/_ -> _hello_html/_ -> _say_hello_html( )_
      3. _playground/_ -> _bye/_ -> _say_bye_html( )_

5. startapp _ive_
   1. Terminal
      1. python manage.py startapp _ive_
   2. helloidol/settings.py
      1. '_ive_' in INSTALLED_APPS

6. helloidol/urls
   1. ive/ -> ive.urls

7. _ive_/
   1. views
      1. show_one( )
      2. show_you( )
   2. urls
      1. ive/ -> one -> show_one()
      2. ive/ -> you -> show_you()
   3. templates/ive/
      1. ~~one.html~~
      2. ~~you.html~~
      3. member.html