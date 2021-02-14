# PHP

PHP magic constants and methods

`__CLASS__`: returns the name of the current class 

`__construct()`: constructor called automatillcally when an object is created \(PHP 5 and up\) 

`__destruct()` : destructor called automatically after object is no more in used \(PHP 5 and up\)

`__get()`: functions as a getter on an object. `__set()`: functions as a setter for getting object data

#### access modifiers

`private` : access only inside the class `protected` : access only within the class or classes that instantiate that class.

#### example

```php
<?php

class User 
{
    private $name = "";
    private $age = "";

    public function __construct($name, $age){
        $this->name = $name;
        $this->age = $age;
    }

    public function __get($property)
    {
        if (property_exists($this, $property)){
            return $this->$property;        
        }
    }

    public function __set($property, $value)
    {
        if(property_exists($this, $property)){
            $this->$property = $value;
        }
        return $this;
    }
}

$user1 = new User("oscar",24);
echo $user1->__get("name");
//OUTPUT: oscar
 $user1->__set("name","juan");
 echo $user1->__get("name");
//OUTPUT: juan
?>
```

### PHP folder structure



_Resources:_

* [login with facebook](https://www.mitrajit.com/login-facebook-using-php-mysql/) 
* [digital marketing](https://indemandcareer.com/)
*  [php object oriented](https://code.tutsplus.com/tutorials/object-oriented-php-for-beginners--net-12762)
* [https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-18-04](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-18-04)
* [https://docs.php.earth/faq/misc/structure/](https://docs.php.earth/faq/misc/structure/)



