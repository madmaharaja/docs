# postLogin

The `postLogin` hook is triggered after a user has logged into the front end. It
passes the user object as argument and does not expect a return value.

> **Tag** Available from version 2.4.3.


## Parameters

1. *FrontendUser* `$objUser`

    The front end user (object) which has been logged in.


## Example

```php
<?php

// config.php
$GLOBALS['TL_HOOKS']['postLogin'][] = array('MyClass', 'myPostLogin');

// MyClass.php
public function myPostLogin(FrontendUser $objUser)
{
    // Do something
}
```


## More information


### References

- [system/libraries/User.php](https://github.com/contao/core/blob/2.11.7/system/libraries/User.php#L301)


### See also

- [postLogout](postLogout.md) - triggered when a user is logged out
