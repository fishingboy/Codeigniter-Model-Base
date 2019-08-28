# Codeigniter-Model-Base

## Installation
```
composer require fishingboy/codeigniter-model-base
```

## usage 

If your table name is `users`, You should create model file: `application/models/Users_model.php`

```
<?php

use fishingboy\ci_model_base\CI_Model_Base;

class Users_model extends CI_Model_base
{
    protected $table = "users";
}

```

`Create()`
```php
$this->users_model->create([
  'title' => 'sample'
);
```

`Update()`
```php
$this->users_model->update($id, [
  'title' => 'sample'
);
```

