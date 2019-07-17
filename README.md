# hocita
Extension for Yii2 Framework

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
composer require yii/hocita:1.0.0
```

or add

```
"yii/hocita": "*"
```

to the require section of your `composer.json` file.



Usage
-----
To use it, modify the view .
````php
   /* @var $this yii\web\View */
   use yii\helpers\Html;
   $this->title = 'About';
   $this->params['breadcrumbs'][] = $this->title;
   $this->registerMetaTag(['name' => 'keywords', 'content' => 'yii, developing, views,
      meta, tags']);
   $this->registerMetaTag(['name' => 'description', 'content' => 'This is the
      description of this page!'], 'description');
?>
<div class = "site-about">
   <h1><?= Html::encode($this->title) ?></h1>
   <p>
      This is the About page. You may modify the following file to customize its content:
   </p>
   <h1><?= Hoci\SayHello::world();  ?></h1>
</div>
````

Contact links
[Facebook](https://www.facebook.com/kris.top.50)
[Skype](thangtk2)
