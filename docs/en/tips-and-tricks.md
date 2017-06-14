Tips and tricks
===============

1. Using HTML content instead text labels

```php
'components' => [
    // ...
    'socialShare' => [
        'class' => \ymaker\social\share\configurators\Configurator::class,
        'socialNetworks' => [
            'facebook' => [
                'class' => \ymaker\social\share\drivers\Facebook::class,
                'label' => \yii\helpers\Html::tag('i', '', ['class' => 'icon-fb']),
            ],
            // ...
        ],
    ],
],
```

2. Translate text labels

```php
'components' => [
    // ...
    'socialShare' => [
        'class' => \ymaker\social\share\configurators\Configurator::class,
        'socialNetworks' => [
            'facebook' => [
                'class' => \ymaker\social\share\drivers\Facebook::class,
                'label' => Yii::t('app', 'Facebook'),
            ],
            // ...
        ],
    ],
],
```

3. Overwrite icon in default icons set

In this example for Facebook will be used `my-facebook-icon` CSS class

```php
'components' => [
    // ...
    'socialShare' => [
        'class' => \ymaker\social\share\configurators\Configurator::class,
        'enableDefaultIcons' => true,
        'icons' => [
            \ymaker\social\share\drivers\Facebook::class => 'my-facebook-icon'
        ],
    ],
],
```