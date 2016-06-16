# chain-functions-php

#### My simple chain method implementation

#### In progress

```php
$t = new MicroChain();

$obj = $t->initialize(TestClass::class, 'findById', function($model) {
    return $model->getId();
}, 83)->push(testClass2::class, 'findById', function ($model) {
    return $model->getId();
})->push(testClass3::class, 'findById', function ($model) {
    return $model->getName();
});

var_dump($obj->getPointer());
```
